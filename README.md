```
# wifi_pwn-modulefix
# wifi_pwn python2 scripts modul error fixing tricks. No need pip2!
```
```
find the missing module (find, locale) -> add the module path in scipt (import os...) -> forcing import again due error the first import trick

try:
        import <module>
except Exception, e:
	print 'Failed to import <module>:',e
        import <module> # again import
	
(no found the module)
pip3 install <module> -> search again (find, locale) -> (import module tricks)
```
```
(run)
python2 <script>.py -h # --help
```
```
The only advantage of this is that it doesn't require any dependencies by default!

Some scripts won't work with this method either!
Solution: Download pip2 from source. Recommended use virtualenv in order to avoid other errors.
other info: https://stackoverflow.com/questions/46602880/importerror-no-module-named-scapy-all
```
