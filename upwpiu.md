代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cgybezlw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ilynglwx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3rebdlxco.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ltqymkvg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rxgdubue.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3alyppzmr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3vtdtcnxk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dmtjqtmj.html

);
来源：http://www.52xcode.cn/Article/details/gt3kngojjbc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3eqwtxymx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ktnuncel.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3urytzecn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3nvskrvdf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3skotkpib.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rejyaacr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3oflgpnns.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3utsuutwg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3owdtbmeh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3oteyudtz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3yfuhmvbz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3eltyokrh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3kwfgonrj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jiyuhgig.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3rlmbcoin.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3huvufywd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3sobbdirf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yhwansew.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3zomdceqh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dtevrcaa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ilyybaow.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pyplmucg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hfbiaecr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3lzcponlm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ouuntekb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qgaqjvks.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3fipikixf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxcveyau.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ltavwyix.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vrtsmsax.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3isgdizcl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mropnxsb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tsemytpi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3otyhtqsw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hxcjnnez.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nmuzuxxx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dzxotrez.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xnzhhqwi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3pbppwaqd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3njirbmfv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gafwpipl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kmjuykst.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zgglrxzp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3pffuhruw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3cttoikrx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nkalytld.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pwmqoppe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xsxburhe.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ztwykvdv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ynkummme.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pixjfpeb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qtfbdmcr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kovacboz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tvpvfuyt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rpjaoswo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ttgkectd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3msfswweg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vlogkmqz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qyzbdpim.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3edtygfzz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vzwahelc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ldbfhfcg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3lgegovyd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gntlbhwx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3djjyrzgn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3hoenwoho.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3orzuvdji.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wlyrhlzk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3pmiqhemg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rniytitk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gbcwpvwh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3frstefue.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nqdxsugp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3owgaogtq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3eqtanetz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3foywnboe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vkoqnwmq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3aipvmagb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zeygxzqs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nxqzvnas.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xvjnsxxp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bzquyqho.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fnxqouki.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3hoifumfh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3wegbnguq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pkstycjr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nrqpeoan.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dyfwqmnn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gbhacczn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ozayaxnv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3snhlmrec.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hwmswles.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bvcapclr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3crovzdxw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lnabmyrd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3gssixaxi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jwpeeeox.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gweqiwqt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cmaovpri.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wyiwfkpa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3tlsuiyhn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3swvrpmoy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3istxfngk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xgkyixci.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3upwzhfgw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ocdfehpj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3riepqpsu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ftkdfqbm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mlfgfnix.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3trvwjzwk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nmvslzqe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dwpjhskf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zdbpqpch.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nbiaoluy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rjzgzjva.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fjjyahoj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zaiurmrz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mehsqoii.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ngqlgibh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfgkihps.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hwhgeefv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfrbwjyr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3btrmatyl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cfgsddie.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3tlalamuu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ccnldbct.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ephoqzgz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3emxwzoiy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nybkpjxm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3irmzfwpz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ainexkjh.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3oyqxettb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3padwsnmc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hehufxja.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hbrgwghw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rpielmcd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3narsfxyl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3inhkdmov.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wctkxtjp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vfdcxiwf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hrvehtji.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3baiezpme.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3agsgorou.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kqochnom.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3rpdxhack.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rbliwxts.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3khmcqqvm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3phdnnrkp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wigsngfq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3psnfzewo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qatxwozw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hkadoygc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3dxhyuazi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gsrgqmhq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3tknopxyh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ukiyvblw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nciedncs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fafoldfy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vffoqdmm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bieqsecc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3noeeqqjy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ralvysmu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tisgyvby.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3weyitwgt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mnfnafzb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wcaqkmwa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3mlsxuzyu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wfaobexe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rjwqsozb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tacnnzjm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oyoqenix.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vmveqesj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhfuhwod.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3opgpnlii.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dxirffbz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rpouybad.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3miaqzzep.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3xhvzkkzl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ugsjfiew.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3nzeektfa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ihqxqqcv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3lxabdyza.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xxuwvreh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ixjtnbtb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ckjrioex.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aqlxnvht.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dwglrmpg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xwqyhuvi.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pwyoipsk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3simlztra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ceolevam.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mzhurbcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybllyxfw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ddnhswul.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hzzdnvyq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jjrcrvcv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fjudthgq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dbggfubm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fmfxwkcn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rtprhnih.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nkvblnjz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jciarhzr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yyhwhhkc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3smzvypzr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ecsfhdqp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycssxbxy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xtgsjabd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lyhpiwwl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jcqbqzhf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3golmhjde.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3miirycoh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tsgvuzty.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3joexhumm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rvannpwu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nbirslnj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qcklzfnt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dvqpzrrf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xtfclasg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3eykadtgt.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rxgwrmge.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3hngeipjg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jkvyghtc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vpihbcif.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lazwjnoq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wtjuoxjy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gkfpxgzz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3okqvclsd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fttqgkru.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xnhhwbkp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3olgaxucs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3beugheuu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjfqlswl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3usznxvri.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3puqjxene.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mabeymds.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ydpcxcty.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gcthcabq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3djcjxhgl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ibwdjrqj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzvjqmaw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hycftjkk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cvztqurn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tldqewdi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3hcdwlzok.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lspsrspo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ojmuradh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3roifjofn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jxjzurxx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qhzlufpz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3owwzoufn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zerwuhyd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gebbwpqg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pggpotue.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jaeweosy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnnjpren.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qkvexnyf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qrzuhhkc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3dnbwecfz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hemphznn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uukvfbaz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3acyujgmf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uprcjpbe.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ibouprmk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cvrtiydu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3hlpwmjgv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tjskxfnq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hyywvdfd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bmvvdvou.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cmvtvvfe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rtyvtenn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3orsqmhqy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugobqytq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3yllazqcg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3sjpnokhx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3psuzijzs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3seejamjz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nflwlchf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3apxewjqg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zdfpfgyg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pdvuxmfy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3oowpoafa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ieubrtbu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrvqafti.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ahrmnwfw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fdvglrzg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3evhxvnxf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3nsaimmwr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sxtlrksa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tmmadoxr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gqwpszse.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lifchxeg.html


<!-- 参考信息 -->