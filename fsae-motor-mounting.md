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
      <a href="#">FSAE Motor Mounting</a>
      <a href="https://amgeorge22.github.io/personal-portfolio/tilt-in-space-wheelchair">Tilt-In-Space Wheelchair</a>
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

As a part of Olin Electric Motorsports (Formula SAE), I designed and fabricated a mounting system that withstands load cases of up to 10,500 Newtons in order to safely secure our race car motor to the chassis. I conducted topology studies to optimize light-weighting of the mounting plates and utilized Finite Element Analysis (FEA) to ensure a minimum 1.5 factor of safety on our plates and brackets. Check out [<a href="https://docs.google.com/presentation/d/1Rq5lbfT-gt4GSHfbYNGIG5v_Nh4KfM8RXztWXbIOif4/edit?usp=sharing" target="_blank">this detailed breakdown</a>] to understand the design decisions made! 

![clockage render](assets\fsae-motor-mounting\clockage-render.jpg)
![clockage in car iso view](assets\fsae-motor-mounting\clockage-in-car-iso.jpg)
![clockage in car top view](assets\fsae-motor-mounting\clockage-in-car-top.jpg)
![physical clockage](assets\fsae-motor-mounting\clockage-phyiscal-assembly.jpg)
![output plate analysis](assets\fsae-motor-mounting\FEA-output-plate.jpg)
![motor mounting plate analysis](assets\fsae-motor-mounting\topology-input-plate.jpg)
![plate overview](assets\fsae-motor-mounting\output-plate-overview.jpg)
![system diagram](assets\fsae-motor-mounting\system-diagram.jpg)


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