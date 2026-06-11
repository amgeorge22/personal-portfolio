<nav class="navbar">
  <div class="navbar-item">
    <a href="https://amgeorge22.github.io/personal-portfolio/home">Home</a>
  </div>
  <div class="navbar-item">
    <a href="#">Mechanical Projects</a>
    <div class="dropdown-content">
      <a href="https://amgeorge22.github.io/personal-portfolio/injection-molded-keychain">Injection Molded Keychain</a>
      <a href="https://amgeorge22.github.io/personal-portfolio/urethane-casting-airpods-case">Urethane Casting Airpods Case</a>
      <a href="#">CNC Machined Box</a>
      <a href="#mechanical4">FSAE Motor Mounting</a>
      <a href="#mechanical5">Tilt-In-Space Wheelchair</a>
      <a href="#mechanical6">Beam Deflection Calculator</a>
      <a href="#mechanical7">3D Printing Variability Study</a>
    </div>
  </div>
  <div class="navbar-item">
    <a href="#">Robotics/Mechatronics Projects</a>
    <div class="dropdown-content">
      <a href="#robotics1">Autonomous Robot Mapping & Navigation</a>
      <a href="#robotics2">Apple Orchard Leaf Blower</a>
      <a href="#robotics3">Corn Stalk Nitrogen Sensing Attachment</a>
      <a href="#robotics4">Automated Poker Dealer</a>
      <a href="#robotics5">Inverted Pendulum Controller</a>
    </div>
  </div>
  <div class="navbar-item">
    <a href="#">Software Projects</a>
    <div class="dropdown-content">
      <a href="#software1">Sudoku Solving with Graph Coloring</a>
      <a href="#software2">Machine Learning Spot-It! Model</a>
      <a href="#software3">SoftDew Valley - Stardew Valley Clone</a>
      <a href="#software4">Poi Style Classifier</a>
    </div>
  </div>
  <div class="navbar-item">
    <a href="#">Research Papers</a>
    <div class="dropdown-content">
      <a href="#research1">When Is It Relevant?</a>
      <a href="#research2">Student Voice in Collaborative AutoEthnography</a>
    </div>
  </div>
</nav>

As part of my Design for Manufacturing course, I designed and fabricated a precision-machined “treasure box” to hold two poker blind chips. 

The goal of this project was to design two interlocking halves that could be machined on a CNC mill out of  3" x 3" x 1.25" aluminum stock. The box had to have internal geometry to secure an object of our choice and could fit whatever aesthetic we wanted. I chose to design my box to hold two poker blind chips, both of which were 1.875" in diameter. The overall shape of the box was a spade, to fit with the poker theme. The two halves of the box were aligned with a 0.25" dowel pin and 0.25" diamond pin for easy assembly.

![closed spade box](assets\cnc-machined-box\spade-box.jpg)
![open spade box](assets\cnc-machined-box\flat-open.jpg)

The final project is pictured above. It successfully holds two poker chips, and both of them are easy to remove due to the machined divots next to the hole that holds the chips. The two halves are also easy to align and remove, allowing the box to be opened and closed many times. While the shape of the box fits my intended aesthetic very well, I hope to be able to powder coat the box black in the near future.

![final CAM](assets\cnc-machined-box\cam-bottom.jpg)
![roughing CAM](assets\cnc-machined-box\spade-top.jpg)
![in CNC](assets\cnc-machined-box\machining-bottom.jpg)
![at CNC 1](assets\cnc-machined-box\me-machining-top1.jpg)
![at CNC 2](assets\cnc-machined-box\me-machining-top2.jpg)
![Tormach display panel](assets\cnc-machined-box\top-tormach-path.jpg)

This project marked my first full workflow from CAD to CAM to machining. I generated all toolpaths in Fusion 360 and machined the components on a Tormach CNC mill, gaining hands-on experience with setup, workholding strategy, and multi-operation machining. The parts were produced using a pedestal milling approach, with excess stock faced off in a secondary operation to achieve final geometry and surface finish.

