```

print(...)
    print(value, ..., sep=' ', end='\n', file=sys.stdout, flush=False)
    
    Prints the values to a stream, or to sys.stdout by default.
    Optional keyword arguments:
    file:  a file-like object (stream); defaults to the current sys.stdout.
    sep:   string inserted between values, default a space.
    end:   string appended after the last value, default a newline.
    flush: whether to forcibly flush the stream.


```
```
string
    + 連接
        note: 
            順序影響 
            ex: s = "BreakAllCTF{HappyHackingDay}"
                str = ""
                for i in s:
                    str = i + str  # }yaDgnikcaHyppaH{FTCllAkaerB
                  # str = str + i  # BreakAllCTF{HappyHackingDay}
                  # str += i       # BreakAllCTF{HappyHackingDay}
                print(str)

    * 複製
    
    ''' \n \t ''' or """ \n \t """  allowing strings to span multiple lines, including verbatim NEWLINEs, TABs, and any other special characters.
    
    str[] 提取部分
        [0]  提取第一個字元
        [-1] 提取最後一個字元
        
        [start:end:step]
            start  提取起始位置
            end    提取結尾位置(輸入值-1)
            step   提取的間隔

```
```
len(obj, /)
    Return the number of items in a container.


```
```
class list(object)
 |  list() -> new empty list
 |  list(iterable) -> new list initialized from iterable's items
 |  
 |  Methods defined here:
 |  
 |  __add__(self, value, /)
 |      Return self+value.
 |  
 |  __contains__(self, key, /)
 |      Return key in self.
 |  
 |  __delitem__(self, key, /)
 |      Delete self[key].
 |  
 |  __eq__(self, value, /)
 |      Return self==value.
 |  
 |  __ge__(self, value, /)
 |      Return self>=value.
 |  
 |  __getattribute__(self, name, /)
 |      Return getattr(self, name).
 |  
 |  __getitem__(...)
 |      x.__getitem__(y) <==> x[y]
 |  
 |  __gt__(self, value, /)
 |      Return self>value.
 |  
 |  __iadd__(self, value, /)
 |      Implement self+=value.
 |  
 |  __imul__(self, value, /)
 |      Implement self*=value.
 |  
 |  __init__(self, /, *args, **kwargs)
 |      Initialize self.  See help(type(self)) for accurate signature.
 |  
 |  __iter__(self, /)
 |      Implement iter(self).
 |  
 |  __le__(self, value, /)
 |      Return self<=value.
 |  
 |  __len__(self, /)
 |      Return len(self).
 |  
 |  __lt__(self, value, /)
 |      Return self<value.
 |  
 |  __mul__(self, value, /)
 |      Return self*value.
 |  
 |  __ne__(self, value, /)
 |      Return self!=value.
 |  
 |  __new__(*args, **kwargs) from builtins.type
 |      Create and return a new object.  See help(type) for accurate signature.
 |  
 |  __repr__(self, /)
 |      Return repr(self).
 |  
 |  __reversed__(...)
 |      L.__reversed__() -- return a reverse iterator over the list
 |  
 |  __rmul__(self, value, /)
 |      Return value*self.
 |  
 |  __setitem__(self, key, value, /)
 |      Set self[key] to value.
 |  
 |  __sizeof__(...)
 |      L.__sizeof__() -- size of L in memory, in bytes
 |  
 |  append(...)
 |      L.append(object) -> None -- append object to end
 |  
 |  clear(...)
 |      L.clear() -> None -- remove all items from L
 |  
 |  copy(...)
 |      L.copy() -> list -- a shallow copy of L
 |  
 |  count(...)
 |      L.count(value) -> integer -- return number of occurrences of value
 |  
 |  extend(...)
 |      L.extend(iterable) -> None -- extend list by appending elements from the iterable
 |  
 |  index(...)
 |      L.index(value, [start, [stop]]) -> integer -- return first index of value.
 |      Raises ValueError if the value is not present.
 |  
 |  insert(...)
 |      L.insert(index, object) -- insert object before index
 |  
 |  pop(...)
 |      L.pop([index]) -> item -- remove and return item at index (default last).
 |      Raises IndexError if list is empty or index is out of range.
 |  
 |  remove(...)
 |      L.remove(value) -> None -- remove first occurrence of value.
 |      Raises ValueError if the value is not present.
 |  
 |  reverse(...)
 |      L.reverse() -- reverse *IN PLACE*
 |  
 |  sort(...)
 |      L.sort(key=None, reverse=False) -> None -- stable sort *IN PLACE*
 |  
 |  ----------------------------------------------------------------------
 |  Data and other attributes defined here:
 |  
 |  __hash__ = None


```
```
string

capitalize(...) method of builtins.str instance
    S.capitalize() -> str
    
    Return a capitalized version of S, i.e. make the first character
    have upper case and the rest lower case.



encode(...) method of builtins.str instance
    S.encode(encoding='utf-8', errors='strict') -> bytes
    
    Encode S using the codec registered for encoding. Default encoding
    is 'utf-8'. errors may be given to set a different error
    handling scheme. Default is 'strict' meaning that encoding errors raise
    a UnicodeEncodeError. Other possible values are 'ignore', 'replace' and
    'xmlcharrefreplace' as well as any other name registered with
    codecs.register_error that can handle UnicodeEncodeErrors.



find(...) method of builtins.str instance
    S.find(sub[, start[, end]]) -> int
    
    Return the lowest index in S where substring sub is found,
    such that sub is contained within S[start:end].  Optional
    arguments start and end are interpreted as in slice notation.
    
    Return -1 on failure.



format(...) method of builtins.str instance
    S.format(*args, **kwargs) -> str
    
    Return a formatted version of S, using substitutions from args and kwargs.
    The substitutions are identified by braces ('{' and '}').



isalnum(...) method of builtins.str instance
    S.isalnum() -> bool
    
    Return True if all characters in S are alphanumeric
    and there is at least one character in S, False otherwise.



isalpha(...) method of builtins.str instance
    S.isalpha() -> bool
    
    Return True if all characters in S are alphabetic
    and there is at least one character in S, False otherwise.



join(...) method of builtins.str instance
    S.join(iterable) -> str
    
    Return a string which is the concatenation of the strings in the
    iterable.  The separator between elements is S.


```
```
time

time.localtime([ sec ])
    it converts number of seconds to local time. If secs is not provided 
    or None, the current time as returned by time() is used. The dst flag 
    is set to 1 when DST applies to the given time.
    
    sec − These are the number of seconds to be converted into structure struct_time representation.


```
```
sum(iterable, start=0, /)
    Return the sum of a 'start' value (default: 0) plus an iterable of numbers
    
    When the iterable is empty, return the start value.
    This function is intended specifically for use with numeric values and may
    reject non-numeric types.


```
```
class range(object)
 |  range(stop) -> range object
 |  range(start, stop[, step]) -> range object
 |  
 |  Return an object that produces a sequence of integers from start (inclusive)
 |  to stop (exclusive) by step.  range(i, j) produces i, i+1, i+2, ..., j-1.
 |  start defaults to 0, and stop is omitted!  range(4) produces 0, 1, 2, 3.
 |  These are exactly the valid indices for a list of 4 elements.
 |  When step is given, it specifies the increment (or decrement).
 |  
 |  Methods defined here:
 |  
 |  __bool__(self, /)
 |      self != 0
 |  
 |  __contains__(self, key, /)
 |      Return key in self.
 |  
 |  __eq__(self, value, /)
 |      Return self==value.
 |  
 |  __ge__(self, value, /)
 |      Return self>=value.
 |  
 |  __getattribute__(self, name, /)
 |      Return getattr(self, name).
 |  
 |  __getitem__(self, key, /)
 |      Return self[key].
 |  
 |  __gt__(self, value, /)
 |      Return self>value.
 |  
 |  __hash__(self, /)
 |      Return hash(self).
 |  
 |  __iter__(self, /)
 |      Implement iter(self).
 |  
 |  __le__(self, value, /)
 |      Return self<=value.
 |  
 |  __len__(self, /)
 |      Return len(self).
 |  
 |  __lt__(self, value, /)
 |      Return self<value.
 |  
 |  __ne__(self, value, /)
 |      Return self!=value.
 |  
 |  __new__(*args, **kwargs) from builtins.type
 |      Create and return a new object.  See help(type) for accurate signature.
 |  
 |  __reduce__(...)
 |      helper for pickle
 |  
 |  __repr__(self, /)
 |      Return repr(self).
 |  
 |  __reversed__(...)
 |      Return a reverse iterator.
 |  
 |  count(...)
 |      rangeobject.count(value) -> integer -- return number of occurrences of value
 |  
 |  index(...)
 |      rangeobject.index(value, [start, [stop]]) -> integer -- return index of value.
 |      Raise ValueError if the value is not present.
 |  
 |  ----------------------------------------------------------------------
 |  Data descriptors defined here:
 |  
 |  start
 |  
 |  step
 |  
 |  stop


```
