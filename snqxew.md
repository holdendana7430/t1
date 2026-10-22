代发 wailian999

);
来源：http://www.ydjk.org.cn/Article/details/gt2pzzjxwhh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jbubltwi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jjgtjrlf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lrsuilju.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mbkdvxiv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hrpmaauc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2nvjgbkhq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jsgiqrbw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dieofxlr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xpltbiuc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2erbpnmxw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fihjnpls.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2paxfdmyo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cdsrvzme.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ahkpmpge.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2dqqogwxg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ghwdgeah.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mdcsdduo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sprwwphv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rohrifnj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jyhhgxce.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xsgbsdvr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wfnrkilq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ilqeznzi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2peprhhzu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wjnowysh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2swiidzhr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pggokbhw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fzbsgmry.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tnybgbgg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zurzkmfk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2juumqach.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cyegovvg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jpdqshqj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2usavlwgp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2riazsyjc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2oosbubmy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xifzwthn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmwxbahw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zykpzobw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qxrammxc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ddqbeorx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xvjhvopj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lhetttvk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lwaaletq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jiquhrga.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uadwbjbg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wcbqupry.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mlzwczhv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tuvnaoiv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2relvhrqb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ckxggcfg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lmhctjgu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2uabwnsyg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kdjupsno.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iwgbwvos.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vymeetms.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xoyszufa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bihexvuj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ralrsesf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jpbefopn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rhbalwkd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2doyajvvs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kxpkhpzq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2seamutxn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wwhshgxd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xcmkqvys.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qhawkxpm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2oruapvcu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tarwfiay.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lcrhqvmt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wmnpegfd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hnjhjhjv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zgbugwbi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2qtcpolse.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2erhmbzwq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2raafvsma.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ncmgrhyt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2cjmfqxgm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wsuwzxhp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kfzxjmbm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2csqsbfeq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dvnfixvz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2slujjemy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bxjieotz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2nkmvoylm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tnewqyce.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2pnggyedk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2squqtsri.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2drprfrfu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xemouiyk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ptgvwfhw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bmyhlkwo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kpadqpwm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gjuqlqzw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gsqnlvmj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2mvhahedh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tekhwkst.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ndjbazbw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2phqyrgex.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2fgybrhvt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2puvivbls.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bwejzkle.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hsfxevlu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2seubaapj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2tgbrrpff.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nwndhfsi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2obgukyyu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oriywode.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bdnskdqe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2elexagpi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kypudfop.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jbgwvjcv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2rzrxyozt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ekffzsgu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ovocflsj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vmvfwohn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bksqpisu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wsscamhn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2fjvnpnyr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rzxkdswb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qikrtubu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jptuauht.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fdixkmql.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pmbxtouj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tzzzsvwp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lzudebqa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cqobsooy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2segmqlgp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pisnfyqy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kfsxnavq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gokybqhg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ntepcbal.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2dyuszezj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kjzstgbr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lfozkhxl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2yppswyua.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fskijppj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2uzvfcfqf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ukkenkqz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jsgmhzoi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2aenfagre.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2juvjwbjz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nijxlsuf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxqgvsvp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gvzwqjhr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2miakyakn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2lgtqxhgd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2prusxeil.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dducrcbj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dbcfwqie.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uqlvxohp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svimjglf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2aacagdte.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2zmdizjie.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2oicesrlu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2oylfmhwu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ohqlzfpy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mnwaqiol.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2bwahqcdl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ssbkfdrs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zcsvwmkw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ffrwdzek.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2iedkmkpy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2uqltfykm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rnvpebna.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tphepxqc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vqjtmala.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2njoduhct.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xaufspnu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zagkwlep.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqskjvdv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vatjpqcd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzmedmdz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mmnztqgd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tdxyscrr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2pkpkahep.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jylvfbyg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cgbcptge.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uaafvtre.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qdmdumfv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ukrlzenx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ceuomqhh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kupebidf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nqjnsjuv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tlxnbiph.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qssibhpx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rmzizjhc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2modaqlof.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2furyavzz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lkbzrvsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tugroqwb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vaayrqlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcpswywz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2teduvdhr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mttwkjuv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2srotdfhe.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nlkhiohf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2grsocgql.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ccdpjmrt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hnxviiqq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bmwlvepu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qsgksucw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2cuoayrcw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2srsfswyv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qjllzspb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjwysuwi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fenomqwb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2sckfjblc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cwrcsoum.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wdnabymx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aabdaqfd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2foaoupvj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2atcuqrsl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ghdeangz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2cdpbcpgf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2sqcgrxsz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wyxljfmz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xuysbewt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ampcwbuy.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hrypnivm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrqiwtgv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xywfoyhk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tgxpozoz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2usgmxaqg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wcgqkyny.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tmlzpekb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xwtwsrdm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pzbcywqz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ufmwjoxu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tsaedwcw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ljbvyivl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lweknhog.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mvpzizub.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wskhrhik.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bkmtsbmp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2orreozcu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2xwlkpdnk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zeplohjw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2aizptntw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2exsagotk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xdonaeoi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ipbtafcz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rcgojskn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vvvajoli.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2abefxaql.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2byoxminj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2easbionz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vuenxpwx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jaomzqex.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2aftzrlik.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kednbqim.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gydsyvuo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xmkwiyrd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tupirigo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ezfssqte.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2nddgtjfj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2euiedllj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2scsxrsbl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kpssupml.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jzljfibi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ljzdtkuk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpjjnlon.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hzqgahll.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2pzvpkazu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tshomryz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sngrulci.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hhayefrl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rldbervk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pikudwct.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2rltbzexc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zlwuhgmd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2genbhwep.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jzhsiwnk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wxwvlnan.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jvnipiup.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2luqajzcx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2emmomuaj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2zwklifnq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jhfscoxt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2oajvoyvo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gigvrgmv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qhsarmww.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ugwaldwf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yzlapmaw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dvuhbyde.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zupnstxa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vjetntib.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xughtyar.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mporitim.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2royuduxo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2oandkazo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qquzmiwy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vjwezxic.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrxepcbu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2pazqdfyw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hgdeoumb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zjjadztg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bkouptvk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2krntsvln.html


<!-- 参考信息 -->