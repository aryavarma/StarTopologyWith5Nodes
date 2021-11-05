# Star Topology With 5 Nodes (Animation using NS3 and NetAnim)
 
Question :

 Write down a program in NS3 to simulate Star topology with 5 nodes. (A minor change carried out on an existing code) 
 https://www.nsnam.org/doxygen/star-animation_8cc_source.html
 
 # Steps:
 1. Create or copy-paste the following file in the folder ns-allinone-3.33/ns-3.33/scratch. I chose star-topology.cc as file name.
 2. Open the terminal and run the command:(Make sure u open the terminal in the same folder where your star-topology.cc file is)
 
 Command
 
 ./waf --run scratch/star-topology

After that 
Follow the steps shown in the image

![image](https://user-images.githubusercontent.com/74491117/140513831-065d31b6-5b04-4e51-87f6-51fce1f65f83.png)

After NetAnim is started search for *star-anim.xml* file and open it .

![image](https://user-images.githubusercontent.com/74491117/140515011-9cfc3bf3-d243-43b6-8636-420953ac01c8.png)

 # Output:
 
![image](https://user-images.githubusercontent.com/74491117/140513606-24b66233-b06a-4d9c-b8a9-83f84b066933.png)
![image](https://user-images.githubusercontent.com/74491117/140513645-e127ea18-0a40-4168-87c6-d47359acc001.png)
![image](https://user-images.githubusercontent.com/74491117/140513681-cd81d2b3-ef56-4ceb-8355-6b4922f32ea7.png)
![image](https://user-images.githubusercontent.com/74491117/140513719-15824485-0b4d-414a-b4a1-9efe60ea1bd6.png)
![image](https://user-images.githubusercontent.com/74491117/140513761-0aa2cdd2-9e65-429e-a7b3-6e2e0ad8eed4.png)

 # Theory just for reference:
 # Star Topology
  A star topology is the most common network topology and it resembles very similar to a star. In the center of the star topology is a central hub that each node connects to. Because of the
  central hub, star topologies are more reliable than the previous setups and have several advantages. Since each node has its own connection to the central hub, troubleshooting is easy. It limits the impact of a single failure. Additionally, The performance is faster because data doesn’t
  have to go through each node before reaching its destination. If one node fails, the rest of them will still work as normal.
 
 
 # References :
 Updated this code, which was taken from
 https://www.nsnam.org/doxygen/star-animation_8cc_source.html
 
 
 For 5 nodes we have to update *line 57* of the above mentioned code

 uint32_t nSpokes = 5;
 #You can put any number(Number of nodes).
 
