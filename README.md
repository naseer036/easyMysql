# easyMysql
why write queries again and again when you can let your system remember them.
phase-1
#commands

#sq store the previously ran query
#s store current query in register
#. show query in register
#; execute the query in register

##Main Menu
#1. query mode
#2. execute stores query
#3. show stored query
#4. show previous queries ran
#5. search queries

phase-2
#run command 
	#1. show -> c1
	#2. desc -> c2
	#3. select -> c3
	#4. like -> c4
	#5. use -> c5#c database command menus
#e execute the current command and display output
#@columnName use previous result column position/name
##rowNumber use previous result row position

expected output for phase-2
# example query 
-> select tabid,name from vtiger_tab;
# select  c-2 e 'vtiger_tab' 	// c-2 e 'vtiger_tab' describes the table specified and displays the output. the out put can be used in the current query
# select 			//notice that the select is retained and the execute command is removed, so that the current query can be continued.

# 		+----------------------------+--------------+------+-----+---------+-------+
# 		| Field                      | Type         | Null | Key | Default | Extra |
# 		+----------------------------+--------------+------+-----+---------+-------+
# 	1	| tabid                      | int(19)      | NO   | PRI | 0       |       |
# 	2	| name                       | varchar(100) | NO   | UNI | NULL    |       |
# 	3	| presence                   | int(19)      | NO   |     | 1       |       |
# 	4	| tabsequence                | int(10)      | YES  |     | NULL    |       |
# 	5	| tablabel                   | varchar(100) | YES  |     | NULL    |       |
# 	6	| modifiedby                 | int(19)      | YES  | MUL | NULL    |       |
# 	7	| modifiedtime               | int(19)      | YES  |     | NULL    |       |
# 	8	| customized                 | int(19)      | YES  |     | NULL    |       |
# 	9	| ownedby                    | int(19)      | YES  |     | NULL    |       |
# 	10	| isentitytype               | int(11)      | NO   |     | 1       |       |
# 	11	| version                    | varchar(10)  | YES  |     | NULL    |       |
# 	12	| parent                     | varchar(30)  | YES  |     | NULL    |       |
# 	13	| source                     | varchar(255) | YES  |     | NULL    |       |
# 	14	| trial                      | int(1)       | NO   |     | 0       |       |
# 	15	| extnstore                  | int(1)       | NO   |     | 0       |       |
# 	16	| issyncable                 | tinyint(1)   | YES  |     | 0       |       |
# 	17	| allowduplicates            | tinyint(1)   | YES  |     | 1       |       |
# 	18	| sync_action_for_duplicates | int(1)       | YES  |     | 1       |       |
# 	19	| duplicate_condition        | varchar(5)   | YES  |     | all     |       |
# 		+----------------------------+--------------+------+-----+---------+-------+
# select @1#1			//@1#1 gets the first column, first row value and insert's it there
# select tabid,@1#2		//@1#2 gets the first column, second rwo value and insets it in place of the command
# select tabid,name from vtiger_tab
# select tabid,name from vtiger_tab
