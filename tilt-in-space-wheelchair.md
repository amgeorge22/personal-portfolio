<nav class="navbar">
  <div class="navbar-item">
    <a href="https://amgeorge22.github.io/personal-portfolio/home">Home</a>
  </div>
  <div class="navbar-item">
    <a href="#">Mechanical Projects</a>
    <div class="dropdown-content">
      <a href="https://amgeorge22.github.io/personal-portfolio/injection-molded-keychain">Injection Molded Keychain</a>
      <a href="https://amgeorge22.github.io/personal-portfolio/urethane-casting-airpods-case">Urethane Casting Airpods Case</a>
      <a href="https://amgeorge22.github.io/personal-portfolio/cnc-machined-box">CNC Machined Box</a>
      <a href="https://amgeorge22.github.io/personal-portfolio/fsae-motor-mounting">FSAE Motor Mounting</a>
      <a href="#">Tilt-In-Space Wheelchair</a>
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

For the class Mechanical Design, I worked in a team of four alongside [<a href="https://www.kyaroassistive.org" target="_blank">(Kyaro Assistive Tech)</a>] to create a “Tilt-In-Space” wheelchair. Our wheelchair is able to rotate backwards in increments of 15°, and lock in place at each increment. It is designed to be easy to manufacture (able to be machined within the shop capabilities in Tanzania) and easy to operate. To make it easy to manufacture, we modified the original Kyaro wheelchair design, ultimately creating an additional 5 unique parts to be added to the original design. 

The wheelchair was designed in OnShape, and any unique parts and modifications to the original wheelchair were physically prototyped. 
To learn more about the project, check out the website here: [<a href="https://sites.google.com/view/tiltinspacewheelchair/home" target="_blank">(https://sites.google.com/view/tiltinspacewheelchair/home)</a>]

![exploded front](assets\tilt-in-space-wheelchair\exploded-front)
![exploded central frame](assets\tilt-in-space-wheelchair\exploded-central-frame)
![expoded iso](assets\tilt-in-space-wheelchair\exploded-iso)
![exploded top](assets\tilt-in-space-wheelchair\exploded-top)
![CAD central frame + linkage](assets\tilt-in-space-wheelchair\cad-central-frame-and-linkage)
![CAD full chair](assets\tilt-in-space-wheelchair\cad-full-chair)
![CAD full chair iso tilted back](assets\tilt-in-space-wheelchair\cad-full-chair-iso-tilted)
![CAD full chair iso upright](assets\tilt-in-space-wheelchair\cad-full-chair-iso-upright)

### WIP 
- Add photos of chair in action and go into more detail in general
- reorder CAD photos to an order that makes sense
- Add labels to CAD photos

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