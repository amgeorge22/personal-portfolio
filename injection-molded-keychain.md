<nav class="navbar">
  <div class="navbar-item">
    <a href="https://amgeorge22.github.io/personal-portfolio/home">Home</a>
    <div class="dropdown-content">
    </div>
    <a href="#">Mechanical Projects</a>
    <div class="dropdown-content">
      <a href="#">Injection Molded Keychain</a>
      <a href="https://amgeorge22.github.io/personal-portfolio/urethane-casting-airpods-case">Urethane Casting Airpods Case</a>
      <a href="#mechanical3">DFM Treasure Box</a>
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

As part of my Design for Manufacturing course, I designed and fabricated an injection molded keychain.

The goal of this project was to design a part using injection molding that interfaced with at least one other component. The injection molded part had to be smaller than 5" x 3" x 3" and less than 2 cubic oz of plastic in order to work with our school's injection molder.

We created a mold that would create two keychains per shot of plastic. Once the injection molding is complete, the keychain is added via a split ring.

![keychains on table](assets\injection-molded-keychains\keychains.jpg)

The final project is pictured above. The partner I was working with and I were both involved in the musical Cinderella this semester, and we wanted to commemorate the experience with these keychains. The overall shape of the keychain is based on the glass slipper from the show, and the text on the keychain says "Cinderella" and "2026".

The first step of this project was creating the design of the keychain. I used SOLIDWORKS to design the keychain. Once the initial CAD was done, I used SOLIDWORKS' built in Flow Analysis and Mold Analysis tools to verify the design.

![basic CAD of shoe keychain](assets\injection-molded-keychains\basic-shoe-cad.png)
The initial keychain CAD, featuring a hole that the split ring of the keychain attaches to, the "Cinderella 2026" text, and a decorative raised edge.

![Flow Analysis of Single Keychain](assets\injection-molded-keychains\shoe-flow-analysis.png)
The flow analysis of a singular keychain. The chosen injection point is the heel of the slipper. The parting line (where the mold parts) is the flat back of the keychain. The chosen material for the keychain is polypropylene. It takes about three and a half seconds for plastic to flow through the whole keychain, which is an acceptable range.
![Mold Analysis of Single Keychain](assets\injection-molded-keychains\shoe-mold-analysis.png)
The mold analysis of a singular keychain. The parting line is the flat back of the keychain. This analysis was done with a 3 degree draft angle, meaning that regions that do not have a 3 degree or greater draft would be highlighted in yellow. This draft angle makes it easier to remove the part from the mold.

Once the design of the initial shoe was complete, it was time to create the full injected part. Because this part is so small, we were able to include two keychains in one mold. There are several features that injection molding requires in order to create a successful part:
- Sprue:  The sprue is where plastic is injected into the mold.
- Runners: Runners carry plastic from the sprue to the part being molded. Full round is the most efficient runner shape, which is being used here
- Gates: Gates choke off the flow and spread of plastic by making it flow through a very narrow part. To remove a part from the full injected part, the part is broken off at the gate, which is easy to do because of how thin the gate is.
- Cold Slug Well: The cold slug well catches cold (hardened) plastic at the tip of the injection nozzle, so this cold part does not enter the runners. 

The fully injected part looked like this:
![Full Injection Molded Part](assets\injection-molded-keychains\injection-molded-part-w-terms.png)

Once the fully injected part is designed, I once again do flow analysis to verify the design.

![Flow Analysis of Full Injection Molded Part](assets\injection-molded-keychains\whole-part-flow-time.png)
The flow analysis of the full part. Flow analysis here looks promising and very similar to the singular keychain design. The fill time is just below four seconds, which is a reasonable amount of time for our injection molder.
![Ease of Separation Analysis of Full Injection Molded Part](assets\injection-molded-keychains\whole-part-ease-flow.png)
The ease of fill of the fill part. The part is all green, which means that it should be easy for the plastic to flow to all corners of the part. The purple spheres represent air traps. This is useful because it tells use where to scratch in air vents (details below).

