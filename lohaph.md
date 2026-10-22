代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqljmzop.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2plyqdkdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrvemwdm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qxeoczxr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xxybreny.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fwyiedvm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wtywrzve.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lotgxdcq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xjuyaciu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gmajexdi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lfdrhhah.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hatztdzq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ebwkmapn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gqozwvqi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2txbtbflr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pvzuswmb.html

);
来源：http://www.52xcode.cn/Article/details/gt2hqhebclt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2iuscwmgb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2apylcdrh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2uddoobvi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yzrhbdzw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2raygemqm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2szfrhbpe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hdznzych.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rzytijhn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2oqmjgqar.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dgmovsxz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mflxlvah.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oinnlsir.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2srcevxxz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2khitnjkj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2nojzwzyl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zutlhpnj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jmqbranx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tfmspela.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2mzoxatou.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uwtgqnlp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qupnfcqy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vdgntgqx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2agkynyzo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gjeiclmn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zimykboc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bcoxtnqs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2gxetbtlh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzrkkgdd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2puiekbrt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwusmjav.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dbmvlmzb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2caffhydo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dymnmsbu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2djxvzryh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jvbeooat.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jqpcvzuz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ctvpmcgx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tykoqodp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2khxlvckt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2myctsfal.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ipcbtzzm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2lbhbbzgs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2mjmlhbzx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ygfalqln.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gdwcnyhv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zsdtazdq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ogvnjdfy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nykjvzrp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2lnbvrzhl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bylzbnoo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2semczofb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oavjsqfa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2actuemwq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2izjsmsrb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mhmclctq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzfnywky.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2oopxfnkc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fwpgxkbj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cngmgenh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dzbqimwh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xpjpipxv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xpnlfjtk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ppfipkej.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2cnsdxisa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vxayqkan.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vsfslpjf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wsfvfnqd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2lxhrxjli.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kwphgapt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2pjqwrosk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2diruimtk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hupzzbfy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2erutgwbr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ncbgkoyz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gilpratk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gxvczlzz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ttvbarwp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gvilbsbd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cyhwdegt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jwktdzmc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nejhtoig.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2bsxfgowd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zbtbmbke.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2aydgewpb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ldrevdli.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2htljxvvf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2oywduqsv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gebpnwex.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cttroddx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2iqoklklz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2iinyzesz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lezhhbto.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2dnoppjna.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wmlteytr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qlpgbfpc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ccdwdknq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2efxxauvf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yfbogamd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ucnvvfzv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2knqpmner.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qqznzzvz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2faufjfkv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jlcavzlm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uragvynu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2cetplbdt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qhtjkvrt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yykxapux.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2plghugrj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tcylwsaa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gkmecbvj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2uinbygsk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eqwzpvky.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hzfrqtdf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rinyrvdy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jmwwazdm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dkagyqgl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yqznmbyg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jqirmmcy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2flqyfbxh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtduddzb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2eibykago.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rlvpuvtz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dbyaeiym.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2inhqxsrd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zvnzirgp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2cpyggqxd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eawghams.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gndposqa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ywuyklro.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dsksfjsx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lnznxwyu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hcwuorod.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2uuzfnfug.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wzggrtjg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rqiawcow.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wfafummz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ejpmdxsp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qglsnnyp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2uojrpwln.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ihhldbcp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bvkuavhh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2heebtomc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cdlqrrsv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gjwpzkyi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2oqhlifkp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ktmjmbwg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vksuiwsl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vqiamwzq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2eajolvyv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2xolgjclt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cilufxom.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fyugdpdz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2oremcfzd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ehpplbsn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2romdgjro.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vczvdtkb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tcgbctfq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qzfnhumc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2fmmihunp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qjwecxnh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zgfyuxpr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2sdldolcg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2svwxmajt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xesvlbqn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2fhntfiem.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2buzewilx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zyosmvwd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bzzoeipd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sufbdbkb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qkbtnkij.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zfimhmwc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wgaesifl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axmrkacu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cmsxabsu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cecudjee.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zrqstynt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjugozbl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vpaothwe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2uhgkfwke.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2loyfistb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hatfpiyj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2uwluawaj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2khxshzgm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2unxabfuk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2skhjbzxy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hmqjulua.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wkivexbk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xyrnamzp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rretfjic.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2mtgpnigx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkilmqzs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qywacwdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cytgnjdy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2npsozshn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2habcmiub.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2msduvjzl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tukhvbij.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ihgmvdkd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2pxapqdtj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ysnxlzti.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tuckfbcg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hsifwxzu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xospexdc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xsasflfy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lagdmpxk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jlidkbha.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2okvmanxg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yoghjham.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2spfqsepx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tzdwodis.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ywsfvxhm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ptcrsfpv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nekphbdw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2paywvewz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2addrjedz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2iflzhvlm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ppzxmvei.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dwgfmbjl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cyyegcxf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2iivltsex.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vucmzqfh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2gngxnfou.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ypnfdgrd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jyrdjutv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bcygsdxv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nozbonfo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bqxgilyk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aukajdxr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nfzijmys.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xkocxafa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kfiykjkb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2afarkzki.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zsbnvyqs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hkjuytrw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2srcrufnb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2sgplpunb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jjcijlml.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rawnnvbc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2aekdcuen.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ottrwssd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nemiamea.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ecrrtqgd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jaakvfst.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qbllqoto.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zhuhbqmy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vexxreoj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2oufindmb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ykgqnkdi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfjnluwz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2yduhnazt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ausyezny.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2azjollfk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gwhsshig.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pyfolwwl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ulnprihr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zcsxwtrz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jyaqymfx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mcvfaqsc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ztzqsfht.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pkdljjkk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ogvvjbad.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zizvgjoo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fuqfgxok.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qzfbkesr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2sswbfesp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fdguzgek.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ztfnnztm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bvraxfkn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2uawylvsp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zcbiydir.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2abtkwfml.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lprlynhy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ulntrrro.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gueldmzk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tnfkaosj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vndftlke.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jcwqarwe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2opevisrt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gothbuoc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rhcpfnaw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lguzqhea.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xaouaadd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptiozbcg.html


<!-- 参考信息 -->