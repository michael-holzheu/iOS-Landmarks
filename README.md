Today we followed the instructions of the Apple tutorial [Creating and Combining Views](https://developer.apple.com/tutorials/swiftui/creating-and-combining-views) to create our first iOS-App:

<img width="1204" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222926142-fa1a4a82-2d2d-4f5a-b22e-b6fb10ddf08d.png">

# Table of Contents

- [What we will learn about xCode](#what-we-will-learn-about-xcode)
  * [IDE Components](#ide-components)
  * [List of IDE components](#list-of-ide-components)
  * [Concepts](#concepts)
    + [Binding](#binding)
    + [State variable](#state-variable)
  * [Views](#views)
  * [Containers](#containers)
    + [General](#general)
  * [Shortcuts](#shortcuts)
- [Section 3: Combine Views Using Stacks](#section-3--combine-views-using-stacks)
  * [Create VStack](#create-vstack)
    + [Befor Create](#befor-create)
    + [After Create](#after-create)
    + [Create Text View](#create-text-view)
    + [Add Text View](#add-text-view)
  * [Create HStack](#create-hstack)
    + [After Create](#after-create-1)
  * [Add Text View](#add-text-view-1)
  * [Add Spacer - Step 1](#add-spacer---step-1)
  * [Add Spacer - Step 2](#add-spacer---step-2)
  * [Add Padding](#add-padding)
  * [Remove Padding](#remove-padding)
- [Section 4: Create a Custom Image View](#section-4--create-a-custom-image-view)
  * [Add image to asset catalog - Step 1](#add-image-to-asset-catalog---step-1)
  * [Add image to asset catalog - Step 2](#add-image-to-asset-catalog---step-2)
  * [Add image to asset catalog - Step 3](#add-image-to-asset-catalog---step-3)
  * [Add image to asset catalog - Step 4: Rename file](#add-image-to-asset-catalog---step-4--rename-file)
  * [Create new source file SwiftUI View - Step 1](#create-new-source-file-swiftui-view---step-1)
  * [Create new source file SwiftUI View - Step 2](#create-new-source-file-swiftui-view---step-2)
  * [Create new source file SwiftUI View - Step 3](#create-new-source-file-swiftui-view---step-3)
  * [Create new source file SwiftUI View - Step 4](#create-new-source-file-swiftui-view---step-4)
  * [Add image to UI](#add-image-to-ui)
  * [Add circle mask](#add-circle-mask)
  * [Add overlay](#add-overlay)
  * [Add shaddow](#add-shaddow)
  * [Change border color to white](#change-border-color-to-white)
- [Section 5: Use SwiftUI Views From Other Frameworks](#section-5--use-swiftui-views-from-other-frameworks)
  * [Create new UI file - Step 1](#create-new-ui-file---step-1)
  * [Create new UI file - Step 2: MapView.swift](#create-new-ui-file---step-2--mapviewswift)
  * [Add import statement](#add-import-statement)
  * [Add State](#add-state)
  * [Add Map view with $state as coordinates](#add-map-view-with--state-as-coordinates)
- [Section 6: Compose the Detail View](#section-6--compose-the-detail-view)
  * [Create new VStack - Step 1](#create-new-vstack---step-1)
  * [Create new VStack - Step 2](#create-new-vstack---step-2)
  * [Add MapView](#add-mapview)
  * [Remove image - Leftover from initial template](#remove-image---leftover-from-initial-template)
  * [Add CircleImage](#add-circleimage)
  * [Move up CircleImage](#move-up-circleimage)
  * [Add Spacer to move all to top of the screen](#add-spacer-to-move-all-to-top-of-the-screen)
  * [Add ignoresSaveArea (no effect?)](#add-ignoressavearea)
  * [Add descriptive text](#add-descriptive-text)
  * [Move attributes to HStack](#move-attributes-to-hstack)
  * [Remove green](#remove-green)
- [Section 7: Run on real device](#section-7--run-on-real-device)
  * [Add Account](#add-account)
  * [Assign Team](#assign-team)
  * [Enalbe developer modus on iPad](#enalbe-developer-modus-on-ipad)
  * [Restart iPad](#restart-ipad)
  * [Connect iPad via USB and select device](#connect-ipad-via-usb-and-select-device)
  * [Try to run app](#try-to-run-app)
  * [App will be installed, but can't be run](#app-will-be-installed--but-can-t-be-run)
  * [Trust developer - Step 1: Einstellungen > Allgemein > Geräteverwaltung](#trust-developer---step-1--einstellungen---allgemein---ger-teverwaltung)
  * [Trust developer - Step 2](#trust-developer---step-2)
  * [Run app - Tada!](#run-app)

# What we will learn about xCode

## IDE Components

<img width="1239" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222914656-c4ee6098-8ac4-429e-ab49-0891ee590b18.png">

## List of IDE components

- Asset catalog
- Editor
- Canvas
- Inspector

## Concepts

### Binding

- Use a leading '$' to mark a binding
- For example $state
- It is like a reference to the underlying value

### State variable

- Attribute: @State
- Source of truth for data
- All related views will automatically updated when data changes

## Views

- Divider
- Image
- Map
- Spacer
- Text

## Containers

- HStack (Horizontal Stack)
- VStack (Vertical Stack)

### General

- All attributes to container (e.g. font) apply to all children


## Shortcuts

- CMD-Click: Opens context menu
- CTRL-I: Autoformat (indentation)

# Section 3: Combine Views Using Stacks

## Create VStack

### Befor Create
![image](https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222916397-af0563c5-f233-4d7a-b6eb-7e81d0335a92.png)

### After Create
![image](https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222916591-94677d34-e1be-4e53-838b-dce7b0a24c11.png)

### Create Text View
![image](https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222916721-51b28ac7-c855-4143-85c0-8cecf212d78b.png)

### Add Text View
<img width="1259" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222917267-b6fde914-540b-46f5-bc8b-949a2a8b7d57.png">

## Create HStack

<img width="1259" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222918084-92daffb1-2457-410f-b410-bad42896f0e5.png">

### After Create
<img width="1259" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222918161-afa979a1-67e1-4819-9638-f6dc59e1553c.png">

## Add Text View
<img width="1259" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222919079-e700a9d1-bda0-4c1c-a922-6457b8eb93b6.png">

## Add Spacer - Step 1
<img width="1259" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222919130-97fa5570-5a8c-4235-9a1f-54602df7eb8b.png">

## Add Spacer - Step 2
<img width="1259" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222919181-15af31ff-6d1c-4340-8cfe-64c58ea9d235.png">

## Add Padding

<img width="1259" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222919278-c01c86d8-e382-4ea3-bba0-1d8303ff0937.png">

## Remove Padding

<img width="1259" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222919307-55322c85-2b46-49b0-b188-3bd385799b7b.png">

# Section 4: Create a Custom Image View

## Add image to asset catalog - Step 1

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920254-36aa909f-ebc5-429e-9608-517f84851e69.png">

## Add image to asset catalog - Step 2

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920309-2f961fe8-58f8-47b5-b135-e6f25f2749a9.png">

## Add image to asset catalog - Step 3

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920333-f5d57914-e715-4cca-aa95-2798db3f68dd.png">

## Add image to asset catalog - Step 4: Rename file

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920770-3e334b74-326c-4544-ba68-a3c2da14c134.png">

## Create new source file SwiftUI View - Step 1

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920497-04d45004-9bb8-4195-b31e-a27a8ff9e72c.png">

## Create new source file SwiftUI View - Step 2

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920557-cb6e0a8c-f228-4804-8a67-d3aa94589b78.png">

## Create new source file SwiftUI View - Step 3

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920625-0e89cab7-0eef-4800-9efb-89a86670f0ee.png">

## Create new source file SwiftUI View - Step 4

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920682-d8a5ac92-b3a7-4525-a35b-26878d861100.png">

## Add image to UI

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920883-b89df8e9-ebfe-4d5e-abc9-3eadff17cb8b.png">

## Add circle mask

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222920950-93489cb0-bcd5-470d-b048-013d89a86ac3.png">

## Add overlay

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222921122-8f7bcc47-7481-4036-b8bf-d1dea31ef6a2.png">

## Add shaddow

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222921173-121288ee-f668-48b8-bf41-ef6886455c61.png">

## Change border color to white

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222921238-a6e0f3bc-b410-40fe-a420-727244e97f48.png">

# Section 5: Use SwiftUI Views From Other Frameworks

## Create new UI file - Step 1

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222921738-eb15d100-e52d-4b2e-8c7c-33e0f47d7c11.png">

## Create new UI file - Step 2: MapView.swift

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222921782-6e55bd59-91bc-4d1c-99e5-f8b00a0b61dd.png">

## Add import statement

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222921849-ecc40f30-5043-4c16-9f26-80fe92eb4bb5.png">

## Add State

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222922265-9ff97928-a882-449f-a597-32d73b056356.png">

## Add Map view with $state as coordinates

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222922348-982b7fc8-b609-40cd-a88c-992fb1aef8af.png">

# Section 6: Compose the Detail View

## Create new VStack - Step 1

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222922821-f310a9b9-f07c-42c9-97c3-06e1d6b33226.png">

## Create new VStack - Step 2

<img width="1261" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222923028-2d07bbf6-b79c-4e17-ae41-ddc1d0fb67ed.png">

## Add MapView

<img width="1244" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222923165-daf04ba6-e557-4d52-8e1f-5fd5050fd6bc.png">

## Remove image - Leftover from initial template

<img width="1244" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222923244-5dcbd1e9-8e23-40c7-946d-e68573a35ad9.png">

## Add CircleImage

<img width="1244" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222923342-2a0defd3-3a43-481c-a9aa-29ff7d724934.png">

## Move up CircleImage

<img width="1266" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222923453-9288fcc5-00b1-4e96-9381-94e15e14053c.png">

## Add Spacer to move all to top of the screen

<img width="1266" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222923513-c8283c23-d949-453d-9898-2f06ceebf096.png">

## Add ignoresSaveArea

<img width="1266" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222923673-4bcd96b8-35bb-4a14-9a6d-28fba2762d58.png">

## Add descriptive text

<img width="1266" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222924081-806587b9-c5b9-49a9-bd82-7822a8ae69ad.png">

## Move attributes to HStack

<img width="1266" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222924291-0613675b-cfd3-43ee-a691-a1b9fde28324.png">

## Remove green

<img width="1266" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222924331-ff5c9111-a529-44ad-837e-12e340195da4.png">

# Section 7: Run on real device

## Add Account

<img width="1266" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222924785-f2f94ddc-c365-4dee-b7ec-a9727a53b369.png">

## Assign Team

<img width="1251" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222925036-dc4de8ef-2cb9-43a1-9700-cce0b6b1675e.png">

## Enalbe developer modus on iPad

<img width="1030" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222925294-9bc52284-7e53-47e4-b165-c3f531359a1f.png">

## Restart iPad

<img width="1035" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222925329-02fce384-a750-4c27-bb79-dbae36284fd4.png">

## Connect iPad via USB and select device

<img width="1266" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222924893-94fb86f9-1a4b-4193-8738-deba3e76749e.png">

## Try to run app

<img width="1277" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222925726-483b9626-1ada-4bfc-8dd9-775b51e6ccbe.png">

## App will be installed, but can't be run

<img width="1206" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222925934-ae939876-728e-4ef9-b173-d433ab1953d1.png">

## Trust developer - Step 1: Einstellungen > Allgemein > Geräteverwaltung

<img width="1207" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222926012-0bb53063-594a-4e37-b0e7-3a8e38697d44.png">

## Trust developer - Step 2

<img width="1201" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222926090-f494bac8-0a56-4bbc-ab50-c901cf14e733.png">

## Run app

<a href="https://youtu.be/Jkzf_HWq90Y?t=666"><img width="1201" alt="image" src="https://github.com/michael-holzheu/Landmarks/blob/main/user-images/222926142-fa1a4a82-2d2d-4f5a-b22e-b6fb10ddf08d-play.png"></a>

Best Regards and Happy Coding!

Michael Holzheu
