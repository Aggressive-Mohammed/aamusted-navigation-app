# Front-End
Our website was produced using plain HTML5/CSS3/JS. No framework (such as ReactJS, Vue, Angular), design website, or substantial DOM manipulation libraries were used to implement the front-end. The full-screen map was implemented using LeafletJS, a JS library for interactive maps. LeafletJS was used as it is a common tool used by developers to implement maps similiar to the map that we implemented on our own site. The paths are displayed by adding a GeoJSON layer (generated in the back-end) to this map based on a request to the back-end server module. Our weather data comes from Open Weather Map's API services, providing real-time data for anywhere in the world. The logo containging the Husky dog and location marker was designed and customized for this project by our team "in house" (something that the entire team is very proud of). On the front-end a big focus for our team was not just coming up with a finished product but putting ourselves in the shoes of the user and thinking what features or components matter most deeply to them. With this vision in mind our front-end design team tested our site with multiple users and used analytics to understand which parts of our site users responded with most.

# Back-End 
The back-end was implemented by using a parser module to parse through files containing lines that translated to node and edge values. This was done in order to facilitate the use of a path-finding algorithm that attempted to find the least-cost path based on a larger distance as the cost. This made it easier to efficently "scrape" through a map and create nodes (only using a text file) with the use of additionaly tools to mantain accuracy as well as a team-wide standardized style for node creation. The back-end was primarily implemented with java in an attempt to facilitate the most direct application of course material as possible. The desision module that implement our path-finding algorithm served as the focal point of our back-end and returned all the information needed for the path through a call to the get decision method. This was faciliated through the use of a comprehensive server module, which is hosted via Azure Functions, in order to allow communication with the front-end of our web application.