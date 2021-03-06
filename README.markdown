# Screen Recorder

A port of `screen_recorder.rb` from from [AXElements](http://github.com/Marketcircle/AXElements),
but cleaned up and rewritten in C to be more portable across languages and
runtimes.

[Documentation](http://rdoc.info/gems/screen_recorder/frames)


## Examples

    require 'screen_recorder'

    # in block form
    ScreenRecorder.record do
        sleep 10 # go and do stuff
    end
    # now go check ~/Movies

    # in "classic" form
    recorder = ScreenRecorder.new
    recorder.start
    # go do stuff
    recorder.stop
    # now go check ~/Movies

Both block and non-block forms take an optional string, which should
be a path to save the recording (the default saves to `~/Movies`).


## TODO

* Expose recorder options at initialization (e.g. turn off mouse clicks)


## Copyright

Copyright (c) 2012, Mark Rada
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright
  notice, this list of conditions and the following disclaimer.
* Redistributions in binary form must reproduce the above copyright
  notice, this list of conditions and the following disclaimer in the
  documentation and/or other materials provided with the distribution.
* Neither the name of Mark Rada nor the names of its
  contributors may be used to endorse or promote products derived
  from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL Mark Rada BE LIABLE FOR ANY
DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/AXElements/screen_recorder/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