It looks like our part should have no issues when it comes to plastic flow. Now I can use SOLIDWORKS' mold tools to create the mold for this part.
![Mold Analysis of Full Injection Molded Part](assets\injection-molded-keychains\whole-part-mold-analyis.png)
The mold analysis of the full part. Like the last mold analysis, this was done with a three degree draft angle. The lack of yellow signifies that there should be no mold separation issues.
![Full mold in CAD](assets\injection-molded-keychains\full-mold.png)
The full mold
![Top half of mold in CAD](assets\injection-molded-keychains\top-mold.png)
The top half (cavity) of the mold. The tabs at the top and bottom of the mold fit a pry bar to allow for easier mold separation.
![Bottom half of mold in CAD](assets\injection-molded-keychains\bottom-mold.png)
The bottom half (core) of the mold. Because the flat back of the keychain is the parting line, this part of the mold does not have any keychain features and only has the runners, gates, and cold slug well.

Once the design of the mold was done, I handed it off to my partner to do the CAM and CNC manufacturing of the part (to see more of my own CAM and CNC experience, check out this project!). Once the machining is done, we scratched air vents into the toe and the top of the heel in order to allow air to escape. These locations were informed by the air gaps in my ease of flow analysis. The final mold is pictured below:
![Machined mold](assets\injection-molded-keychains\machined-mold.jpg)

You might notice that this mold does not have the decorative raised edge that the initial part has. One of our challenges was figuring out how to create that feature in CAM, so we chose to remove it in order to create a simpler part.

Finally, it's time to do the injection molding! 

We ran into a couple issues during the injection molding process. This primarily manifested as undershooting, which is when the plastic does not flow to all parts of the mold. This symptom was caused by two issues:
- The stack height of our mold (the overall height of the mold) was incorrect. This made it so not enough pressure was being used to shoot the plastic into the mold.
- Our desired material (clear polypropylene) was older than other materials available to us, and had to much moisture to allow for smooth flow. Switching to other colors (such as pink and blue) resolved this issue.
By overcoming these issues we were able to successfully create our part.
![undershot-part](assets\injection-molded-keychains\undershot-in-mold.jpg)
An image of an undershot part. We can see the plastic flow through the sprue, runners, and enter the keychain, but the plastic fails to reach the toe of the slipper

![Successful shot with blue PPE](assets\injection-molded-keychains\blue-keychains-in-mold.jpg)
The mold with a successful shot of plastic using blue polypropylene
![Full part removed from mold](assets\injection-molded-keychains\blue-keychains-w-attached-sprue.jpg)
The full part removed from the mold
![Parts disconnected from runner](assets\injection-molded-keychains\blue-keychains-w-detatched-sprue.jpg)
The part disconnected from the sprue and runners. The gate allows for clean separation of the keychain.
![Final keychain](assets\injection-molded-keychains\blue-keychain.jpg)
The final keychain!

Once the keychain was out of the mold, it was fairly simple to attach the chain. The thickness of the slipper made it slightly difficult to fit the split ring around the hole, so future iterations of the keychain would be slightly thinner.

### Cost Analysis
Mold: The mold blanks we used (which include the sprue and machined holes for alignment pins) cost approximately $100 each. In addition to this, we did roughly 1 hour of machining (30 minutes on the cavity and 5 minutes on the core, plus setup time), which would cost about $30 (based off of machinist pay in MA). This makes the total cost of the mold approximately $230.

Alignment Pins: We used the following alignment pins, adding up to a total of $51.40.
- Hole Liner: $14.27 (x2)
- Diamond Pin: $16.02 (x1)
- Round Pin: $6.84 (x1)

Plastic: Our keychains are made out of polypropylene, which on average costs $1.43/kg. The full part weights 11.28g, meaning the plastic for the keychain costs $0.08 per part.

Chain: We bought these keychains off Amazon, which cost $4.69 for a pack of 50, putting the cost at roughly $0.10/chain.


Total Cost for 10,000: The total upfront cost is $281.40, and the price per full keychain is $0.18. For 10,000 keychains, the total cost per keychain would be approximately $0.21. This does not include the labor costs for the actual injection molding process or the assembly process.

<style>
  .navbar {
    background-color: #0066cc;
    padding: 0;
    margin: -20px -20px 30px -20px;
    display: flex;
    justify-content: center;
    gap: 0;
  }
  
  .navbar-item {
    position: relative;
    display: inline-block;
  }
  
  .navbar-item > a {
    display: block;
    color: white;
    text-align: center;
    padding: 16px 20px;
    text-decoration: none;
    font-size: 16px;
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