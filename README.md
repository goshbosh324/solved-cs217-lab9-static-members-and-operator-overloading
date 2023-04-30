Download Link: https://assignmentchef.com/product/solved-cs217-lab9-static-members-and-operator-overloading
<br>
<h1>Task 1</h1>

We want to create a class of Counter, the object of which holds the count of anything. Also we want to keep track of total objects of class and serial No of each object. Write a class Counter. This class has three private data members:

<ul>

 <li>count : An integer that holds a count value.</li>

 <li>objCount: An integer that holds the count of objects.</li>

 <li>serialNo: An integer that holds the serial number of objects of Counter class.

  <ul>

   <li>Write a default constructor that initializes each data member of the class such that count with 0, objCount that increments the count of the objects and serialNo with the correct serial no (object 1 should have serial no 1, object2 should have serial no 2 and so on). Counter()</li>

   <li>Write a constructor that accepts an argument int c that is assigned to the data member count. Also initialize objCount that increments the count of the objects and serialNo with the correct serial no (object 1 should have serial no 1, object2 should have serial no 2 and so on). Counter(int c)</li>

   <li>Write destructor of the class which adjust the count of Objects. Counter()</li>

   <li>Create the getter-setter functions for the data members.</li>

  </ul></li>

 <li>void setCount(int c)</li>

 <li>int getCount()const</li>

 <li>int getSerialNo()const</li>

 <li>static int getObjCount()</li>

 <li>static int IncrementObjCount()

  <ul>

   <li>Define operator = that assigns the value of count to the left hand operand.</li>

   <li>Define “-” unary operator that inverts the value of count data member for counter class and should allow the statements like <em>c</em>1 = −<em>c</em>1; or <em>c</em>2 = −<em>c</em>1;</li>

   <li>Write main function to test all the implemented functionality.</li>

  </ul></li>

</ul>

<h1>Task 2</h1>

Write a class Distance that holds distances or measurements expressed in feet and inches. This class has two private data members:

<ul>

 <li>feet: An integer that holds the feet.</li>

 <li>inches: An integer that holds the inches.

  <ul>

   <li>Write a constructor with default parameters that initializes each data member of the class such that int f is assigned to feet and int i is assigned to inches (Default values 0)</li>

  </ul></li>

</ul>

<strong>If inches are greater than equal to 12 then they must be appropriatly converted to corresponding feet</strong>

<ul>

 <li>Generate appropriate getter-setter functions for the data members.</li>

</ul>

<ul>

 <li>bool setFeet(int f)</li>

 <li>int getFeet()const</li>

 <li>bool setInches(int i) It should ensure proper conversion to feets.</li>

 <li>int getInches()const

  <ul>

   <li>Define an operator+ that overloads the standard + math operator and allows one Distance object to be added to another. Distance operator+(const Distance &amp;obj)</li>

   <li>Define an operator- function that overloads the standard – math operator and allows subtracting one Distance object from another. Distance operator-(const Distance &amp;obj)</li>

   <li>Define an operator<em>&gt; </em>function that overloads the <em>&gt; </em>operator and returns true if the calling object contains a value greater than that of the parameter and returns false otherwise. bool operator&gt;(const Distance &amp;obj)</li>

   <li>Define an operator<em>&lt; </em>function that overloads the <em>&lt; </em>operator and returns true if the calling object contains a value smaller than that of the parameter and returns false otherwise. bool operator&lt;(const Distance &amp;obj)</li>

   <li>Define an operator= function that overloads the = operator and assign one Distance object to another. const Distance operator=(const Distance &amp;obj)</li>

   <li>Write main function to test all the implemented functionality.</li>

  </ul></li>

</ul>

<h1>Task 3</h1>

Design a class Complex for handling Complex numbers and include the following:

<ul>

 <li>real: a double</li>

 <li>imaginary: a double</li>

</ul>

The class has the following member functions.

<ul>

 <li>A constructor initializing the number with default parameters.</li>

 <li>Getters and Setters of the class data members as given below</li>

</ul>

<ul>

 <li>void setReal(double r)</li>

 <li>double getReal()const</li>

 <li>void setImaginary(double i)</li>

 <li>double getImaginary() const</li>

