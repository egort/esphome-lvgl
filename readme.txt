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

Moodlight GPIO Settings
4	Red	  Inverted
16	Green Inverted
17	Blue  Inverted

