<!-- Microsoft Xaml Controls Features Specification Template -->

<!-- Title / Name of Feature -->
# Progress Ring Control

<!-- Brief summary of feature proposal --> 
Update Progress Ring to follow Win 10 Design Guide; add `Determinate`, `Error`, and `Paused` states so that it is parallel to Progress Bar.

<!-- If the feature proposal is an update, provide before / after images -->
**Before** | **After**
------------ | -------------
<img src="https://docs.microsoft.com/en-us/windows/uwp/design/controls-and-patterns/images/progressring_singlestate.png" width="200px"> | <img src="https://docs.microsoft.com/en-us/windows/communitytoolkit/resources/images/controls/radialprogressbar.png" width="200px">

<!-- Purpose of feature proposal or update -->
## Problem to Solve 
Current Progress Ring only has `Indeterminate` state  (`IsActive` Property). 

The proposal is for ProgressRing to also have the same properties as ProgressBar; specifically, `Determinate`, `Error`, `Paused` states. This feature update will allow for more flexibility where it makes more sense visually to use ProgressRing rather than ProgressBar. 

This also updates the Progress Ring visuals to be similar to Progress Bar and up to date with Windows Design Guidance.

<!-- Provide user research if applicable (is there a research study that indicates better UX with this proposed update?) -->
### Supporting User Research

[*Progress Indicators in Mobile UX Design*](https://uxplanet.org/progress-indicators-in-mobile-ux-design-a141e22f3ea0) by Nick Babich

Determinate progress indicator "offer a reason to wait and reduce users' perception of time". Furthermore, inifintely loading spinners tend to have negative connotations, as **"people don't like to stare at loading spinner with no indication of progress or time."** 

<!-- Provide competitive research if applicable (what are other teams' solutions, both within and outside of Microsoft? How can we leverage their existing solutions) -->
## Existing Solutions

**Microsoft**

_Current styling for Xbox - Fabric - Fluent/Win10_
![Xbox - Fabric - Fluent/Win10 Comps for Progress Indicators](https://user-images.githubusercontent.com/7389110/57580387-dba31c00-74a0-11e9-9c70-6f8cfa6a658e.png)

**External**

_Current styling for iOS Mobile_

<img src="https://miro.medium.com/max/1280/1*EttlyrQ2zrwq3hSjDxsuaA.png" width="600px">


## Visuals Comps 

### Controls States

States | Indeterminate | Determinate
------------ | ------------- | -------------
Running | ![Indeterminate-Running](https://github.com/karenbtlai/xaml-design-md/blob/master/indeterminate-running.png?raw=true) | ![Determinate-Running](https://github.com/karenbtlai/xaml-design-md/blob/master/determinate-running.png?raw=true)
Paused | ![Indeterminate-Paused](https://github.com/karenbtlai/xaml-design-md/blob/master/indeterminate-paused.png?raw=true) | ![Determinate-Paused](https://github.com/karenbtlai/xaml-design-md/blob/master/determinate-paused.png?raw=true)
Error | ![Indeterminate-Error](https://github.com/karenbtlai/xaml-design-md/blob/master/indeterminate-error.png?raw=true) | ![Determinate-Error](https://github.com/karenbtlai/xaml-design-md/blob/master/determinate-error.png?raw=true)

### Controls Property Mapping

Property | Controls Mapping
------------ | -------------
`Foreground` | Ring indicator
`Background` | Ring gray track 
`Stroke` | Ring thickness
`Margin` | Ring Margin
`Padding` | n/a

## Context
![Progress Ring Context](https://github.com/karenbtlai/xaml-design-md/blob/master/progressring-context.png?raw=true)

## Animation / Link to Prototype
[CodePen Prototype](https://codepen.io/anon/pen/aQeVOm)
