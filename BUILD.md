# Build Outline

## BOM

## Design

## Tools
- 1/16 bit (pilot)
- 3/32 bit (RPi mount)
- 1/8 bit (panel mount)
- 1/4 bit (LED)
- 1/2 bit (LED notch)

## Clean

## Top Half
- Cartridge Insert
    - Super glue to top half (24-hour cure)
    - Install USB ports
- Fan
    - Mark air direction (positive pressure)
    - Crimp female dupont pins
    - 2-pin female header
    - Position on left side
    - Position wire toward front/center
    - Super glue to top half (24-hour cure)
- LED
    - Choose resistor value
    - Supply 5V to minimum resistor and 1k potentiometer in series
    - Connect multimeter to monitor resistance
    - Adjust pot until ideal brightness found
    - Write down desired resistance
    - Crimp female dupont pins
    - 2-pin female header
    - Drill pilot through assembled chassis to create a reference point for the
      notch in bottom half
    - Separate the halves and finish hole using 1/4 bit
    - Install LED

## Bottom Half
- LED
    - Drill hole through reference using 1/2 bit
    - Avoid pillar (may need to reduce bit size)
    - Remove top of notch with xacto blade to create a U-shaped notch
- Barrel Connector
    - Solder hookup wire for center positive
    - Heat shrink around soldered terminals
    - Separate and solder unterminated ends
    - Write down preferred length (10"?)
- Back Panel
    - Place panel and secure with clamp
    - Mark drills with pencil and remove panel
    - Drill pilots from inside
    - Create center line based on pilot holes for Ethernet and HDMI
    - Mark slots in pencil for Ethernet and HDMI on outside
    - Drill screw holes from outside using 1/8
    - Drill HDMI and Ethernet holes, square off with xacto and file
    - Slightly enlarge power hole with xacto
    - Install panel mounts
- RPi
    - Drill holes for mounts using 3/32 (check 1/16)
    - Install standoffs; attach from bottom with screws
    - Install second tier standoffs and secure RPi
    - Install heat sinks on CPU & GPU
        - Position with fins parallel to airflow (left to right)
    - PowerBlock
        - Rework resistor for LED
        - Solder 2 pin header on 5V OUT for fan
        - Solder power to 5V IN
        - Install PowerBlock and screw down
    - Switch Panels
        - Assemble Switch Panels
            - Solder J1-J3
            - Solder S1-S3
            - Installation order (left to right)
                - 4 x toggle
                - 2 x momentary
        - Partially thread screw from below through the panel to hold it in
          place
        - Place felt discs over switch posts

## Final Assembly
- Connect J1 (1-2) to switch header
- Connect fan to 5V OUT header
- Connect LED to header
- Connect USB from Back Panel (#1-2, left to right)
- Connect USB from Cartridge Insert to RPi (#3-4, left to right)
- Connect Ethernet
- Connect HDMI
- Screw top and bottom halves together (4 screws from below)

## References
- See: https://sensorgnome.org/@api/deki/files/7290/=usb_port_numbering.png
