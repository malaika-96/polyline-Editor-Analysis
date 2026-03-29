Phase 2 – Analysis (Polyline Editor Application)

Student: Malaika
Seat No.: B23110006063
Human Computer Interaction And Computer Graphics
Course Code: CS-555
Course Instructor's Name: Dr. Humera Tariq

1. Introduction to Analysis Phase:
The analysis phase focuses on understanding:

What the user needs
How the system will behave
What kind of data will be used
How interaction will take place

In this phase, we break down the system into smaller parts so that the design becomes easier and more effective.

2. Task Analysis:
Task analysis identifies all the activities a user performs while using the system.

Main Tasks:
Press ‘b’ to start a new polyline
Click on screen to add points (vertices)
Select a point near cursor
Drag a point to move it (‘m’ key)
Delete a point (‘d’ key)
Refresh drawing (‘r’ key)
Exit application (‘q’ key)

Task Flow Diagram:
Start
  ↓
Press 'b'
  ↓
Click to add points
  ↓
Edit Options:
   → Move (m)
   → Delete (d)
  ↓
Refresh (r)
  ↓
Quit (q)

3. User Analysis:
   
Target Users:
Students learning graphics
Beginners in drawing tools
Designers (basic level)

User Characteristics:
Basic computer knowledge
Familiar with mouse + keyboard
Prefer simple and responsive systems

User Expectations:
Easy to learn
Fast response
Clear visual feedback
No complex steps

5. Data Analysis:
The system needs to store and manage polylines efficiently.

Data Elements:
Polyline = collection of points
Each point = (x, y coordinates)

Structure:
Maximum 100 polylines
Each polyline contains multiple vertices

Data Structure (Recommended):
Array of polylines
Each polyline = list of points

Diagram:
Polylines Array
 ├── Polyline 1 → (x1,y1), (x2,y2), (x3,y3)
 ├── Polyline 2 → (x1,y1), (x2,y2)
 ├── Polyline 3 → (x1,y1), (x2,y2), (x3,y3), (x4,y4)

 5. Functional Analysis:
    
a) Begin (‘b’):
Creates a new polyline
Stored in next available slot

b) Delete (‘d’):
Find nearest vertex
Remove that point
Join previous and next vertices

c) Move (‘m’):
Select nearest vertex
Drag to new location
Update connected lines

d) Refresh (‘r’):
Clear screen
Redraw all polylines

e) Quit (‘q’):
Exit program

6. Interaction Analysis:
   
Input Methods:

Mouse:
Click → add/select point
Drag → move point

Keyboard:
b, d, m, r, q

Output:
Lines drawn on screen
Real-time updates

7. Interaction Diagram:

   User Actions → System Processing → Output

Mouse Click → Add Point → Line Drawn
Mouse Drag  → Move Point → Updated Line
Key Press   → Execute Action → Screen Update

8. Constraints: 
Maximum 100 polylines
Real-time performance required
Accurate selection of nearest point
Smooth dragging without delay

9. Challenges and Issues:
Finding closest vertex quickly
Handling overlapping points
Avoiding errors when deleting edge points
Keeping system fast during redraw
Managing large number of points

10. Possible Improvements:
Undo / Redo feature
Save and Load file option
Insert point between two vertices
Color selection for polylines
3D polyline editing (advanced feature)

11. Example Scenario:
User presses ‘b’ → new polyline starts
User clicks multiple times → shape is formed
User presses ‘m’ → selects a point and drags it
Shape updates automatically
User presses ‘d’ → deletes a point
Lines reconnect
User presses ‘r’ → screen refreshes
User presses ‘q’ → program exits

12. Summary:
    
In this analysis phase, we studied:
User tasks and behavior
Data structures
System functions
Interaction methods

This analysis helps in creating a system that is:
Easy to use
Efficient
Interactive
User-friendly
