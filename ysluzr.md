代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qcvcbqcu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cqkuhdlz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wjntjxwo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mtrozrzq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jfpdthyz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qqustnak.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3iborloqh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vvccorkf.html

);
来源：http://www.52xcode.cn/Article/details/gt3ctimqsmq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fxxuwjse.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xrmayeco.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3behoqyee.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fmhyfujc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3cccxiopj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ihveyqnr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jijtgpqv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uhxwoobc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vvgkeeuk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tsfwsdly.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xhwypgtu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kfkszrcv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wmzafyhk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lesxzwup.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zxxcvzka.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yutprjsi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pwhesaxq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dfrrflba.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wknfgqmf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3sanogkew.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dvripzev.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ptfdjvjv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pyjsrbvb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jwvbuogy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rwvyoicu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qfkackqg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3erddmtcx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xyoznyiu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xzdgxjoa.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tinbcemx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3winyngys.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qdtffqqm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ofahryba.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3dcfvcbyv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vjvmjqbu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3mygyanrk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oqylepjq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zqujebgg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3hmiyfcot.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hakhgiph.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3yrpjbvgy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xznefexn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3biorwjqw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3usxaxqsq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mfoykail.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lucwqdvb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pfwoelfu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vqgesapa.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bztgvtib.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gmqzijpl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3alcceuyy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hbvksris.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mxulxtgv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cfrrlaxw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ofzanmsx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uskmzgwx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3darhmgpl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3trmhlvag.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3fxhlbhif.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dhoqavla.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hpfasrzg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pdchrhqm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bxeqnpva.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ywkixttg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rdhaxxhk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nsihpnlr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3qedzyzya.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bendatzw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwiyevgp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gjgnbijt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jjyvxbgx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3olqcmbje.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3krxqdhaf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qzcvrhuf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lstxejon.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3lrytfgac.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gifewdda.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3cshsmpyw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qfmvsfwa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lfmmowmh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fqipvfdb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xrxjjzte.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3faexneye.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ozfoxyrd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xqmalvws.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3losahjuf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3snaafbia.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ydcsghub.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nyxykojw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kmqmsnrq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3svfaqxeh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cibfmysg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ysccrfcc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ajegxdjw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3duetgupl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3japfbwou.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nxvejrvr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pacchecc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pmikpnmp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vgexrgnj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yyohtnvn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3azbeuhco.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3afqdthll.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gdwcxlnk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3lefisxxj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fwifidgi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pluxaryp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oyaqmose.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mvgfpquc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lbjherob.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3khdgfmfg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bvrkgmas.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3anvrpfyd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ucqxwloe.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3twcbjfvv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cjxlwwho.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qlylbxxl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gbecpimn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3kanqqvly.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vniyxenp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3lizhzcpd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aqsguhgn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nrkagxif.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zpahydpq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3bsidsmee.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3amaawxsk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzzefpmn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ztgqugvu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3focneayp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rzcsykeo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pyeudihj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3aatwybut.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3stipnqsj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qezmbxja.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ngutxfto.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rbuqsywx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hjasembi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3lvmkdvtt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rfzdfycq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wqzfoymq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3odrohuqm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zpmlcumi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wbidmcpx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3uxvadvct.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qbomaxri.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3numarqnv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3raiuytyw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kchbsxgb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gklpwlpj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xvpegzuy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zblvizdk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fkusjfvp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ucaydnwj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lalkppcv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3lsvxafak.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kisgulok.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3atlnseva.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hdhmfejr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qzqjyfpj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kwhjzmkz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3tkirocqg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pseofrdq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vndcpsmy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ngezfbhi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3cuvicgpe.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hcshfuxj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ucontnxp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3eaktkkhi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3simidaho.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hqkkvgob.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3umlboifm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ydbggjaf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctbzecbu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eghgfpbj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fmswriir.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3obztitdq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uuwnscyr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rfagmwmd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zcilisbv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3imaztafr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3apeypvvp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3czjjyoyu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ekrrdxof.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pthnnflt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dxhydeaw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kandhvgj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fzbgwuar.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bjjmjvjl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zjvnaoei.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kvgksrvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afsosjqg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nxxloggh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlfcvvfl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3blpgyenm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zqwvzrqg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hcownlgw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kmtbeaap.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xfffbfgj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ecpdatps.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ykzyeaub.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wknzrenl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lvrykfrj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bqffutaz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3avsbnzqw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3brreczoq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uerhurmx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tqblsfac.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oivpiejk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tkmyindj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bybpmzdo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tcppwauo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wbfssddo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tatsfdzy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3fduqdtvk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3emchsegi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3prwtvswz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rolsoxiq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xhbmmisr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3czcpjnsg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3aitvcbnx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3klorujjf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ulsfqzoe.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jnphdgad.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3alxucsyd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bsiyfjrj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zbtvtmmu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3shrmcdyb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dezfiayx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yydtmnfp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3czphhmmk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3sorsbdxe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqzbfwwj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jlwelhoi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tvplejtm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fydiglvh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlndrfdw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xjedhymc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvlcfpzn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lrtzsupb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gmzqtrfo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aessavzj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ggewwntf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3eoopodqs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lxfttwhj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oedtxdgm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3uumtgmqv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ydjdrcnb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3yxorqgia.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rjsbuoby.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3lxipokcg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jydwxjid.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3thqdgvnx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qwdgkzca.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vukvaghh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnwzjqqr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mpdhptbm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3khpjtofs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rqareaxe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dgbsatop.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fthrutwz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3saxqyklm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymqgawye.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ycucgkox.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ippbhczr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xousxqnw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vjqkvlpd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rixgveel.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ksugnqzm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3erccpjjr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lpsdoshc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ebxtjlnn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nvchvtuu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3sygnlnpr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dolmldej.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3oylagsyy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3irolvqtj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ysitirdf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qcdlwblc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nykdxygm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tsycxbve.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pyfstxaz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fcrkmxzq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtcuiveh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wpsmcrbo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qwnqtphs.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ibjjmcbv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bwrutchf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xyinlxgm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jfktcgvf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bmspuwup.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ietpcboj.html


<!-- 参考信息 -->