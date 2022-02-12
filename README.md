# RPA-in-Python

![alt text](https://github.com/kiddojazz/RPA-in-Python/blob/main/images/Robot.png)

In this post, we'll cover a few packages for doing robotic process automation with Python and the entire work of Robotics Process Automation in Industry and other business processes.

The world of Science and Technology keeps evolving daily with big organizations turning to robotic process automation to carry out their daily tasks, thereby making employees focus on other tasks that require more human interaction.

There has been a misconception that with the advance of RPA software there would be a loss of jobs and the need for human beings to perform certain types of daily tasks would not be required as the software/bot would be able to do it faster and better.

# What is robotic process automation?
According to Wikipedia, Robotic Process Automation (RPA) is a form of business process automation technology based on metaphorical software robots (bots) or artificial Intelligence.
The RPA software can be said to be a robot or bot that can learn, mimic(copy), and then execute processes based on business processes.

The RPA can also be said to be an application of Technology, governed by Logic and structural input, aimed at recording steps and automating business processes as a required output.

# What are the benefits of RPA?

1. **Cost-Effective:** RPA provides measurable business benefits; such as cost reduction, speed, and greater accuracy.

2. **Accuracy:** It provides organizations with the ability to reduce staffing costs and human error. Robots are reliable and do not show features as fatigues.

3. **Employee Productivity:** With the introduction of RPA in most organizations employees are able to focus on client and customer relationships.

4. **Business Data Security:** A well-designed and managed RPA system help prevent the leak of information which has been a major concern for most big organizations.

5. **Improved Analytics:** Error-free, accurate data from various sources would improve the quality of the analytics process. This in turn helps business managers make better decisions.

6. **Consistency:** RPA is safe and is consistent in performing repeated tasks across multiple boards.

7. **Versatility:** RPA is used across various industries and has the ability to perform multiple tasks. Note any process of automation that is backed up by logical processes and is usually repeated can be automated to save to focus on more important tasks.

8. **Better Support and Management:** Operational processes are improved with the implementation of RPA in the work process. It helps improve operational quality and monitor operational networks across various sessions of an organization.

Now let's do some coding, for this project we would be using the RPA Framework which is an open-source libraries tool. 

## Let's start by installing all necessary Python Package

Let's start

```
!pip install rpa
```

The rpa library is an open-source python package developed by  GitHub: [tebelorg](https://github.com/tebelorg/RPA-Python)

```
import rpa as r
```

## Applications
- **Site Navigation**
RPA has the ability to navigate through the web and get specific information. The process saves time and stress.
Now we can initialize the rpa to open a new browser window. The browser used by the rpa package is Google Chrome.

```
r.init()
```

After we initiate the rpa, our aim is to navigate through a particular blog post

```
r.url("https://www.urbizedge.com/custom-shape-map-in-power-bi/")
#This is aimed at navigating to a website by using the rpa bot
```

After you achieve the navigating it is only proper you close the browser.
```
r.close()
```

![alt text](https://github.com/kiddojazz/RPA-in-Python/blob/main/images/1_whqu1h1ZuDYDuJAxWf_F_A.gif)

- **Automatically Download Data from a site**

Start by initializing the rpa library

```
r.init()
```

The data that would be used for this stage is the breast cancer dataset that is provided by UCI database.


```
r.url("https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer/")
```

This would automatically open your Chrome browser and navigate to the UCI website to download the breast cancer dataset.

![alt text](https://github.com/kiddojazz/RPA-in-Python/blob/main/images/1_suVb1vHRVX-SDeFS1tmDhA.png)

After getten to the site you would have to click on the download button which can be done by running the click line of code. This would help in downloading the code.

```
r.click("breast-cancer.data")
```

![alt text](https://github.com/kiddojazz/RPA-in-Python/blob/main/images/1_vA_A5J_ZwKsb6oEUKYojEA.png)

- **Web Automation**

Web automation is the concept of letting software robots perform pre-defined actions, tasks, and processes on a web browser or web application.

Start by activating the RPA library.

```
r.init()
r.url('https://www.google.com')
r.type('//*[@name="q"]', 'USA[enter]')
print(r.read('result-stats'))
r.snap('page', 'USA.png')
```

What is actually happening here is firstly, your chrome browser opens when you initialize the code.
It then navigate to google were is search for a specific key word which we have inserted called USA.
Lastly it then saves the search location as a png format.

Below is an explanation of the entire process of what actually happened.

![alt text](https://github.com/kiddojazz/RPA-in-Python/blob/main/images/1_NYu8AhHZdcLr7hDOhRn0Pw.gif)

At the end of each line of code you have to close the rpa system. This way saves energy of your device.

```
r.close()
#This is meant to close the RPA system running of Chrome.
```

**Note:** That if there are two hyperlinks with the same label "here" and we execute rpa.click("breast-cancer.data"), then the robot will click on the first one it finds.

## Conclusion
In the world of advancement of science and technology, rise in AR, AI,NFT, BlockChain and other cryptocurrency, you don't have to be scared of technology rather you have to embrance the rise of it. RPA would grow to have more application especially in the healthcare and finance sector. This would help save time which are usually lost during document sorting.
