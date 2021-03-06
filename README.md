An Arduino library to tokenize and parse commands received over a serial port. 
Commands are based on JSON Strings <COMMAND>\r<JSON string>\r

Initially documented here: http://arduino.vn/node/1497

This version is the one on Github. 
Basic API: in examples. (Basic_API)
/******************************************************************************* 
SerialCommand - An Arduino library to tokenize and parse commands received over
a serial port. 
Based on 2011-2013 Steven Cogswell  <steven.cogswell@gmail.com>
Based on 2017 Ngo Huynh Ngoc Khanh <ngohuynhngockhanh@gmail.com>
Copyright 2017 Dao Minh An <minhan7497@gmail.com>
http://arduino.vn

Version 2017.   

Version History:
May 11 2011 - Initial version
May 13 2011 -	Prevent overwriting bounds of SerialCommandCallback[] array in addCommand()
			defaultHandler() for non-matching commands
Mar 2012 - Some const char * changes to make compiler happier about deprecated warnings.  
           Arduino 1.0 compatibility (Arduino.h header) 
Oct 2013 - SerialCommand object can be created using a SoftwareSerial object, for SoftwareSerial
           support.  Requires #include <SoftwareSerial.h> in your sketch even if you don't use 
           a SoftwareSerial port in the project.  sigh.   See Example Sketch for usage. 
Oct 2013 - Conditional compilation for the SoftwareSerial support, in case you really, really
           hate it and want it removed.  
Feb 2017 - Allow command and arguments into two buffers JSON
July 2017 - A little fix by DMA by add a new function available()

This library is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.

This library is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public
License along with this library; if not, write to the Free Software
Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA

Developed from the version of kps from : http://arduino.vn/bai-viet/1497-esp8266-ket-noi-internet-phan-2-arduino-gap-esp8266-hai-dua-noi-chuyen-bang-json
                                         
https://github.com/ngohuynhngockhanh/ArduinoSerialCommand

***********************************************************************************/







                                         
