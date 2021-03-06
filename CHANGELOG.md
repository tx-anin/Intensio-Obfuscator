# CHANGELOG of Intensio-Obfuscator project

## 03-16-2020
- [upgrade] to version 1.0.8.2
- [update] StringGenerator function to reduce the process of string replacement when `-rts, --replacetostr` is called
- [update] move any line feed (\n) after disabling the color

## 03-10-2020
- [upgrade] to version 1.0.8.1 
- [remove] intensio_error.py file, that contained useless feature to improve verbosity type of error during the reading of Intensio-Obfuscator code
- [remove] `simple` level of string generated for obfuscation is removed, previous parameter` hard` level obfuscation is used by default for level of strings generated for obfuscation now
- [remove] parameter `-mlvl, --mixerlevel` to control obfuscation level of strings generated (`simple` by default or `hard`)

## 02-01-2020
- [update] visibility of code with PEP 8 recommandation part `maximum line length` 

## 01-28-2020
- [upgrade] to version 1.0.8
- [update] `-m, -mixerlevel` becomes `-mlen, --mixerlength` to control length of random strings generated
- [update] redefine all colors without external library
- [fix] issue # 14
- [fix] issue # 28
- [add] new paramter `-mlvl, --mixerlevel` to control obfuscation level of strings generated (`simple` by default or `hard`)

## 03-10-2020 
- [Remove] intensio_error.py file, that contained useless feature to improve verbosity type of error during the reading of Intensio-Obfuscator code
- [Remove] `simple` level of string generated for obfuscation is removed, previous parameter` hard` level obfuscation is used by default for level of strings generated for obfuscation now
- [Remove] parameter `-mlvl, --mixerlevel` to control obfuscation level of strings generated (`simple` by default or `hard`)

## 02-01-2020
- [Update] visibility of code with PEP 8 recommandation part : `maximum line length` 

## 01-28-2020
- [Upgrade] to version 1.0.8
- [Update] `-m, -mixerlevel` becomes `-mlen, --mixerlength` to control length of random strings generated
- [Update] redefine all colors without external library
- [Fix] issue # 14
- [Fix] issue # 28
- [Add] new paramter `-mlvl, --mixerlevel` to control obfuscation level of strings generated (`simple` by default or `hard`)
 
## 01-07-2020
- [upgrade] to version 1.0.7
- [update] spelling error (remove becomes delete)
- [update] name of class `Remove` to `Delete`
- [update] name of `intensio_remove.py` to `intensio_delete.py`
- [add] new feature to exclude file name of obfuscation #35
- [add] `Intensio-Obfuscator/intensio/exclude/file_name/exclude_file_name_by_user.txt` allow a user to exclude file name when the `replace file name [-rfn, --replacefilename]` is called

## 10-02-2019
- [upgrade] to version 1.0.6 
- [update] documentation Improvement 
- [update] improve visual quality of code
- [update] `replace string to string mixed` feature, better detect somes code cases
- [update] `padding script` feature, add 2 new random scripts
- [update] change path of `Intensio-Obfuscator/intensio/exclude/python/include_python_words.txt` to `Intensio-Obfuscator/intensio/exclude/string_to_string_mixed_feature/exclude_word.txt`
- [update] `exclude/string_to_string_mixed/exclude_words.txt`, adding several native python functions
- [update] improve check process in `replace string to string mixed` feature and `padding script` feature with `-v, --verbose` parameter is enable
- [update] `remove line space` feature is no longer called after each obfuscation function, henceforth now she is called only once at the beginning of the obfuscation process.
- [update] change `print()` function that write in all file with fileinput library by sys.stdout.write function, now no space line is added after end line
- [update] improve all regex that catch a specifique pattern in a file
- [fix] issue #20 - no answer of user
- [fix] issue #21 - updating `Remove comments` feature when she handle multiple quotes on one line and multiple lines \(I am waiting for the user to validate the fix\)
- [fix] issue #22
- [remove] `-c, --python` parameter, because is useless currently
- [remove] demo, `docs/examples/python_code_examples.md` is enough
- [remove] `Remove print function` feature, simpler action by the user herself
- [remove] `Intensio-Obfuscator/intensio/include/python/include_python_words.txt` file is now useless with improve caught words in `replace string to string mixed` feature
- [add] color and type of progress bar
- [add] `correction padding class` feature (check if class are empty after `remove comments` feature is executed and adding padding)
- [add] `correction padding function` feature (check if function are empty after `remove comments` feature is executed and adding padding)
- [add] verbosity mode into `remove pyc file` feature - `padding class` feature - `padding function` feature
- [add] check process in `replace file name` feature - `replace string to hex` feature - `padding class` feature - `padding function` feature and `remove pyc file` feature with `-v, --verbose` parameter
- [add] `Intensio-Obfuscator/releases/` to store all old version of project 

## 07-27-2019
- [upgrade] to version 1.0.5
- [update] Documentation Improvement 
- [update] color when tool Failed and Successful
- [update] renaming all parameters and functions
- [fix] issue #17
- [fix] issue #18
- [fix] issue #19
- [add] new feature `-rth, --replacetohex`, see README.md for more informations
- [add] new part of obfuscation `intermediate` in examples
- [add] new feature `-rfn, --replacefilesname` see README.md for more informations
- [add] new feature to trash all pyc files

## 07-01-2019
- [upgrade] to version 1.0.4
- [update] `-rc --rcomments`, this parameter is henceforth by executed default
- [update] `-m --mixer` to `-m --mixerlevel`
- [update] documentation Improvement
- [fix] issue #11 - Improvement of the handle and detect process to all features
- [remove] `docs/malfunctions.md` reference any known dysfunctions, is merged with `docs/recommendation.md`
- [add] an copy of Intensio-Obfuscator project at test obfuscation code #5
- [add] verbose mode `-v --verbose` #9

## 06-17-2019
- [ugrade] version 1.0.3
- [update] `-rm --remove` parameter to `-rc --rcomments` parameter to remove all comments
- [add] new feature `-rp --rprint` this parameter remove all print functions
- [add] `docs/recommendation.md` reference to all the best practices for using this tool
- [add] `docs/malfunctions.md`  reference any known dysfunctions
- [add] `docs/examples/python_example.md` to put all examples will follow shortly

## 06-15-2019
- [upgrade] version 1.0.2
- [update] Path change from `include_python_words.txt` path to `include/python/include_python_words.txt`
- [update] Path change from `exclude_python_words.txt` path to `include/python/exclude_python_words.txt`
- [update] Correcting spelling errors in `intensio_replace.py`, `intensio_obfuscation.py`, `intensio_padding.py`, `intensio_remove.py`
- [update] Improvement of the code by adding a better management of the display of the analyzed inputs/outputs and the variables/classes/functions found
- [remove] `-f --onfile` and `-d --multiplefiles` parameters, henceforth it is necessary to pointed a directory that containt files to obfuscate
- [add] a display tqdm bar progress  when  `-r --replace`, `-p --padding`, `-rm --remove` features are specified

## 06-07-2019
- [upgrade] version 1.0.1
- [update] one file example and multiple files example (larger project)
- [update] README.md file improvement
- [add] rules to replacement of variables - classes - functions
- [add] rules to padding random scripts 
- [add] `include_python_words.txt`
- [add] `exclude_python_words.txt`
- [add] Allow execute each obfuscation features separately

## 06-02-2019
- [upgrade] version 1.0.0
- [add] Repository created
