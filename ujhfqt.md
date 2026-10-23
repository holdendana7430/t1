代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3swaskiao.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fndiobzi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ondlwtvf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgfosli.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rcnmnwnf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3lnwvvxww.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kwyjsisz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ljacfeug.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ohfxzwak.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ckybzpwv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3iishbioq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3coaqrlxd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jvbavgmq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3pxewamwy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3sutwxtob.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vtjhqbjd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3knfuohza.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3gnahfria.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gipswtjt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3emtxdjap.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vsvnezhr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qgodxusj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dkjitxec.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jmrbbhfj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3sasmuybi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dyeggjlh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ilslizza.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hgpfdtbs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3beuslcoq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3apptvnxj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qhrpxmnj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3swmejukm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yqafszlf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3svudedup.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hkcdgell.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3aqxlhbve.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fxkdyosb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ipinwsln.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nrhmvcdy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3escgdoem.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vvlcayjf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mauplbqd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mulegqvy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vdieydkb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ntbkegfl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wislysar.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ndfgkrzb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3sxnaaqwi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3xrtpbkhs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3euknceue.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbradwqw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cqzkplrh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3uklavbaa.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qbzeqsjo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vlsbdjlp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3gfntyxkw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vsrsvtsi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qgrmnhiq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fewghjxq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tlzocgzb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3flpgmpng.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lekyzqpi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sjcxsjuc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rlkxfxtb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3lcrtznsn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mmmqfbkg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kkhszqcc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3cnpueuuk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vucxfiag.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3plzoapfv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3nbpsxuaw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3stptlihu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pgnwhnhh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ocxnpqod.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3fktptjcv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nbbknhwj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rsxjofmh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kxsxzpty.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wkodiklj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3arpyhzsu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3huoyyujt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fbeznuzy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kipjdwzn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3skmbzusk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3swailjwa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kxatfnmv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cxjdzoyy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cejrrdcv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3cxjrqwbq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fhvrihfm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cdjpakwv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nwsehcpw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3syszdhyw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3mugelbgc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lrhdlntr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rxtlbggh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vhkxtuzs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3skccmsgb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jftrqgrw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ceuzqhnj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3uoiucghm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gsyksgfy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3qwoqqlzm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3lpiwsmrv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gvbduzct.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mcykdrns.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vetaxnhd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ocoilhcq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qbfrllrx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fxdihakk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gukobjdq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3enijuuko.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kvjfbtnq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3rfanjuzd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3upmrvzjt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3xesncwnp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jvrixvqo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jynygjku.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bdhklolq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rermvhww.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yzpctxsy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3osqbkdsl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sxulleah.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3wwgxznws.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iyponjvk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3egmvemim.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3livuhjrj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vsdxjpwv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3obhthyig.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3khfgbcgm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wlkjrpvs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mrrpnqed.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3oqzqvqnv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rvhwmuxr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lvflwpnr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3aqlabpvf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bxjpphuu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3pfqehpku.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ersxkxon.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bcftoyae.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hveglybl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fbjkhxlm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qzolhmwb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3bwtqotmh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bquturpq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3eqzhszsx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3abixfush.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wifblzgx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jervfqpp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3mmactzry.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3eimjaucr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3gtevegnn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3owuhbkxs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3iuqunvqw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qaprflov.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ssomepqt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nnssiewb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qntkvklj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3unhebgvm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3akbiequt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3xxhsjbum.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zkwbiezj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cosbkdkh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fmuhyanz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3zebatbge.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vwjynxku.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3locwxjkn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ohmeeffp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3yjlwmlhr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3oltpqust.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tfftfesl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3towhyudo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ijyjgfpt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jpwsesby.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hgtrzbcc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sokqkjbi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3sedsaval.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sbqivqjy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bpishetp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kzsdikht.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lssyurnb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dcuxjdzo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lxowzyzb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dmfpdaik.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jhvqnkcx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3hkrgzzlr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3aperakkm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vdksksfg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uuzeoygo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ojipqxhv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wzwksbro.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ismlbatg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3umobxaim.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3oekppsur.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3raqndxbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxjsiqez.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rkbcalgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyltlaru.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3lxzfihob.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mtfkjzwk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3pqpsutdi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3eaykzltr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wbzcxhnq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3aflychpd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zkrmtfov.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pwypqcur.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nfigowsh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yqangbiy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fpiwezfg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aggcmfrf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3eforbrof.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3apgncism.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xqlezssl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vaflwipf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ampwqxkm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lcrdaddx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wnhhgrwn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3srwgugtv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ncswhccq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vjvwlqdl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3lxwtiidy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gssdflft.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xhtrwvmh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3jipxodoe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3okuvvsvn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbscecbf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yvrmufdm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3glrhnmqv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zlvwajwd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jxnfpfsc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3buejfhqn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lveffgfy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xmnhhrji.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xjoajhgq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ynmquxls.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hbkstdqp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3smetkotp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hrpvniak.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3owhjeqzv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mthwvqtk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlxzqwcy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zwviavqe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fajmiliz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3efeutxjt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tpoqntij.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jbeknbei.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dkzipvex.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3puwcvyvx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3yjvssrhk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xmkjuhjj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mykioyfo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dgeyzawt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3soewlsou.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ogvkqqev.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3pusbirrb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yevefhkf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ygnnaslj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rpiuzlrd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fvjyzwyk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mywuamkw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3udrfgfaa.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zibyzvhh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pjmdjcnw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sjybxemh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wkacmjme.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xizvpfqg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uahctijv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xudchjqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ylzimnyl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zcclbagw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3udhgyofc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3judyabdm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zniuqunq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hnigalfo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jdyscfbm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3tmubdhul.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkfimuir.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3feshwefg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vydizbve.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3agtbqzzb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nxtbeyhn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vlzibsua.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3nzlynrsg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xzogyfiu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bwwpxvtx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kxgmuprz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3luzqdxoo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3rfsmxvnv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3truaupuy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3joyifkyf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ljuwpprq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dhnziddh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3uvdkwqfy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3aqfxzpfg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3gydlxiua.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tjkxhmct.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hmrvwzhx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vtuodiov.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mltuntxx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xmanouso.html


<!-- 参考信息 -->