![finished in CNC](assets\cnc-machined-box\pedestal-milling.jpg)
![box with jig (pre-pedestal milling)](assets\cnc-machined-box\pre-pedestal-w-jig.jpg)

One of the challenges with this project was the pedestal milling. Part of the geometry of the spade is the point at the end, which is not easy to clamp onto with a vise in the CNC mill. I designed and 3D printed a custom jig to hold the point, which allowed me to securely clamp the piece in the mill and successfully remove excess stock from the bottom of both of the halves.

![exploded CAD front](assets\cnc-machined-box\front-box-assembly.jpg)
![exploded CAD iso](assets\cnc-machined-box\iso-box-assembly.jpg)

Another challenge was determining the tolerances of the alignment holes that the pins were set in. One of the pins was a dowel pin, which had a diameter of 0.25" throughout. The other was a diamond pin, which had a shank with a diameter of 3/16" and a diamond head diameter of 0.25". I used a reamer for the 0.25" holes in order to ensure that they were concentric and the correct diameter for my dowel pins. The fit on these holes is good - the dowel pin fits snugly with very little wiggle, but is still easy to remove if necessary. I failed to realize that the shank of the diamond pin required equally precise tolerance. I simply used a 3/16" drill bit, and, as a result, there is a small amount of wiggle. While the two halves of the box fit together well, this small amount of wiggle prevents it from being as polished a final product as it could be.

While machining the two halves of the box, I was worried that it would be difficult to slide the pins into the box. To avoid this, I added a chamfer to all the holes in the box. This makes it easy to drop the poker chips into the box, as well as getting the pins in place.



Overall, this was a successful project that taught me a lot about designing for CNC machining, how to set up CAM, and how to operate a CNC mill. I also learned how to tolerance a part to ensure proper fit, which will continue to be useful for future projects.

### Manufacturing Details
#### List of Operations (Top Half)
- Facing (2" face mill)
- Roughing Cuts (3/4" flat end mill and 1/4" flat end mill)
- Drilling & Reaming (3/16" drill bit, 1/4" drill bit, 1/4" reamer)
- Finishing Cuts (3/4" flat end mill and 1/4" flat end mill)
- Chamfer (chamfer mill)

![top half CAM](assets\cnc-machined-box\top-operations.jpg)

#### List of Operations (Bottom Half)
- Facing (2" face mill)
- Roughing Cuts (3/4" flat end mill and 1/4" flat end mill)
- Drilling & Reaming (3/16" drill bit, 1/4" drill bit, 1/4" reamer)
- Finishing Cuts (3/4" flat end mill and 1/4" flat end mill)
- Chamfer (chamfer mill)

![bottom half CAM](assets\cnc-machined-box\bottom-operations.jpg)

### Drawings
![top drawing](assets\cnc-machined-box\spade-box-top-drawing.jpg)
![bottom drawing](assets\cnc-machined-box\spade-box-bottom-drawing.jpg)
![assembly drawing](assets\cnc-machined-box\spade-box-assembly-drawing.jpg)

### BOM
![Bill of Materials](assets\cnc-machined-box\BOM.png)


<style>
  .navbar {
    background-color: #0066cc;
    padding: 0;
    margin: -20px -20px 30px -20px;
    display: flex;
    justify-content: center;
    align-items: stretch;
    gap: 0;
    flex-wrap: nowrap;
  }
  
  .navbar-item {
    position: relative;
    display: inline-flex;
    flex: 1 1 auto;
    min-width: 0;
  }
  
  .navbar-item > a {
    display: block;
    color: white;
    text-align: center;
    padding: 12px 14px;
    text-decoration: none;
    font-size: 14px;
    white-space: nowrap;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  
  .navbar-item > a:hover {
    background-color: #004499;
  }
  
  .dropdown-content {
    display: none;
    position: absolute;
    background-color: #004499;
    min-width: 200px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    z-index: 1;
    top: 100%;
    left: 0;
  }
  
  .dropdown-content a {
    color: white;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
    transition: background-color 0.3s ease;
  }
  
  .dropdown-content a:hover {
    background-color: #003366;
  }
  
  .navbar-item:hover .dropdown-content {
    display: block;
  }
</style>