# Ex09 Event Registration Web Application
## Date:19/12/2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
import React from "react";
import screenshot202512191351591 from "./screenshot-2025-12-19-135159-1.png";

export const AndroidCompact = (): JSX.Element => {
  return (
    <div className="bg-[#e69cd6] w-full min-w-[396px] min-h-[640px] flex flex-col">
      <img
        className="ml-0.5 w-[393px] h-[220px] aspect-[1.79] object-cover"
        alt="Screenshot"
        src={screenshot202512191351591}
      />

      <div className="ml-[95px] w-[200px] h-[58px] mt-[18px] [font-family:'Irish_Grover-Regular',Helvetica] font-normal text-black text-5xl tracking-[0] leading-[normal]">
        TANGLED
      </div>

      <div className="ml-[29px] w-[335px] h-[58px] mt-[27px] [font-family:'Irish_Grover-Regular',Helvetica] font-normal text-black text-5xl tracking-[0] leading-[normal]">
        REGISTER NOW
      </div>
    </div>
  );
};

import React from "react";

export const AndroidCompact = (): JSX.Element => {
  const formFields = [
    { id: "name", label: "NAME:", type: "text", name: "name" },
    { id: "class", label: "CLASS:", type: "text", name: "class" },
    { id: "event", label: "EVENT:", type: "text", name: "event" },
    { id: "contact", label: "CONTACT:", type: "text", name: "contact" },
  ];

  const handleSubmit = (e: React.FormEvent<HTMLFormElement>) => {
    e.preventDefault();
    const formData = new FormData(e.currentTarget);
    const data = Object.fromEntries(formData.entries());
    console.log("Form submitted:", data);
  };

  return (
    <div className="bg-[#db9bf8] w-full min-w-[360px] min-h-[640px] flex">
      <form
        onSubmit={handleSubmit}
        className="mt-[50px] w-[186px] h-[270px] ml-[33px]"
        aria-label="Contact information form"
      >
        <div className="[font-family:'Jersey_20-Regular',Helvetica] font-normal text-black text-5xl tracking-[0] leading-[normal]">
          {formFields.map((field, index) => (
            <div key={field.id} className="flex flex-col">
              <label
                htmlFor={field.id}
                className="[font-family:'Jersey_20-Regular',Helvetica] font-normal text-black text-5xl tracking-[0] leading-[normal]"
              >
                {field.label}
              </label>
              {index < formFields.length - 1 && <br />}
            </div>
          ))}
        </div>
      </form>
    </div>
  );
};

import React from "react";

export const AndroidCompact = (): JSX.Element => {
  return (
    <main className="bg-[#e69cd6] w-full min-w-[360px] min-h-[640px] flex">
      <h1 className="mt-[226px] w-[305px] h-[78px] ml-[27px] [font-family:'Irish_Grover-Regular',Helvetica] font-normal text-black text-[32px] tracking-[0] leading-[normal]">
        THANKS FOR
        <br />
        YOUR REGISTRATION
      </h1>
    </main>
  );
};
```


## OUTPUT:
![alt text](<Screenshot 2025-12-24 111250-1.png>)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
