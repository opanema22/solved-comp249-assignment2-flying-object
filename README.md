Download Link: https://assignmentchef.com/product/solved-comp249-assignment2-flying-object
<br>
The purpose of this assignment is to practice class inheritance, and other Object Oriented Programming concepts such as constructors, access rights, method overriding, etc. The assignment would also allow you to practice the notion of package creation. This assignment contains two parts. You need to complete part I to be able to do part II. You should however handle each part as if it was a separate assignment (i.e. you should not modify Part I after finishing with it; rather create a copy of that part and use it to create Part II. This is needed so that you can finally submit both parts!

<strong><u>Part I</u> </strong>

Various flying objects can be described as follows:

− An <strong>Airplane</strong> class, which has the following attriobutes: a <em>brand</em> (String type), <em>price</em> (double type)  and <em>horse power</em> (int type).                                                                                                        **

−

−

−

−

(double type).




** All images have been obtained from, and © <u>wikipedia.org</u>

− An          <strong>AgriculturalDrone</strong>      (which is          used     for        crop production) is <strong>UAV</strong> that additionally has the following: <em>brand </em>(Sting type), and <em>carry capacity</em> (int type).




− A <strong>MAV (Micro Air Vehicle)</strong>, is a<a href="https://en.wikipedia.org/wiki/Miniature_UAV"> miniature </a><a href="https://en.wikipedia.org/wiki/Miniature_UAV"><strong>UAV</strong></a> that has a size restriction (and can be as small as few centimeters. It has the following: <em>model</em> (String type) and <em>size</em> (double type).







<strong><u>Phase I:</u></strong>




<ol>

 <li>Draw a UML representation for the hierarchy of the above-mentioned Your representation must also be accurate in terms of UML representation of the different entities and the relation between them. You must use a software to draw your UML diagrams (no hand-writing/drawing is allowed).</li>

</ol>




<ol start="2">

 <li>Write the implementation of the above-mentioned classes using inheritance and according to the specifications and requirements given below:</li>

</ol>




<ul>

 <li>You must have 5 different Java packages for the classes. The first package will include the <strong>Airplane</strong> The second package will include the <strong>Helicopter</strong>, and the <strong>Quadcopter </strong>classes.</li>

</ul>

The third package will include the <strong>Multirotor</strong> class. The fourth package will include <strong>UAV </strong>class, and the last package will include the <strong>AgriculturalDrone</strong> and <strong>MAV</strong> classes.




<ul>

 <li>For each of the classes, you must have at least three constructors, a default constructor, a parametrized constructor (which will accept enough parameters to initialize ALL the attributes of the created object from this class) and a copy constructor. For instance, the parametrized constructor of the <strong>Quadcopter </strong>class must accept 7 parameters to initialize the <em>brand</em>, the <em>price</em>, the <em>horse power</em>, the <em>number of cylinders</em>, the <em>creation year</em>, the <em>passenger capacity</em>, and the <em>maximum flying speed</em>.</li>

</ul>




<ul>

 <li>An object creation using the default constructor must trigger the default constructor of its ancestor classes, while creation using parametrized constructors must trigger the parametrized constructors of the ancestors.</li>

</ul>




<ul>

 <li>For each of the classes, you must include at least the following methods: accessors, mutators, <strong><em>toString()</em></strong> and <strong><em>equals()</em></strong> methods (notice that you are always <u>overriding</u> the last two methods).</li>

</ul>




− The <strong><em>toString()</em></strong> method must return clear description and information of the object (i.e <em>“This Agricultural Drone is manufactured by Agridrones. It weights 340 pounds, and costs 98000$. It can carry up to 25 Kg….</em>).




− The <strong><em>equals() </em></strong>method must first verify if the passed object (to compare to) is null and if it is of a different type than the calling object. The method would clearly return false if any of these conditions is true; otherwise the comparison of the attributes is conducted to see if the two objects are actually equal. Two objects are equal if the values of all their attributes are equal.




<ul>

 <li><u>For all classes you <strong>must</strong> use the appropriate access rights, which allow most ease of use/access</u> <strong><u>without compromising security</u></strong><u>. Do not use most restrictive rights unless they make sense!</u></li>

 <li><u>When accessing attributes from a base class, you must take full advantage of the permitted rights.</u> For instance, if you can directly access an attribute by name from a base class, then you must do so instead of calling a public method from that base class to access the attribute.</li>

</ul>




<ol start="3">

 <li>Write a driver program (that contains the main() method) that would utilize all of your classes. The driver class can be in a separate package or in any of the already existing packages. In the main() method you must:

  <ul>

   <li>Create various objects from the 7 classes, and display all their information (you must take advantage of the <strong><em>toString()</em></strong> method).</li>

   <li>Test the equality of some of the created objects using the <strong><em>equals()</em></strong></li>

   <li>Create an array of 15 to 20 these flying objects (<strong><u>HINT</u></strong>: Do you need to add something else to the classes described above? If so; go ahead with that!) and <u>fill that array with</u> <u>various objects from these classes</u> (each class must have at least one entry in that array).</li>

   <li>Trace(search) that array to find the two objects that have the least expensive price (that is least expensive and second least expensive). Display all information of these two objects along with their location (index) in the array.</li>

  </ul></li>

</ol>

<strong> </strong>

<strong><u>Phase II</u>  </strong>

<em> </em>

In that phase, you need to modify/expand the implementation from Phase I as follows:







<ol>

 <li>In the driver program, you need to add another static method (add it above the main() method), called <strong><em>copyFlyingObjects</em></strong>. The method will take as input an array of these objects (the array can be of any size) and returns a copy of that array. That is to say, the method needs to create an array of the same length as the passed array, copies all objects from the passed array to a new array, then returns the new array. Your copy of the objects <strong><u>will automatically</u></strong> depend on the <u>copy constructors</u> of the different listed classes. You <strong><u>must</u></strong> consider ther following restrictoins: <strong><u>Do NOT attempt</u> to explicitly find the exact type of the objects being copied, <u>do NOT</u> <u>attempt</u> to find the object type inside the copy constructors and <u>Do NOT use clone().</u>  </strong></li>

</ol>

<strong> </strong>

<ol start="2">

 <li>In the driver program, create an array of 15 to 20 objects (must have at least one from each of the classes), then call the <em>copyFlyingObjects()</em> method to create a copy of the that array.</li>

</ol>




<ol start="3">

 <li>Display the contents of both arrays, then add some comments indicating <strong><u>whether or not the</u> <u>copying is correct.</u> </strong><strong><u>If not; you need to explain why it has not been successful or as you might</u></strong><strong> <u>have expected.</u> </strong></li>

</ol>

<strong> </strong>

<strong>General Guidelines When Writing Programs  </strong>

<ul>

 <li>Include the following comments at the top of each class you are writing.</li>

</ul>

// —————————————————–

// Part: (include Part Number)

// Written by: (include your name(s) and student ID(s))

// —————————————————–




<ul>

 <li><u>Use <strong>JavaDoc</strong> to create the documentations of your program.</u> Use appropriate comments when needed.</li>

 <li>Display clear prompts for the user whenever you are expecting the user to enter data from the keyboard.</li>

 <li>All outputs should be displayed with clear messages and in an easy to read format.</li>

 <li>End your program with a closing message so that the user knows that the program has terminated.</li>

</ul>