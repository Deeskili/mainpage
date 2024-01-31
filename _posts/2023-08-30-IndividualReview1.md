---
toc: false
comments: true
layout: post
title: Individual Review 
description: Sum of TRI 1 
type: tangibles
courses: { compsci: {week: 11} }
---


### Individual Code

#### Journey Through API Development

**Initial Exploration with CSV**
- **Objective:** To create a manageable and editable database for recipes.
- **Approach:** Initially experimented with a CSV file as a database.
- **Outcome:** Realized that while CSV files are good for static data, they fall short when dynamic and editable data are necessary.

**Transition to SQLite**
- **Objective:** Transition towards a more dynamic database.
- **Approach:** Adopted SQLite for a more structured and easily manageable database.
- **Challenges:** Faced issues with database initialization and connecting it with Flask.
- **Outcome:** Successfully integrated SQLite with Flask, resulting in a more robust and dynamic database.

- **Frontend and Backend Contributions:** Apart from backend database transitions, contributions were also made towards enhancing the frontend's visual appeal. Assistance was provided in creating a seamless and effective linkage between various frontend components. Collaborated with Saathvik, providing support in backend API development, ensuring a harmonized alignment between backend functionalities and frontend expectations.

**Favorite Code Snippets**


- **Command-Line Execution:** The ability to manage the application through the command line was crucial. These command lines were among the favorites because they allowed for efficient management, navigation, and execution of the Flask application.

```bash
cd /Users/caydenshi/vscode/backendrocketmain  # Navigate to your project directory
export FLASK_APP=api/editedrecipesqlite.py  # Point to your application file
export FLASK_ENV=development  # Set the environment to development
flask run  # Run your Flask application
```


```python
class Recipe(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    title = db.Column(db.String(128), unique=True, nullable=False)
    ingredients = db.Column(db.String(256), nullable=False)
    instructions = db.Column(db.String(256), nullable=True)
    
    def serialize(self):
        return {
            "id": self.id,
            "title": self.title,
            "ingredients": self.ingredients,
            "instructions": self.instructions
        }
```

### GitHub Analytics Review

**Key Commits**
- Initial implementation with CSV.
- Transition to SQLite for a more dynamic database.
- Integration of SQLite with Flask.

**Challenges**
- Issues faced with Flask and SQLite integration.
- Debugging error messages and finding solutions to tackle them.



### Individual Blog

```plaintext
Procedure move_robot(start, turn, end)
    ROTATE_LEFT()        # Rotating the robot to the left
    MOVE_FORWARD()       # Move the robot forward
    ROTATE_RIGHT()       # Rotating the robot to the right
    MOVE_FORWARD()       # Move the robot forward
    MOVE_FORWARD()       # Repeat the forward movement
    ROTATE_LEFT()        # Rotating the robot to the left
    MOVE_FORWARD()       # Move the robot forward
    MOVE_FORWARD()       # Repeat the forward movement
End Procedure
```
[click here to view question image](https://media.discordapp.net/attachments/1143438030749847604/1165903186473783317/image.png?ex=65488af5&is=653615f5&hm=349a4cfef60546b6f85e59a2448ac85ed4fd0181d63f70456904909e46401d74&)


#### Trimester 1 Reflections

**Memories and Learnings**
- **Teamwork:** Learning the value of collaboration and leveraging each team member's strengths.
- **Persistence:** Faced several challenges but didn’t give up. Persistent effort led to the resolution of problems.
- **Adaptability:** Transition from a CSV to SQLite database for better functionality.
- **Assisting Others:** Actively contributed by assisting various groups including Ronit’s, Ian’s, Cindy’s, Austin’s, and Will’s groups, sharing knowledge and helping troubleshoot issues.

**Positive Accomplishments**
- Successful implementation of a more dynamic, robust, and manageable database using SQLite.
- Learning and applying new tools and technologies to improve the functionality of our project.

**Opportunities for Growth and Future Learning**
- Looking forward to enhancing my debugging skills.
- Keen on exploring more advanced database options and improving the overall structure and functionality of our application.
- Eager to delve deeper into backend technologies to make our application more sophisticated and user-friendly.
