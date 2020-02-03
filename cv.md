# **Misyukevich Darya**
## Contacts
E-mail: <missukevitch@gmail.com>  
Phone: [+375 (29) 573 10 79](tel:+375295731079)
## Summary
I want to became a good web developer. I hope that my work will bring me pleasure and good income. I am purposeful, hardworking and I have a great desire to learn and develop.
## Skills
* Figma, Photoshop, Illustrator
* HTML
* CSS
* JS
* C++
## Code examples
~~~
var students = [
   {"Name": "Darya", "Age": 19, "AverageMark": 7.8 },
   {"Name":"Polina", "Age": 19, "AverageMark": 7.5},
   {"Name":"Kseniya", "Age": 18, "AverageMark": 3}];   
   
   function StudentsTable(props) {
      let rows = [];
  		let students = props.students;
  		
  		for (let i = 0; i < students.length; i++) {
  			rows.push(<StudentRow student = {students[i]} index = {i} />);
  		}
  		
     	return <table>
             <tr><th>Name</th><th>Age</th><th>AverageMark</th></tr>
             {rows}
            	</table>;
   }
   
   function StudentRow(props) {
  		let student = props.student;
      let index = props.index;

      function studentStyles() {
         return (index % 2 == 0) ? "pink" : "#8B9498";
      }

      function checkAverage() {
          if(student.AverageMark < 4)
            return "red";
      }

  		return <tr style = {{backgroundColor:studentStyles()}} >
  				<td>{student.Name}</td>
  				<td>{student.Age}</td>
  				<td style = {{color:checkAverage()}}>{student.AverageMark}</td>
  			  </tr>;
   }
   
   ReactDOM.render(
        <StudentsTable students = {students} />,
        document.getElementById("app")
    )

~~~

