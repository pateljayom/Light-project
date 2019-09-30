# Light-project
Codes for light project
import UIKit

class ViewController: UIViewController {
    
    var lightOn = true
    var colorLight=true
    @IBOutlet weak var buttonChange: UIButton!
    
    override func viewDidLoad() {
        super.viewDidLoad()
        updateUI()
        
        // Do any additional setup after loading the view, typically from a nib.
    }
    
    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }
    
    @IBAction func lightbutton(_ sender: Any) {
        updateUI()
        lightOn = !lightOn
        
    }
    
    @IBAction func button2(_ sender: Any) {
        updateUI2()
        
        colorLight = !colorLight
        
        
    }
    
    func updateUI (){
        if lightOn {
            view.backgroundColor = .white
        } else {
            view.backgroundColor = .black
        }
    }
    
    
    
    
    func updateUI2 (){
        if colorLight {
            view.backgroundColor = .white
            
        } else {
            view.backgroundColor = .black
            
        }
    }
    
}
