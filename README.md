---


---

<h1 id="map-it-robo">Map-it-ROBO</h1>
<p><strong>Building a map</strong> using a dataset consisting of odometry, IMU,<br>
laser range finder, SONAR and video recordings from cameras by a wheeled robot. The project uses <strong>GMapping</strong> a <strong>Simultaneous localization and Mapping (SLAM)</strong> algorithm.</p>
<h2 id="the-dataset">The Dataset</h2>
<p>I have used <a href="http://www.rawseeds.org/rs/datasets/view//6">Raw Seeds</a> dataset for SLAM implementation. The dataset consists of odometry, IMU,laser range finder, SONAR and video recordings from cameras. This data is collected by driving a wheeled robot equipped with these sensors through the library at <a href="http://www.rawseeds.org/rs/capture_sessions/view/5"><em><strong>Universita’ Degli Studi Di Milano Bicocca</strong></em></a>.</p>
<h2 id="implementation">Implementation</h2>
<ul>
<li><strong>Ubuntu Linux</strong></li>
<li><strong>ROS</strong>: The Robot Operating System (ROS) is a exible framework for writing robot software. It is a collection of tools, libraries, and conventions that aim to simplify the task of creating complex and robust robot behavior across a wide variety of robotic platforms.</li>
<li><strong>ROS Melodic Morenia</strong>: ROS Melodic Morenia is the twelfth ROS distribution release.</li>
</ul>
<h2 id="installation">Installation</h2>
<p>Setup your sources.list</p>
<pre><code>sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc)main"&gt; /etc/apt/sources.list.d/ros􀀀latest.list'
</code></pre>
<p>Set up your keys</p>
<pre><code>sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-keyC1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
</code></pre>
<p>Installation</p>
<p><code>sudo apt update</code><br>
<code>sudo apt install ros-melodic-desktop-full</code><br>
<code>apt search ros-melodic</code></p>
<p>Initialize rosdep</p>
<p><code>sudo rosdep init</code><br>
<code>rosdep update</code></p>
<p>Environment setup</p>
<p><code>echo "source /opt /ros/melodic/setup.bash" &gt;&gt; :/.bashrc</code><br>
<code>source :/.bashrc</code><br>
<code>source /opt/ros/melodic/setup.bas</code></p>
<p>Dependencies for building packages</p>
<p><code>sudo apt install python-rosinstall python-rosinstall-generator python-wstool build-essential</code></p>
<p>Check Installation</p>
<p><code>rosversion ros</code></p>
<h2 id="result">RESULT</h2>
<h3 id="robot-path-to-be-mapped"><strong>Robot Path to be Mapped</strong></h3>
<p><img src="https://lh3.googleusercontent.com/proxy/FjEO0QHG8vGk70XtJolNqTV8vGg5W0H-Q0q3YsNhHuRasTTRueEramXJYaGIG_p7B_SBvq_r_ZgLqzLsDMgZl_TjluyYHhs5Peo9IZoQvapo86pN1I7XCPVsVaExDC64hqmLPrq_" alt="**Robot Path to be Mapped**"></p>
<h3 id="map-generated"><strong>Map Generated</strong></h3>

