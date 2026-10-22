代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tyfbiwpo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wfftywaq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zunyqzyz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cwwixzzo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ybidoazj.html

);
来源：http://www.52xcode.cn/Article/details/gt2yvppqcif.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2thgkaqmn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2yzfatuti.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2brnamqfr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2trrcaryg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xrlpddvk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pswqlwaa.html

);
来源：http://www.52xcode.cn/Article/details/gt2ynnyfwts.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2amgyzosh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ecpzubnk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cydthejx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nhryzptv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2xrydtwii.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kcbrseyo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2nuaphmbv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2bembvugt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2sjuofwsn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pxuuwzlq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xtqzdonm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lpglnsvx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2sxvdyhnp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tusyyscz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2beeorayh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2beeorpdk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2racoghcs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yppgazux.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2smfhaqdm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pzqltybj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2rempdvud.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2stzjjdht.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sglwnhby.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2skydxgce.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pjupcdxa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zjpnaydb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dyfkjtlp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dtfevrhk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dszssszp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yddxmhww.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2oxajylok.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wflvgkgl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tlhpvhvn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bipnjcsk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2uauxriin.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2kpamatui.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ayajvhzc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fdurjjju.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tlfyceqj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2njkhbytz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bbjahaui.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zcytkjoz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2scltzxpr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2yviurjlq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mxieccde.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rpsnbcxx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ojwnsjkk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2efpziguo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2pgourhdy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jmijqheq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kzwdeeaf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rjsvupzg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2cwzfdbdg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jznmaytt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2crnvkbeh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vdkypzqq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xsgvtrqi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2alxremph.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gsexqvxy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qkakqrdp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wsmivsgj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fqggjtbh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2shpzoyhd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ginacdwj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2knrmwfae.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xmckcljh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hfzugsov.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2snqpeguq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2btrimwpj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2uichfvjt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kakesquj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ghukxrqw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2awrvbbma.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hzgdrnpd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lnpqfkzc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pxmvwjnh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yhvnrrrk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2oaxxgaii.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ildfxbru.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wjwydgag.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mdygwyhe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lgbprekb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zrwycdcx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2edbntmxb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rbzgwnvv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2flxdwxat.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cemvtjhy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2aysqhule.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2obpfugik.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2afniyksn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2pfpiwxvy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dewjzjsw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jvqxlpzv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2adgfpgwp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2exyexhgr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2buydnqle.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kvnefnqu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2demvlyme.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hvbayfbf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qwujorlt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zplsdcff.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gjjhtakb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gzoksliq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zcgdwwnl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qnevurzm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jgnxhtxr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2lltmkbxt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2njzmugna.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2chpdewso.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cnpevelu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rgmhgcrw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bulriswu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2oejdbwcv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2llpvqakc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ojbnnjbp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iqezvyfu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2oavmivpa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kwzcexwq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2pnnoettn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alehryxi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2oyhadagt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tlqaajti.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wjuiltot.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rrhwbhjn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rmkxxwnt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wcslmukw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xiajyvwx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ctiyqany.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rczmdeop.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2sozgahia.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gjecrwdw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2eqngwrqx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qedkuccg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xgmypkiz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wjgtyqps.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zlmvgqtr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2akkjaazf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2smwokcmq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2yednonee.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2kqxrerjl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2egvjmrbf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pjmwdeof.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2afofvxvr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ybdduxlb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qptncqxj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qicdqixs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wpzxftgn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xznsrhbx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kmxdvhap.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vgpwsono.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wpclbyri.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jocqxufc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2rgnfaldg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2btmjgncq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rswrhxgc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nvnrnexr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2blmaqztj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2khtnswdy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ndzmyaya.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wjfjajvj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2obijazdm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dsdftzmg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2eandnjac.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ylcmjpdp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kqscxstq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wcjfkuiv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2cfnbvdtl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ujqwhjhy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ruzaumnt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cxvvwuye.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jgrgrltm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fgqnaoyo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jjptaeur.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fxhgdebo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kmffymkx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2sxujqygw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oldqbtku.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2aunluwcu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2thkuisyq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ofeatzpo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zluvvzvc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ddebgaid.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2glgqtrhn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bnmtcvtv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bmtilxyb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krbozxrr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2cmggqydu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kqjvbmar.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bgawhmnv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2yafoyldn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enfawxnp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vkzfgcrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erjcczan.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jmettrcc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rtgucbyd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2osmkwwsn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2tdmaeejd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jereiubn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2udjhhiwp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2xhrfsfsx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2awzsbbak.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2abxqachh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2immqiixc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vstkgokz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jfvwjzzy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuowbdnt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2awyewgpe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ybusmhrs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kualnmqd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qkleokel.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nvljimps.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2knqvramd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2adwzvwqr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2chiuevqg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2akuvbvtp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yqbzdcev.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yhdckail.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gruprnlo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xxuyzlau.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vsehqpsg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsljzfie.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jcogoymq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kfghvnjy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jefxrana.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lmqzsqai.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fyhrkhak.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bhsgmiza.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jxwsedjk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mprqubaw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2acscmfcn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2fayzqjod.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sczrddtt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rsuuazsn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fzbiozjy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ditieggn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uuquqkgv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2akegkhka.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2tywylqqy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2owcvcvtf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lgbpdttq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ujzrfqto.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nxulnfnz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2latwmzqp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pbhjhudm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xhfvorek.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hoghlrix.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cfzbojqx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vbznnkdg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bpgnkxaz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jaotlkjd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ycynsqjx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2udknweun.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ckqjolto.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ivpnpfqy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tkbdwymp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2shhnliyr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2uwnvobmf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hhdsuazn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jljdihtr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfcncaij.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2yskszxfz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfwsaldk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vemtgzle.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qqenmyhg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2agrglgvc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pwemslcx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rkkynniy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xtxeeeiw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2isqipeuj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2iugxhdbw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2dbbvwkvi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nhvsxrdz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ddewrcsk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xqeyjppz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zdanmgju.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gnjwzrgn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zqlikvte.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kmgzxhal.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pydrthjr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cqksybou.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wyqpksdi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ficyrtua.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gmgddfpd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vtaridls.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2sxatjbrp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hndfvltu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jgthkygb.html


<!-- 参考信息 -->