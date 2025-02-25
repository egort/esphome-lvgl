# Humidity
{"page":1,"id":3,"obj":"arc","x":130,"y":45,"w":140,"h":100,"max":100,"border_side":0,"type":0,"start_angle":180,"end_angle":0,"start_angle10":180,"value_font":12,"value_color":"#0F0F0F","value_ofs_x":-19,"value_ofs_y":-4,"bg_opa":0}
# humidity arc 
mosquitto_pub -h 10.168.1.4 -p 1883 -t "hasp/plate/command/p1b3.val" -m "50"
# humidity value
mosquitto_pub -h 10.168.1.4 -p 1883 -t "hasp/plate/command/p1b3.value_str" -m "50"

# Temperature
{"page":1,"id":2,"obj":"arc","x":5,"y":45,"w":140,"h":100,"max":40,"border_side":0,"type":0,"rotation":0,"start_angle":180,"end_angle":0,"start_angle10":180,"value_font":12,"value_color":"#0F0F0F","value_ofs_x":-19,"value_ofs_y":-4,"bg_opa":0}
# temp arc
mosquitto_pub -h 10.168.1.4 -p 1883 -t "hasp/plate/command/p1b2.val" -m "50"
# temp value
mosquitto_pub -h 10.168.1.4 -p 1883 -t "hasp/plate/command/p1b2.value_str" -m "35"

# text
{"page":1,"id":4,"obj":"label","x":0,"y":120,"w":240,"h":20,"align":"center","text":"CO2 levels: ","radius":0,"border_side":0}

# reboot dev
mosquitto_pub -h 10.168.1.4 -p 1883 -t "hasp/plate/command" -m "reboot"

==============================================================================
// {"page":1,"comment":"---------- Page 1 ----------"}
{"page":1,"id":0,"bg_color":"#FFFFFF","bg_grad_color":"#FFFFFF","text_color":"#000000","radius":0,"border_side":0}

{"page":1,"id":10,"obj":"label","x":160,"y":8,"w":40,"h":20,"align":"left","text":"attic","radius":0,"border_side":0}         // Attic
{"page":1,"id":11,"obj":"label","x":140,"y":100,"w":40,"h":20,"align":"left","text":"living","radius":0,"border_side":0}      // Living Room
{"page":1,"id":12,"obj":"label","x":30,"y":80,"w":40,"h":20,"align":"left","text":"outer","radius":0,"border_side":0}         // Outer space
{"page":1,"id":13,"obj":"label","x":6,"y":215,"w":40,"h":20,"align":"center","text":"water","radius":0,"border_side":0}       // Water Cleaning Room
{"page":1,"id":14,"obj":"label","x":155,"y":158,"w":40,"h":20,"align":"center","text":"veranda","radius":0,"border_side":0}   // Veranda
{"page":1,"id":15,"obj":"label","x":180,"y":40,"w":40,"h":20,"align":"center","text":"artem","radius":0,"border_side":0}      // Artem's Room
{"page":1,"id":16,"obj":"label","x":25,"y":180,"w":40,"h":20,"align":"center","text":"laundry","radius":0,"border_side":0}    // Laundry Room
{"page":1,"id":17,"obj":"label","x":190,"y":105,"w":40,"h":20,"align":"center","text":"hydra","radius":0,"border_side":0}     // Hydraulic Room
{"page":1,"id":18,"obj":"label","x":170,"y":265,"w":40,"h":20,"align":"center","text":"office","radius":0,"border_side":0}    // Office Room
{"page":1,"id":19,"obj":"label","x":120,"y":40,"w":40,"h":20,"align":"center","text":"cath","radius":0,"border_side":0}       // Catherine Room

{"page":1, "id":30,  "obj":"line", "points":[[10,170],[10,240],[70,240],[70,170],[10,170]], "auto_size":0, "y_invert":0}      // 2nd build / laundry room
{"page":1, "id":31,  "obj":"line", "points":[[10,210],[40,210],[40,240],[10,240],[10,210]], "auto_size":0, "y_invert":0}      // 2nd build / water cleaning room
{"page":1, "id":32,  "obj":"line", "points":[[10,240],[10,310],[70,310],[70,240]], "auto_size":0, "y_invert":0}               // 2nd build / RD Room
{"page":1, "id":33,  "obj":"line", "points":[[70,250],[70,310],[140,310],[140,250],[70,250]], "auto_size":0, "y_invert":0}    // 2nd build / Garage
{"page":1, "id":34,  "obj":"line", "points":[[140,250],[140,310],[230,310],[230,250],[140,250]], "auto_size":0, "y_invert":0} // 2nd build / office

{"page":1, "id":40,  "obj":"line", "points":[[110,30],[110,70],[170,70],[170,30],[110,30]], "auto_size":0, "y_invert":0}      // 1st build / Catrine Room
{"page":1, "id":41,  "obj":"line", "points":[[170,30],[170,70],[230,70],[230,30],[170,30]], "auto_size":0, "y_invert":0}      // 1st build / Artem Room
{"page":1, "id":42,  "obj":"line", "points":[[190,70],[190,100],[230,100],[230,70],[190,70]], "auto_size":0, "y_invert":0}    // 1st build / WC
{"page":1, "id":43,  "obj":"line", "points":[[190,100],[190,130],[230,130],[230,100],[190,100]], "auto_size":0, "y_invert":0} // 1st build / Hidraulic Room
{"page":1, "id":44,  "obj":"line", "points":[[110,70],[110,160],[230,160],[230,70],[110,70]], "auto_size":0, "y_invert":0}    // 1st build / Living Room
{"page":1, "id":45,  "obj":"line", "points":[[110,160],[110,180],[230,180],[230,160],[110,160]], "auto_size":0, "y_invert":0} // 1st build / Veranda
{"page":1, "id":46,  "obj":"line", "points":[[80,70],[80,120],[110,120],[110,70],[80,70]], "auto_size":0, "y_invert":0}       // 1st build / Entrance
{"page":1, "id":47,  "obj":"line", "points":[[110,30],[170,5],[230,30]], "auto_size":0, "y_invert":0}                         // 1st build / Attic

// {"page":0,"comment":"---------- All pages ----------"}
// {"page":0,"id":11,"obj":"btn","action":"prev","x":0,"y":290,"w":79,"h":32,"bg_color":"#34495E","text":"\uE141","text_color":"#000000","radius":0,"border_side":0,"text_font":32}
// {"page":0,"id":12,"obj":"btn","action":"back","x":80,"y":290,"w":80,"h":32,"bg_color":"#34495E","text":"\uE2DC","text_color":"#000000","radius":0,"border_side":0,"text_font":24}
// {"page":0,"id":13,"obj":"btn","action":"next","x":161,"y":290,"w":79,"h":32,"bg_color":"#34495E","text":"\uE142","text_color":"#000000","radius":0,"border_side":0,"text_font":32}

Moodlight GPIO Settings
4	Red	  Inverted
16	Green Inverted
17	Blue  Inverted

