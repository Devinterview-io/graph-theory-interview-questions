<div data-v-5e9078c0=""><h1 data-v-5e9078c0="">
      Top 19 Graph Theory interview
      questions and answers in 2021.
    </h1> <p data-v-5e9078c0="" align="center"><a data-v-5e9078c0="" href="https://devinterview.io/"><img data-v-5e9078c0="" src="https://source.unsplash.com/collection/52661698/700x350"></a></p> <p data-v-5e9078c0="">
      You can check all
      19
      Graph Theory interview questions here 👉
      https://devinterview.io/data/graphTheory-interview-questions
    </p> <br data-v-5e9078c0=""> <div data-v-5e9078c0="" class="unit"><div><h2>🔹 1. What is a Graph?</h2></div> <div><h3>Answer:</h3> <div class="answer"><div><div><div class="AnswerBody"><p>A <strong>graph</strong> is a common data structure that consists of a finite set of <strong>nodes</strong> (or <strong>vertices</strong>) and a set of <strong>edges</strong> connecting them. A pair <code>(x,y)</code> is referred to as an edge, which communicates that the <strong>x vertex</strong> connects to the <strong>y vertex</strong>.</p><p>Graphs are used to solve real-life problems that involve representation of the problem space as a <strong>network</strong>. Examples of networks include telephone networks, circuit networks, social networks (like LinkedIn, Facebook etc.).</p><p></p><div><div><div><div></div></div></div></div><p></p></div></div><div class="row my-2"><div><span><i>Source:</i>&nbsp;<span><a href="https://www.educative.io/edpresso/what-is-a-graph-data-structure" rel="noreferrer" target="_blank" title="What is a Graph? Interview Questions Source To Answer">www.educative.io</a></span></span>&nbsp; &nbsp;</div></div></div></div></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 2. What's the difference between the data structure Tree and Graph?</h2></div> <div><h3>Answer:</h3> <div class="answer"><div><div><div class="AnswerBody"><p><strong>Graph:</strong></p><ul><li>Consists of a set of vertices (or nodes) and a set of edges connecting some or all of them</li><li>Any edge can connect any two vertices that aren't already connected by an identical edge (in the same direction, in the case of a directed graph)</li><li>Doesn't have to be connected (the edges don't have to connect all vertices together): a single graph can consist of a few disconnected sets of vertices</li><li>Could be directed or undirected (which would apply to all edges in the graph)</li></ul><p><strong>Tree:</strong></p><ul><li>A type of graph (fit with in the category of Directed Acyclic Graphs (or a DAG))</li><li>Vertices are more commonly called "nodes"</li><li>Edges are directed and represent an "is child of" (or "is parent of") relationship</li><li>Each node (except the root node) has exactly one parent (and zero or more children)</li><li>Has exactly one "root" node (if the tree has at least one node), which is a node without a parent</li><li>Has to be connected</li><li>Is acyclic, meaning it has no cycles: "a cycle is a path <a href="">AKA sequence</a> of edges and vertices wherein a vertex is reachable from itself"</li><li>Trees aren't a recursive data structure</li></ul><p></p><div><div><div><div></div></div></div></div><p></p></div></div><div class="row my-2"><div><span><i>Source:</i>&nbsp;<span><a href="https://stackoverflow.com/questions/7423401/whats-the-difference-between-the-data-structure-tree-and-graph" rel="noreferrer" target="_blank" title="What's the difference between the data structure Tree and Graph? Interview Questions Source To Answer">stackoverflow.com</a></span></span>&nbsp; &nbsp;</div></div></div></div></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 3. List some ways of representing Graphs</h2></div> <div><h3>Answer:</h3> <div class="answer"><div><div><div class="AnswerBody"><ul><li><strong>Edge Lists</strong>. We have an array of two vertex numbers, or an array of objects containing the vertex numbers of the vertices that the edges are incident on (plus weight). Edge lists are simple, but if we want to find whether the graph contains a particular edge, we have to search through the edge list. If the edges appear in the edge list in no particular order, that's a linear search through <code>E</code> edges.</li></ul><pre><code><span class="token cBase">[</span> <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span><span class="token cNum">1</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span><span class="token cNum">6</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span><span class="token cNum">8</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">1</span><span class="token cBase">,</span><span class="token cNum">4</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">1</span><span class="token cBase">,</span><span class="token cNum">6</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">1</span><span class="token cBase">,</span><span class="token cNum">9</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">2</span><span class="token cBase">,</span><span class="token cNum">4</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">2</span><span class="token cBase">,</span><span class="token cNum">6</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">3</span><span class="token cBase">,</span><span class="token cNum">4</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">3</span><span class="token cBase">,</span><span class="token cNum">5</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">3</span><span class="token cBase">,</span><span class="token cNum">8</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">4</span><span class="token cBase">,</span><span class="token cNum">5</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">4</span><span class="token cBase">,</span><span class="token cNum">9</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">7</span><span class="token cBase">,</span><span class="token cNum">8</span><span class="token cBase">]</span><span class="token cBase">,</span> <span class="token cBase">[</span><span class="token cNum">7</span><span class="token cBase">,</span><span class="token cNum">9</span><span class="token cBase">]</span> <span class="token cBase">]</span></code></pre><ul><li><strong>Adjacency Matrices.</strong> With an adjacency matrix, we can find out whether an edge is present in constant time, by just looking up the corresponding entry in the matrix - we can query whether edge <code>(i, j)</code> is in the graph by looking at <code>graph[i][j]</code> value. For a sparse graph, the adjacency matrix is mostly <code>0s</code>, and we use lots of space to represent only a few edges. For an undirected graph, the adjacency matrix is <em>symmetric</em>.</li></ul><pre><code><span class="token cBase">[</span> <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">0</span><span class="token cBase">]</span> <span class="token cBase">]</span></code></pre><ul><li><strong>Adjacency Lists</strong>. For each vertex <code>i</code>, store an array of the vertices adjacent to it (or array of <em>tuples</em> for weighted graph). To find out whether an edge <code>(i,j)</code> is present in the graph, we go to <code>i's</code> adjacency list in constant time and then look for <code>j</code> in <code>i's</code> adjacency list.</li></ul><pre><code><span class="token cBase">[</span> <span class="token cBase">[</span><span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">6</span><span class="token cBase">,</span> <span class="token cNum">8</span><span class="token cBase">]</span><span class="token cBase">,</span>   <span class="token cComment">// 0</span>
  <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">4</span><span class="token cBase">,</span> <span class="token cNum">6</span><span class="token cBase">,</span> <span class="token cNum">9</span><span class="token cBase">]</span><span class="token cBase">,</span>  <span class="token cComment">// 1</span>
  <span class="token cBase">[</span><span class="token cNum">4</span><span class="token cBase">,</span> <span class="token cNum">6</span><span class="token cBase">]</span><span class="token cBase">,</span>        <span class="token cComment">// 2</span>
  <span class="token cBase">[</span><span class="token cNum">4</span><span class="token cBase">,</span> <span class="token cNum">5</span><span class="token cBase">,</span> <span class="token cNum">8</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">2</span><span class="token cBase">,</span> <span class="token cNum">3</span><span class="token cBase">,</span> <span class="token cNum">5</span><span class="token cBase">,</span> <span class="token cNum">9</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">3</span><span class="token cBase">,</span> <span class="token cNum">4</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">2</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">8</span><span class="token cBase">,</span> <span class="token cNum">9</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">0</span><span class="token cBase">,</span> <span class="token cNum">3</span><span class="token cBase">,</span> <span class="token cNum">7</span><span class="token cBase">]</span><span class="token cBase">,</span>
  <span class="token cBase">[</span><span class="token cNum">1</span><span class="token cBase">,</span> <span class="token cNum">4</span><span class="token cBase">,</span> <span class="token cNum">7</span><span class="token cBase">]</span> <span class="token cBase">]</span>    <span class="token cComment">// N</span></code></pre><p></p><div><div><div><div></div></div></div></div><p></p></div></div><div class="row my-2"><div><span><i>Source:</i>&nbsp;<span><a href="https://www.khanacademy.org/computing/computer-science/algorithms/graph-representation/a/representing-graphs" rel="noreferrer" target="_blank" title="List some ways of representing Graphs Interview Questions Source To Answer">www.khanacademy.org</a></span></span>&nbsp; &nbsp;</div></div></div></div></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 4. Explain the BSF (Breadth First Search) traversing method</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 5. Name some common types and categories of Graphs</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 6. What is difference between BFS and Dijkstra's algorithms when looking for shortest path?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 7. Explain what is DFS (Depth First Search) algorithm for a Graph and how does it work?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 8. What are some applications of Graphs?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 9. Provide some practical examples of using Depth-First Search (DFS) vs Breadth-First Search (BFS)?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 10. Explain what is A* Search?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 11. Compare Adjacency Lists or Adjacency Matrices for Graphs representation</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 12. What are key differences between BFS and DFS?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 13. What is Bipartite Graph? How to detect one?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 14. Explain what is heuristic cost function in A* Search and how to calculate one?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 15. Why does a Breadth First Search (BFS) use more memory than Depth First Search (DFS)?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/data/graphTheory-interview-questions">all 19 answers</a></div> <br><br></div> <div data-v-5e9078c0="" class="end"></div> <br data-v-5e9078c0="">
    Thanks 🙌 for reading and good luck on your next tech interview!
    <br data-v-5e9078c0="">
    Explore 3800+ dev interview question here 👉
    <a data-v-5e9078c0="" href="https://devinterview.io/">Devinterview.io</a></div>
