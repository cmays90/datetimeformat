# datetimeformat
A DateTime formatting library for D

#Sample Usage

    import datetimeformat;
    import std.stdio;
    import datetime;

    void main()
    {
        SysTime dt = SysTime(DateTime(2005, 9, 8, 16, 51, 9), dur!"msecs"(427));
        writeln(dt.format("yyyy-mm-dd HH:ii:ss.FFF")); //"2005-09-08 16:51:09.427"
    }

#Acknowledgments

This is based on [Stewart's Utility Library datetime and datetimeformat](http://pr.stewartsplace.org.uk/d/sutil/doc/datetimeformat.html).

It has been adapated to use Phobo's DateTime object instead of SUL's datetime, removing a dependency.

Notably missing in this version is the ability to have and utilize "collapsable" tags.
