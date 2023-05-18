-- GraphDB is a compliant graph database that supports RDF and SPARQL specifications. It uses open APIs based on the RDF4J (formerly Sesame) project and allows for the efficient publication of linked data on the web. The GraphDB Workbench is a tool used for searching, exploring, and managing semantic repositories in GraphDB.

-- Apache Jena, on the other hand, is an open-source Java framework used for building applications in the Semantic Web and Linked Data domain. It provides powerful capabilities for creating ontologies, querying data, and adding constraints using SHACL.

-- In the context of this lab, Apache Jena API was used to create the TBOX (Terminology Box) and ABOX (Assertion Box) for publications' data. The TBOX represents the metadata or schema of the knowledge graph, defining atomic concepts (Classes) and their relationships (Properties). The ABOX, on the other hand, represents the data instances and their relationships. By combining the TBOX and ABOX, we create an ontology that enables various possibilities for querying and analyzing the data.

-- The dataset used in this lab is generated from the DBLP data in XML format and converted to CSV format. To ensure correct topology in the knowledge graph, the data needs to be preprocessed. A Python script is provided in the lab, located in the "preprocess_data" folder, to perform the necessary preprocessing. Running the script will generate an "instance_data.csv" file.

-- To generate the TBOX, the preprocessed data is obtained from the saved grafo and the "tbox.owl" file is created. The generated CSV file should be placed in the "csv" directory within the "data" folder.

-- To generate the ABOX, you need to execute the main Java class named "App." Running this class will generate and save the ABOX in the form of an "Abox.nt" file.

-- After completing the above steps, you should have the following files in the "data" directory: "tbox.owl," "Abox.nt," and "csv/instance_data.csv." These files can be loaded into GraphDB, where you can start querying and exploring the data.

-- In summary, the lab involves using GraphDB and Apache Jena to create a knowledge graph from publications' data. The data is preprocessed, the TBOX is generated to define the schema, and the ABOX is generated to represent the data instances. Finally, the generated files are loaded into GraphDB for further analysis.
