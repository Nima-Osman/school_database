# mySQL code for the building of a school Database Management System

###Individual project code####
CREATE DATABASE individual_project;
USE individual_project;

#create required tables:

CREATE TABLE Students (
    StudentID INT PRIMARY KEY,
    FirstName VARCHAR(50),
    LastName VARCHAR(50),
    BirthDate DATE
);


CREATE TABLE Teachers (
    TeacherID INT PRIMARY KEY,
    FirstName VARCHAR(50),
    LastName VARCHAR(50),
    HireDate DATE
);


CREATE TABLE Subjects (
    SubjectID INT PRIMARY KEY,
    SubjectName VARCHAR(100)
);


CREATE TABLE Classrooms (
    ClassroomID INT PRIMARY KEY,
    RoomNumber VARCHAR(10),
    Capacity INT
);


CREATE TABLE Classes (
    ClassID INT PRIMARY KEY,
    ClassName VARCHAR(100),
    TeacherID INT,
    SubjectID INT,
    ClassroomID INT,
    CONSTRAINT FK_Classes_Teachers FOREIGN KEY (TeacherID) REFERENCES Teachers(TeacherID),
    CONSTRAINT FK_Classes_Subjects FOREIGN KEY (SubjectID) REFERENCES Subjects(SubjectID),
    CONSTRAINT FK_Classes_Classrooms FOREIGN KEY (ClassroomID) REFERENCES Classrooms(ClassroomID)
);


CREATE TABLE Enrollments (
    EnrollmentID INT PRIMARY KEY,
    StudentID INT,
    ClassID INT,
    EnrollmentDate DATE,
    CONSTRAINT FK_Enrollments_Students FOREIGN KEY (StudentID) REFERENCES Students(StudentID),
    CONSTRAINT FK_Enrollments_Classes FOREIGN KEY (ClassID) REFERENCES Classes(ClassID)
);


CREATE TABLE Grades (
    EnrollmentID INT PRIMARY KEY,
    Grade CHAR(2),
    CONSTRAINT FK_Grades_Enrollments FOREIGN KEY (EnrollmentID) REFERENCES Enrollments(EnrollmentID)
);


CREATE TABLE Attendance (
    AttendanceID INT PRIMARY KEY,
    StudentID INT,
    AttendanceDate DATE,
    Status VARCHAR(20),
    CONSTRAINT FK_Attendance_Students FOREIGN KEY (StudentID) REFERENCES Students(StudentID)
);


CREATE TABLE Parents (
    ParentID INT PRIMARY KEY,
    FirstName VARCHAR(50),
    LastName VARCHAR(50),
    PhoneNumber VARCHAR(15),
    Email VARCHAR(100)
);

CREATE TABLE StudentParents (
    StudentID INT,
    ParentID INT,
    PRIMARY KEY (StudentID, ParentID),
    CONSTRAINT FK_StudentParents_Students FOREIGN KEY (StudentID) REFERENCES Students(StudentID),
    CONSTRAINT FK_StudentParents_Parents FOREIGN KEY (ParentID) REFERENCES Parents(ParentID)
);


CREATE TABLE Exams (
    ExamID INT PRIMARY KEY,
    ExamName VARCHAR(100),
    ExamDate DATE
);

CREATE TABLE ExamResults (
    ExamResultID INT PRIMARY KEY,
    StudentID INT,
    ExamID INT,
    Score DECIMAL(5, 2),
    CONSTRAINT FK_ExamResults_Students FOREIGN KEY (StudentID) REFERENCES Students(StudentID),
    CONSTRAINT FK_ExamResults_Exams FOREIGN KEY (ExamID) REFERENCES Exams(ExamID)
);