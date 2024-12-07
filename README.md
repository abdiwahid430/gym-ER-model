+-----------------+      +----------------+      +-------------------+
|   Gymnasium    | 1    |     Member     |    * |      Session      |
+-----------------+      +----------------+      +-------------------+
| Gym_ID (PK)    |<---->| Member_ID (PK) |<---->| Session_ID (PK)   |
| Name           |      | Last Name      |      | Type of Sport     |
| Address        |      | First Name     |      | Schedule          |
| Phone Number   |      | Address        |      | Gym_ID (FK)       |
+-----------------+      | DOB            |      | Max Members (20)  |
                         | Gender         |      +-------------------+
                         +----------------+
  
          *            *                     *            *
   +-------------------+            +--------------------+
   | Session_Enrollment |            |   Session_Coach    |
   +-------------------+            +--------------------+
   | Session_ID (FK)   |            | Session_ID (FK)    |
   | Member_ID (FK)    |            | Coach_ID (FK)      |
   | Enrollment Date   |            +--------------------+
   +-------------------+    
  
                         +-------------------+
                         |      Coach        |
                         +-------------------+
                         | Coach_ID (PK)     |
                         | Last Name         |
                         | First Name        |
                         | Age               |
                         | Specialty         |
                         +-------------------+