</ul>

Overload the following operators in the class by identifying their return types.

<ul>

 <li>Overload the binary + operator which adds two complex numbers.</li>

 <li>Overload the binary – operator which subtracts the complex number passed as argument from the caller object.</li>

 <li>Overload the binary * operator to multiply two complex numbers.(Think about its return type).</li>

 <li>Overload binary assignemnt = operator, think about its return type.</li>

 <li>Overload binary == operator which returns true if operands are equal and returns false otherwise.</li>

 <li>Overload unary ! operator which returns true if the real and the imaginary parts are zero, otherwise return false. bool opeator!()const</li>

 <li>Write main function to test all the implemented functionality.</li>

</ul>

<h1>Task 4</h1>

Write a class called Date that represents a date consisting of a year, month, and day. A Date object should have the following methods and operators:

You are given the operation and you have to overload the required operator for the objects of class.

<table width="607">

 <tbody>

  <tr>

   <td width="214"> </td>

   <td width="394"> </td>

  </tr>

  <tr>

   <td width="214">Date(int year, int month, int day)</td>

   <td width="394">Constructs a new Date object to represent the given date.</td>

  </tr>

  <tr>

   <td width="214">operator =</td>

   <td width="394">Overload = operator to assign values.</td>

  </tr>

  <tr>

   <td width="214">d2=d1+1</td>

   <td width="394">Overload + operator which takes integer as argument . It moves this Date object forward in time by the given number of days.</td>

  </tr>

  <tr>

   <td width="214">d2=d1-4</td>

   <td width="394">Overload – operator which takes integer as argument . It moves this Date object backward in time by the given number of days.</td>

  </tr>

  <tr>

   <td width="214">d3=d1+d2</td>

   <td width="394">Overload + operator which takes Date object as argument.</td>

  </tr>

  <tr>

   <td width="214">d3=d1-d2</td>

   <td width="394">Overload – operator which takes Date object as argument.</td>

  </tr>

  <tr>

   <td width="214">bool a=d1<em>&gt;</em>d2;</td>

   <td width="394">Overload <em>&gt; </em>operator which returns true or false.</td>

  </tr>

  <tr>

   <td width="214">bool a=d1<em>&gt;</em>=d2;</td>

   <td width="394">Overload <em>&gt;</em>= operator which returns true or false.</td>

  </tr>

  <tr>

   <td width="214">bool a=d1<em>&lt;</em>d2;</td>

   <td width="394">Overload <em>&lt; </em>operator which returns true or false.</td>

  </tr>

  <tr>

   <td width="214">bool a=d1<em>&lt;</em>=d2;</td>

   <td width="394">Overload <em>&lt;</em>= operator which returns true or false.</td>

  </tr>

  <tr>

   <td width="214">bool d1!=d2;</td>

   <td width="394">Overload != operator which returns true or false.</td>

  </tr>

  <tr>

   <td width="214">bool d1==d2;</td>

   <td width="394">Overload == operator which returns true or false.</td>

  </tr>

  <tr>

   <td width="214">int getDay()</td>

   <td width="394">Returns the day value of this date; for example, for the date 2006/07/22, returns 22.</td>

  </tr>

  <tr>

   <td width="214">int getMonth()</td>

   <td width="394">Returns the month value of this date; for example, for the date 2006/07/22, returns 7.</td>

  </tr>

  <tr>

   <td width="214">int getYear()</td>

   <td width="394">Returns the year value of this date; for example, for the date 2006/07/22, returns 2006.</td>

  </tr>

  <tr>

   <td width="214">bool isLeapYear()</td>

   <td width="394">Returns true if the year of this date is a leap year. A leap year occurs every four years, except for multiples of 100 that are not multiples of 400. For example, 1956, 1844, 1600, and 2000 are leap years, but 1983, 2002, 1700, and 1900 are not.</td>

  </tr>

  <tr>

   <td width="214">String toString()</td>

   <td width="394">Returns a String representation of this date in year/month/day order, such as “2006/07/22”.</td>

  </tr>

 </tbody>

</table>

<strong>Write </strong>main <strong>function to test all the implemented functionality.</strong>