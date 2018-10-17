# show_subgraphs
PROJECT- A GUI based application to display all the subgraphs of a given graph excluding the
stand alone components.

CLASSES USED AND THEIR IMPORTANT MEMBER FUNCTIONS
a) class GraphTheoryProject : This the main class . In this class we create an object of class
InputPage and set it visible.

b) class InputPage :This class extends javax.swing.Jframe. The user enters the graph through
this input page. The important functions in this class are:
1)void showGraph() :
2)void updateGraph(Vertex v) : This function takes a Vertex class object as parameter and
updates the graph whenever a new vertex is added.
3)void updateGraph(Edge e) : This function takes a Edge class object as parameter and
updates the graph whenever a new edge is created.

c) class Edge : This class has two object vertices for an edge. It has getter and setter functions
for both the vertices of an edge.

d) class Vertex : This class contains a data member nodeNo for uniquely identifying a vertex.
It also has a setter function to set a nodeNo to the current vertex object.

e) class Subgraph : This class contains the main algorithm for generating the subgraphs.The
most important function in this class is:
1)ArrayList< ArrayList<Edge> > generateSubgraphs(ArrayList<Edge> list) :This
funciton takes an ArrayList of Edges(user defined Graph) as input parameters and returns an
ArrayList of ArrayList of Edges (List of Subgraphs).

f) class OutputPage :this class extends javax.swing.Jframe.This page mainly displays our
graph graphically.The important member functions in this class are:
1)OutputPage(ArrayList<Vertex> vertexlist, ArrayList< ArrayList<Edge> >
subgraphlist): It is is constructor which initializes all the data members and draws the first
subgraph.The first subgraph is drawn by calling the function drawGraph().
2)void drawGraph() : It is the function that actually draws the graph with GUI.
3)void checkNav() : This function mainly checks the navigation between the list of sub
graphs while displaying them.It mainly enables or disables the “next” and “previous”
buttons according to the situation.

