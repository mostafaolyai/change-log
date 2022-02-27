You should know about these

<h5>Semantic Versioning</h5>
format: <MAJOR>.<MINOR>.<PATCH>

MAJOR	Introduce a new backward-incompatible change	        1.0.0 → 2.0.0
MINOR	Introduce a new backward-compatible change	            1.0.0 → 1.1.0
PATCH	Fix a bug while maintaining backward-compatibility	    1.0.0 → 1.0.1



<h5>Major</h5>
Remove an operation, i.e. remove an HTTP verb/path combination
Add a mandatory field to a request payload
Add/remove a field to a response payload
Adding a field may not be a breaking change if all consumers are deemed sufficiently tolerant

<h5>Minor</h5>	
Add a new operation, i.e. a new HTTP verb/path combination
Add an optional field to a request payload

<h5>Patch</h5>	
No interface changes

after then install this packages:
npm i --save-dev standard-version

then we just need to add a script in our package.json
<code>
{
    "script":{
        "release":"standard-version"
    }
}
</code>

first commit:
Major
    feat: init
    BREAKING CHANGE: change license
