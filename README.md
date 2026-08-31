# KLH-CSE DSA SHORT PROJECT

## Student Lab Allocation

**Academic Year:** 2026-27  
**Team ID:** 5  
**Department:** KLH-CSE  
**Course:** Data Structures and Algorithms (DSA)

---

## 1. Problem Definition

Student Lab Allocation is a scheduling problem in which a set of students must be assigned to available computer laboratories and time slots.

Manual allocation becomes difficult when the number of students, laboratories, and time slots increases. Each laboratory has a limited capacity, and students must be assigned without exceeding that capacity or creating scheduling conflicts.

The problem is to design a DSA-based system that takes student, laboratory, capacity, and time-slot information as input and generates a valid student-to-lab-to-slot allocation.

---

## 2. Objectives

The main objectives of the Student Lab Allocation project are:

1. **Efficient Data Organization**  
   Store and organize student, laboratory, capacity, and time-slot information using suitable data structures.

2. **Systematic Allocation**  
   Develop an algorithm that processes students in an organized manner and assigns them to feasible laboratory slots.

3. **Capacity Management**  
   Ensure that the number of students assigned to a laboratory does not exceed its available capacity.

4. **Conflict Reduction**  
   Check for scheduling conflicts before confirming an allocation.

5. **Clear Output**  
   Generate an understandable allocation showing which student is assigned to which laboratory and time slot.

---

## 3. Literature Grounding

The Student Lab Allocation problem is related to established scheduling and resource-allocation approaches.

### 3.1 First-Come, First-Served (FCFS)

FCFS processes students according to their order of arrival. It can be implemented using a queue, following the FIFO (First In, First Out) principle.

**Relevance to the Project:**  
A queue can be used to maintain an organized order in which students are considered for allocation.

### 3.2 Greedy Scheduling

Greedy scheduling makes the best currently feasible choice at each step. In this project, a feasible laboratory and time slot can be selected for each student after checking availability and capacity.

**Relevance to the Project:**  
A greedy strategy provides a simple and efficient approach for constructing a valid allocation.

### 3.3 Graph-Based Scheduling

Scheduling conflicts can be represented using a graph. Students or groups that should not share the same time slot can be represented as connected vertices.

**Relevance to the Project:**  
Graph-based methods, such as graph coloring, can be used in future versions to handle more complex scheduling conflicts.

### 3.4 Data Structures in Scheduling

Scheduling problems commonly require efficient organization and processing of data. Arrays or lists can store student and laboratory information, while queues can organize processing order.

**Relevance to the Project:**  
The project applies these DSA concepts to a practical laboratory allocation problem rather than relying on manual scheduling.

---

## 4. Proposed DSA Approach

The proposed system follows these steps:

1. Read student, laboratory, capacity, and time-slot information.
2. Store the information using appropriate data structures.
3. Sort or queue the students for processing.
4. Select an available laboratory and time slot.
5. Check laboratory capacity.
6. Check for scheduling conflicts.
7. If the allocation is valid, assign the student.
8. If the allocation is invalid, try the next feasible laboratory or slot.
9. Continue until all students have been processed.
10. Display the final allocation.

### Basic Flow

START
  |
  v
Input Student, Lab & Slot Data
  |
  v
Sort / Queue Students
  |
  v
Select Available Lab & Slot
  |
  v
Capacity / Conflict Check
  |
  +------ Invalid ------> Try Next Feasible Lab / Slot
  |
 Valid
  |
  v
Assign Student
  |
  v
More Students?
  |
  +---- Yes ----> Process Next Student
  |
  No
  |
  v
END

---

## 5. Expected Output

The system should generate a final allocation similar to:

| Student | Laboratory | Time Slot |
|---|---|---|
| S01 | Lab-1 | 09:00–10:00 |
| S02 | Lab-1 | 09:00–10:00 |
| S03 | Lab-2 | 09:00–10:00 |
| S04 | Lab-2 | 10:00–11:00 |
| S05 | Lab-1 | 10:00–11:00 |

The allocation should respect laboratory capacity and the scheduling constraints defined for the system.

---

## 6. DSA Concepts Applied

- **Arrays / Lists** — Used to store student, laboratory, and slot information.
- **Queue** — Used to process students in an organized FIFO order.
- **Sorting** — Used to establish a consistent processing order.
- **Greedy Algorithm** — Used to select a currently feasible laboratory and slot.
- **Constraint Checking** — Used to validate laboratory capacity and scheduling conditions.

---

## 7. Conclusion

Student Lab Allocation applies Data Structures and Algorithms to a practical scheduling problem. The system organizes student and laboratory information, processes students systematically, checks capacity and scheduling constraints, and generates a clear allocation.

The project demonstrates how fundamental DSA concepts such as queues, lists, sorting, greedy strategies, and constraint checking can be combined to solve a real-world resource-allocation problem.
