# Open Park App

## Data layer

### Data

- Collection of park
  - park:
    - id: number
    - name: string
    - isDone: boolean

### Modifications

- addPark()
- removePark()
- updatePark()
- loadPark()
- togglePark()

## Components

### Store

#### State

- Collection of Parks

#### ParkReducer

- addPark()
- removePark()
- updatePark()
- loadParks()
- togglePark()

### App

- Receives an external collection of Park
- Receives a collection of Park
- Receives dispatch()
- Shows the title of the app inside a heading
- Renders a ParkForm
- Renders a ParksList component

### ParkForm

- State:
  - Park
- handleSubmit()
- Receives dispatch()
- Receives an optional Park to update
- Shows an input text for the name of the Park
- Renders a Button component
  - text: "create" / "modify"
  - actionOnClick: handleSubmit

### ParkList

- Receives a collection of Parks
- Renders as many ParkCard as Parks are in the collection

### ParkCard

- Receives a Park
- Receives dispatch()
- handleClick()
- Shows the Park's name inside a heading
- Shows a check when the received Park is done
- Renders a Button with:
  - text: "delete"
  - actionOnClick: handleClick

### Button

- Receives a text
- Receives an action on click
- Shows a button with the received text
- Calls the received action when the button is clicked
