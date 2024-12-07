# Rofi Türk Theme

![theme](https://github.com/user-attachments/assets/600c19dc-c1cd-4722-ac19-5b7f7ded8e87)

## .config/rofi/img/TÜRK.jpg

![TÜRK](https://github.com/user-attachments/assets/3f2fa25d-c3f6-4d52-893b-1ebd1529a818)

## Desktop Wallpaper

![ATAM](https://github.com/user-attachments/assets/6ef8fda7-2edc-4c5a-933f-8b47317fbdb1)

## .config/rofi/config.rasi

```
/*****----- Configuration -----*****/
configuration {
    show-icons:                 true;
}

/*****----- Global Properties -----*****/
* {
    font:                        "JetBrains Mono Nerd Font 10";
    background:                  #000000;
    foreground:                  #FFFFFF;
    selected:                    #505050;
    active:                      #909090;
    urgent:                      #707070;
}

/*****----- Main Window -----*****/
window {
    /* properties for window widget */
    transparency:                "real";
    location:                    center;
    anchor:                      center;
    fullscreen:                  false;
    width:                       650px;
    x-offset:                    0px;
    y-offset:                    0px;

    /* properties for all widgets */
    enabled:                     true;
    border-radius:               15px;
    cursor:                      "default";
    background-color:            @background;
}

/*****----- Main Box -----*****/
mainbox {
    enabled:                     true;
    spacing:                     0px;
    background-color:            transparent;
    orientation:                 horizontal;
    children:                    [ "imagebox", "listbox" ];
}

imagebox {
    padding:                     10px;
    background-color:            transparent;
    background-image:            url("./img/TÜRK.jpg",height);
    orientation:                 vertical;
    children:                    [ "inputbar", "dummy" ];
}

listbox {
    spacing:                     20px;
    padding:                     20px;
    background-color:            #000000;
    orientation:                 vertical;
    children:                    [ "listview" ];
}

dummy {
    background-color:            transparent;
}

/*****----- Inputbar -----*****/
inputbar {
    enabled:                     true;
    spacing:                     10px;
    padding:                     15px;
    border-radius:               10px;
    background-color:            @background-alt;
    text-color:                  @foreground;
    children:                    [ "textbox-prompt-colon", "entry" ];
}
textbox-prompt-colon {
    enabled:                     true;
    expand:                      false;
    str:                         "";
    background-color:            inherit;
    text-color:                  inherit;
}
entry {
    enabled:                     true;
    background-color:            inherit;
    text-color:                  inherit;
    cursor:                      text;
    placeholder:                 "🇹🇷";
    placeholder-color:           inherit;
}

/*****----- Listview -----*****/
listview {
    enabled:                     true;
    columns:                     1;
    lines:                       5;
    cycle:                       false;
    dynamic:                     true;
    scrollbar:                   false;
    reverse:                     false;
    border:                      0px solid;
    spacing:                     10px;
    text-color:                  @foreground;
}

/*****----- Elements -----*****/
element {
    enabled:                     true;
    spacing:                     15px;
    padding:                     8px;
    border-radius:               10px;
    background-color:            transparent;
    text-color:                  @foreground;
    cursor:                      pointer;
}
element normal.normal {
    background-color:            inherit;
    text-color:                  inherit;
}
element normal.urgent {
    background-color:            @urgent;
    text-color:                  @foreground;
}
element normal.active {
    background-color:            @active;
    text-color:                  @foreground;
}
element selected.normal {
    background-color:            @selected;
    text-color:                  @foreground;
}
element selected.urgent {
    background-color:            @urgent;
    text-color:                  @foreground;
}
element selected.active {
    background-color:            @urgent;
    text-color:                  @foreground;
}
element-icon {
    background-color:            transparent;
    text-color:                  inherit;
    size:                        32px;
    cursor:                      inherit;
}
element-text {
    background-color:            transparent;
    text-color:                  inherit;
    cursor:                      inherit;
    vertical-align:              0.5;
    horizontal-align:            0.0;
}
element.alternate.normal {
    background-color: #000000;
    text-color:       #FFFFFF;
}

/*****----- Message -----*****/
message {
    background-color:            transparent;
}
textbox {
    padding:                     15px;
    border-radius:               10px;
    background-color:            @background-alt;
    text-color:                  @foreground;
    vertical-align:              0.5;
    horizontal-align:            0.0;
}
error-message {
    padding:                     15px;
    border-radius:               20px;
    background-color:            @background;
    text-color:                  @foreground;
}
```
