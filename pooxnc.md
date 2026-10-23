代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gkditbzw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fhkkqvou.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tpzzhhpn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mphqctlo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fqrvjxvq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mkezzxwf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3emozbbfe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vufluups.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gsqvfeni.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vbrqxqnu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nhqjzvsa.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qwvvhuqx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fabczwoi.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hctwjpml.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ahhcokry.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bvhtsvwb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3elsebhie.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xvloweut.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bmhjuvvw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3fvjhrlco.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3elsuszfo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hpuibxzt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lzhduerk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3rzxibsdh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ncxnqild.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rscwddlk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xsjqwkfi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lronibbl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ugttghul.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3dlgmsbqq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fftrkvgm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lvymcotm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vuiikwka.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3erazouhf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgatweoo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zjhbzjol.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wojtypfu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3nahvozcf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rxprdvif.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3efhneogg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bntuwfjz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3eihhmhyg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pwnuihpz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jzwbugxx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hcsfuwhu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3fbfqtmgi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3igkcxvna.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yqmvlpdu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ijsugzty.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ectkfsrv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3efqwukva.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3quhuyqlz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hfvhshkl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bgxbdlpq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ofosatom.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lngczvdk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iybdwdyc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cltqsacl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wyyozhpi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pvhiympv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nperrrad.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cowutunt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lclkeprw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zmbljcim.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3sanjgeom.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gtkijpml.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xntukzzt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3rofoiwzo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lpbxjaza.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iegwnizg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3odgudxsy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mwklumdx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3grzuexim.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mfhkybfr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kndpvukn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nraykbci.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tpfnhdkq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3shfkeyri.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pxpzspuy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3shomogua.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3humistqt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kvnczcwx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rhmstwze.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3innencuv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hzficxnu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3apgvznvx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3scjryfah.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3yueduwfz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wbtfhyle.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ffmyoean.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mqlziatt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kvzevmvh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3gnlopgqq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hfwtfguw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3joksmydh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vvhqjgeg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ujntnfgc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mfhblyhq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mcozswqg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pdbdhjow.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ihvjjehc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3llldshwt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3dqkjbqkt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kmyeakym.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tfknuxma.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rmbznxth.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3extxerdj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lnzjwasw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pqsegmpz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3fnmdwanz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kczdjzyw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3amshefhs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3snukmurt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wjbsdvfk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ugxqgpxn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fqcllltl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lbnurnzf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bkpdsvop.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wvvbfyzv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hqsxnwyy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oenhafrs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3focwpxse.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3uvdannyj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wfiknvma.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nacoigcn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fwnsmtrv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lqxbtkkt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3flcxozis.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mbtfvfyk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zzildmut.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3jtwlhjpe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3swlccjts.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xonlzyvt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ukbrljea.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ftarszoj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yubvvmgk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nyxidkik.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gqkjlehs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3nnhejfyy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bmhlqqoj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xudercde.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ypkiafrj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3imgzomxi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3cixspkay.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3leeqiobn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3aymcvaso.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3etowiyaf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fncdauvo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dspuevja.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3abfcvbzg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kgarcjeo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3dudzenlk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ryrvrtaf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vgipizaf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rnkzzuit.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zxzxiqvu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3alsbqmtv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wziakgob.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yjvgzawi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dcdnvevd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yxlwmpgh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fjfhvtky.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ipsficpj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3odpoamtw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3yeaiebtm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jnpfrsra.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3niksjjky.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ehsrzmdi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jytdxvom.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ctcjeslb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gzlqlejw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3klvaiurd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jbmnebqz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvypzdvh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lghjnlhg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ygrekmxs.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xqchyvbr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mxwcmnvx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ngzggxeu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aknngkxt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3cmatrpky.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mxbliolu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3jdbiahux.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yznpocuw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qryasspi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fpjoeckj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3blqbgifb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kcivayyo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3pnskbznd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3sxlctkua.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ghmnvizt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3eswvqesi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ynugnqzj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zqnpixhd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dfweaxtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwwkjpbq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hlpbmjjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myrzdwcf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rrnillmc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3adpnpyha.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qpolywsf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kybtgbgd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mslpsuxm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3joryhoyp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3dbdejkpg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3stsxdsua.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qgvbezgb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wsfuefyp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mimbzthn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mgxezrvx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3njkhdwzg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqyvjejl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jcpnsxos.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tacxjixu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3riwhzcej.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lkfuvfjv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lvgpxqen.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3djrnzdqx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lasbldnu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3iywvpvti.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tvwfhskt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3bvprpwbx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ivmoqdaz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rtdzpufr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xegwvmxl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xgrmgfth.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3efdipccg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rppxqnhe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oyqxgwlt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3sqjecczv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hesznmtk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3enfwwowm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iohxrfqm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gaikxjud.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uqepffuw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3advrrewp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3trhgiwpc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rpdpkxcw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ixsuirap.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3akspqdfn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xuuukakq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ppgvubgh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhwwygil.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vtnzxeyw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3yxckracl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bgbztecj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bkrvafaq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tlvzofjl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bmglpbdf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eygvptwn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3juqhudvh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ojvjfizt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3snlnncau.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xgjopnvn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3uenroclz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rsodfjxm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3bnamrrwv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3unsmhsaw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3evkjqacr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lwicrbjs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3sjcfkzhv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mtibohnh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uhknlnqd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xwlmkrvp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaysooup.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vudfrots.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qmvskyfo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kjxuajqa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xwwbjiij.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3kurhscyy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rssnmrrd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ccbnzbty.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tdfpfwxv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xthlnvob.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nkbbrnxk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wqympliz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ychycggg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qfrufgyl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vtpgfpol.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mbnbraij.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sqorggcj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3yyzejpxs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3tpurstlr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hediaahk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wvobsuyz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vvutkcas.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bknhzelb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rgszmwnl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fzfawetq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3luhbnyph.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dbahvepv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3irirymoy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3njhahwxx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3disrqswp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3odgdaxur.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3grwlvykv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dlrjzfzr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mjemhonh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wgiknbvq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xzwhftan.html


<!-- 参考信息 -->