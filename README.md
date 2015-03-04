# rtc-pluggable-signaller

By using `rtc-pluggable-signaller` in your code, you provide the ability
for your package to customize which signalling client it uses (and
thus have significant control) over how signalling operates in your
environment.


[![NPM](https://nodei.co/npm/rtc-pluggable-signaller.png)](https://nodei.co/npm/rtc-pluggable-signaller/)



## How it Works

The pluggable signaller looks in the provided `opts` for a `signaller`
attribute.  If the value of this attribute is a string, then it is
assumed that you wish to use the default
[`rtc-signaller`](https://github.com/rtc-io/rtc-signaller) in your
package.  If, however, it is not a string value then it will be passed
straight back as the signaller (assuming that you have provided an
object that is compliant with the rtc.io signalling API).

## License(s)

### Apache 2.0

Copyright 2015 Damon Oehlman <damon.oehlman@nicta.com.au>

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
