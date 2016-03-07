
For Now Assuming UMA for abstract machine, to covert it one can
simply add attribute for data segments


#### Modules
## Logical Layout
# DataSegment
-- Accepts data dynamically,but compiler knows about spacing limits, !!! Opt :D 
1.DataInSize
2.DataIn[0...DataInSize-1]
3.DataOutSize
4.DataOut[0...DataOutSize-1]

#Buffer Segment
-- Temporary memory that may be used as scratch, /*Do this requred?*/

# Code Segment
 -- Only operates on data from data segment, for now
 -- All intructions are vectorized in data i.e SIMD

1.Types 
### Integral Types
	8, 16 , 32 bit Integer Registers with 2-Complement representation

### Pixel Types
	8, 16,  24 bit psuedo Registers with saturated/unsaturated math

### Cast Conversions
	I. Downcasts
		-- Integral Downcasts  16_to_8, 32_to_16
		-- Pixel Downcasts 
		   Consider bitdepth conversions, scope for opts 	    
	II. Upcasts   
		-- Integral Upcasts 8_to_16, 16_to_32
		-- Pixel Upcasts 8_to_16, 16_to_24
		
2.Memory load/Store
3.Local Variables
4.Control Flow
  


