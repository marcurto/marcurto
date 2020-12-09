### Hi, I'm Mar :hugs:

I'm a Frontend developer with a background in Agri-Food Engineering. I started my professional career in the food safety area where I learned how to deal with clients and critical processes on consultant positions. A year ago, I discovered my passion for the world of web development (seriously, I'm in :heart: with programming), especially the fact of being able to transform ideas into code and be able to create products that can be useful and that solve real problems.:earth_africa:



#### How it all started? :thinking:

Some time ago, when I was doing my master's internship, I was asked to create a course for food handlers in Moodle. While I was doing it, I constantly thought: *A Pop-up would be a luxury here!* or *How cool if we could put a drop down here!*. So I did my research and came across HTML and CSS and... voilà!

#### 

#### Covid-19 :mask:

I was working from home and someone said to me: Hey, I've been offered a project, *would you be interested in doing the layout?* Obviously yes (you can check it on www.homebid.es :wink:). And since then, there was no going back. I steeled myself and left my previous job, a bit adrift, but with a clear destination. Let's programming! So thank you so much someone.:sparkles:



#### First of all, I'm an IronHacker :computer:

What I learned? That I had a lot to learn. So I became an IronHacker and spent two months programming like crazy. That allowed me to discover geniuses like React and this made the ideas that remained only ideas to be transformed into something much more reachable. And most importantly, I learned from the best teachers and met wonderful people.

So, who I am now?

```
import React, { Component } from "react";

class Mar extends Component {
	state = {
		technologies: ["React", "JavaScript", "HTML", "CSS", "Node.js", "Express.js"],
		tools: ["Git", "GitHub", "MongoDB", "Heroku", "Postman"],
		interests: ["Frontend Frameworks", "UX/UI", "Music", "World Impact"],
		contact: {
			linkedin: "https://www.linkedin.com/in/marcurto/",
			mail: "mcurtogilabert@gmail.com",
			phone:"653 829 957"
		}
	}

  handleChange = (e) => {
    let { name, value } = e.target;
    this.setState({ [name]: value });
  };

  makeMarHappy = async (e) => {
    e.preventDefault();
    await console.log(`Hi ${e.target.elements.name.value}! Nice to meet you. I'm very exited to know more about ${e.target.elements.project.value} :)`);
    await console.log(`You can contact me by email on ${this.state.contact.mail} or by phone: ${this.state.contact.phone}. Maybe you want to know more about me, so you can check my linkedin on ${this.state.contact.linkedin}`)
  }

  render() {
		return (
            <form onSubmit={this.makeMarHappy}>
              <label htmlFor="name">Your name:</label>
              <input id="name" type="text" name="name" onChange={this.handleChange}/>
              <label htmlFor="project">Your project name:</label>
              <input id="project" type="text" name="project" onChange={this.handleChange}/>
              <input type="submit" value="Contact me!"/>
            </form>
		)
	}

}

export default Mar;
```








