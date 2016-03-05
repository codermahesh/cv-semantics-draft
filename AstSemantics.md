
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
2.Memory load/Store
3.Local Variables
4.


