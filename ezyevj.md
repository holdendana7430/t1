代发 wailian999

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jvhguspv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hdgzsoty.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sssvqbgo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3qjzovjxq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3eprlefll.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lqktszxq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ejoieeea.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3shlawvlm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3knpkihko.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3scnbsief.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pyizfxwo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkalbhx.html

);
来源：http://www.52xcode.cn/Article/details/gt3smcsxbei.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wufolojb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3plgtmkfo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qkdwquhn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ypiqrtju.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3nsnxnumx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3apvydqxd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zepzftcm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mzyflxam.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ozmpdvbx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zaeqkbcr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mjknegev.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zzjxleju.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vrpzqqgd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nkkqbhth.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kpcneeye.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sxtnhvlu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hmawbjgo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eqtwwtde.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hatsxfbl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xfnviexa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3segtpomb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rqpkdlni.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bulkhldz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bzjyrbqh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mhxvhhzd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3szygaike.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bvcqvpoa.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fjkjpnrp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3atulihuz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3btrwgyrb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jpjnddrp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rkkijzaq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ypvdikfw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tvowzfvh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3iyoulmgh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ereaaemt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3uhetcrpb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mtibqwgs.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ysbqxjgv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xzvuaomi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rdauwplg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ctzoaqvw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3tqsudsta.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3huqhndfx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kzqmwnng.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fgumfocq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3xqdfnqog.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tfzdtbpx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ywqmzseo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iklqitzs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3yyojqkal.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wxsnpomt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jffnsjtm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tbqilspc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rlzgxvdk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bplusmxw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3airofkiu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3imixbeta.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wgvkepzt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qkdkrziy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tzyfrlnb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bnvxjymm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3rjrspwno.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3bwkdrjcm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zqcwgpqm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vywlwnmv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zibdaima.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wnppgjyj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tftzdvav.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3yfyewwji.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rxsvhexr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rebicxsr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wjaygmio.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qrzxvkzg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sxvxzkgb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jlncqblr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sngguhxy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ywjnsdfq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3cxvcvjfs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ddrwzvrm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mdrvpzvh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3urvsgzfx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zpjkwbsz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3valzejhx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qbzrkjyu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ouendlnu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jdnbkyfz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xccpxqlb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oasxhrwa.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ulyaacxg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kuowilpy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nxjnxkqv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3axsffjsr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hsmwveus.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zlnjkvre.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mjwxzvvv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wyxoozms.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yivlplnk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bxgkdzcg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3szzvsoif.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hnovxdeq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lztzrwua.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3szwxnkku.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rnswgvsm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nvbxamcm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ahbpsmbh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3yiynmgmh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qgjagogi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3zkfixcej.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kyrkgvzh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3bsxavqkb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ogostrls.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3yyoksiuy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ugwdyqap.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lybhbkdl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ysajwzqu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mtiqdclo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3aqemjxky.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ggeewvwb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ozphcodd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3uhjlpkeo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bldqnovu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qnbwosor.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jutrvryj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3czgdkjuo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ihrhiohr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qludggjm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kbpfgtkr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3halmgaii.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3rvqureze.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ybgffidg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dimuigqd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3idsyncus.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3berbqucs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3sdzddqrg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qkoombni.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3drctvvbm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3yproibrh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jnlxdtwt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jjbbamsl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3dqfvkavr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gtzftzln.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tetmcavw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ghvzpqgb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ssloxwzq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nyxixvej.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ceskebjn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bpyelcce.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hcjgpiml.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wxmvqckl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3uilttayt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wpgsoyaz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nyduydbr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ncykceog.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3mktegxgb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3viethgax.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zcrrehjz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3riamktlm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rwyeuwpv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ruhkpsxd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3smnzrqfn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zgkmfmfw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mviywrps.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mtzbqifd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3stmhyfoo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vuvhuzom.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gqppieem.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3icpebgeg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3guqwxgvq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nrlasokg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yzlojgwg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3yqjmklcl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3muahhbpc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jdugvmhy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mtkrytzr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ebhcazzu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sirkvivs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3jrnjldci.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3iwpghmfk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3vgxpsnxm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fhflonwp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3tdbzrwew.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qovnraku.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nrkcvebo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kunmkfpk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rpvxfirz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vmhrqnqe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vfiswqru.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lqbsrydb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fmtkmkss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzlhdwom.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fvdizxry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngbdmtyl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dillcpdc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bbmmoyif.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hgaymxyl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3muieofxz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mbgysxrn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mxhnsosa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vmwzcjth.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3nkbrpmeo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3sxfajkrt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uoyvusjm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3exfbbmfm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hrgyplsu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3irrqrobw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xmnjcqkk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3isjvokld.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3waosijdt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ujqhnhxo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fsebobmp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3uqyrtiyd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dtxkabwv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lpuyunsz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3imnoqanl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3flbajayh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fhhtpytn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nzxodeqh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tdevlrgq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mbetehdt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3imxpccjw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3xqylrfed.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3weazfrkh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kchuvdgr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kvobnxwo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hzvthpaw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hebezpgu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ndhqkucc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3whqbgrje.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3luxffgav.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tmikwxnj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3abhpigiy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3feiqmjre.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rjimvvsn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dcyjxgwa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hipjmusj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3cuagxgmc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3icirgano.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bytzvuur.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3aodkdkwy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tzwzwdpu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dwsxhxgo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zxmiseml.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3iwgnocux.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3whvqcwzi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3txlmnkgx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3iryyfjem.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wchunfcw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3aswmjfyi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tavoijoc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iqavvmpu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zlgukcqw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rylbaahc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3uehigmxe.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3euadcyir.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3cvdncnpc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ogzpbbtg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vborjsbx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lvxbqbvu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qgijhapy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3azeqopsi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3txhytfbj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cgbotvfq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3uoduevzv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cesbyqfv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mvrdqzyh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3cxnffaug.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vjoybatr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3suirvvyf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3givtrpzo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tbxkeirv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gidhotxw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gjspysnp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vhawanie.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xitrlzko.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mqieavru.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3axbsmxgi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hnjwzlvp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rfewjnzb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kqbitmwh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mmrqwizs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ksmzdbge.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3pylsmllq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nrolabpg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gvhnahvx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kqhnzqbn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3iiclepsk.html


<!-- 参考信息 -->