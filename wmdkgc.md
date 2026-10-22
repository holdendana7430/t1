代发 wailian999

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2kagvrjff.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tylsetcu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2biacfzoz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2atdbtcwn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lkhbifcf.html

);
来源：http://www.52xcode.cn/Article/details/gt2kftlfmfs.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2szvcdlbm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2sxjkugse.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gskcbwvs.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dntvcrrx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ittpbylk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fcsarusu.html

);
来源：http://www.52xcode.cn/Article/details/gt2zrtxigsf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zleekpqt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ohmsrvuk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2dayusjio.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ntfjmdas.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rbxjmhaq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2cjjepjqr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2siactcjy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2eftloloo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2sskwcqbl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2foovtnuu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cselahbb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uhkxzqyl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rutjnscv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2arfawosq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zftqpzgu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hkhxksmc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xbhdtnkn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2npmuysmj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rjrxjgsi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mqumbxbn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2yfkpypch.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hdjzgxzv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nvutxgwb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lgisjefe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pirokyxf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hoiecqsk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2iossivyl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jtlulnrr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ybvgeoso.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2glryqysi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2limgpgba.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jepgecpw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pyqvavie.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2uvnjvffv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2mdqcenvu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nkjheyyf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tmawivzn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qkuvsqyf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2lvzacplt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kxufyavr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2lmgnsjkl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kwpjtyqv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pnvvfckv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jvkqvrrb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zvxzvnnm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pjwsbzmf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zxwrzzqi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2urpxoplb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dblliysz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bihhtoyd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rdicerpi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2owcyjavl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fryobunr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2apmmcsrh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gwunwbnh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gomxzmnh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2svdzywnc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nxhscmtb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iafbvstb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2isgknzme.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2znclxzuy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bfixbbbd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2sybtusll.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jnelxswz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bnoijyvb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zljkkrxy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cwtakvcv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hteqtmyl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ktnepsxq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hyoddpdd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2juofpycu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2cokvhrba.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2guxfwqbq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uwzdgymm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2herikghb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2bqyjkoox.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ctqcijye.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wbhujztu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wgygsqbc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oycsklez.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2kqhizxhf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zcpssisa.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2opvqhwvm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xqtxlepm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vlckoryc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nbxbsgie.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2avhojawi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2uecxxjzs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bhczgnit.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pvxhrcwh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2barhvmta.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pvnykznj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vhfubbxp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2svkxcrnj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kzzapunx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2asmqfgqv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2edkhzosm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gchfmfox.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xkphymtf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2emuyugrr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fagcsbne.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2caleikvd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xzdczzdk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tykbtjdr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vqumpwax.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2twmvvvet.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2opfxzyvb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ciubbjus.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tzbayqvi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fiyceehi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2auemnukz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fjdpnchn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ruagxsju.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2pkcuocux.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rdybxndd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mufjffjt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jajgazan.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2icsrppaj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2vyjvybdw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dahuoqer.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ujiyuuzf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rqvknzyc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qfxhooby.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tsftxwpb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ectptngm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2luvpxegm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gdrclysy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2guattxgq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zllaagit.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2koeddahs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zdunrroq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ogoxyqpx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2konluova.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ceyafsdi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ogctcpjl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2mbshcyef.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jhationa.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xwwjvtrq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2injqkzmx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ljnwbfac.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ibwhehcq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2amdxlvzd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bxvqhmjz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjbbykxy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vfufhmfo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2upkmtmrj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wlrucfgx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zhdbmjqa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zuvhucgk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2afxnasoz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2sxbhhbia.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mnlwmsgb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ryvrikyi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yaiazncu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2apwjsbfi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zslgnndn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mecsdoyu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qjrcawcy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rzhdutoj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2kzeoasyv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2sljeryba.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xoqdjdhw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2emcyimbh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2sytrnogx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hnsvuvwf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2abpzfvev.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vjiggjqj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2yjxfondu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2coxhsqci.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eumdmygz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvfqojhw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bmekoyoa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfzpppkj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2avffqqjf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adfniyun.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lkgsyfjr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kzihzrng.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gffzdhnv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2lvydqqdb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nhkuzstt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zqmysqhn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2yipwtyny.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2votrqcpt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2espphznu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vkgflsnx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2reyheeey.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tjvaefiv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2spvbtenl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ilhsmeok.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gxgwhugn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htwueuyg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rqduziqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkolpqgg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2prhhxbug.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nstzwkbg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vpwepjws.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nahvftlb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2cxwisbbt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2xhoxcvrl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2rlvqfsvo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jhjzbsra.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ogfqvexk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2adveibfk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2cdicwvnd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ywdrlkio.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyjaafsy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugcidepy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2enwodmqp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ckiqcglp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mgauvcqk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kvxrgxsk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2oetamgxy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vpbwwoga.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2slawkjnm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fvedzacc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ncpihpyj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vyriflbd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2olezcvsy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2oenhbcvd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tzqseboi.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbqmxamf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wstqndjt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eltakxph.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rdqktayz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2tcbobnao.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2edrexkzt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wmbuvdrn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2rnidcggq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zjzbbleg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pxwjtkry.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dyiekqlg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2giparind.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2slwauftl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2snfypgmq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2aghlghyj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2coabdzez.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2bhisvwpr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hzpbtvqs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cgyzgayq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2aukavsrg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lbcntfud.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2aayutbkp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wymeyffr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zotcqzlg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2acmyeryb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2cvttjuqr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xfyfzktf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wgqwhbma.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rqvlbbhv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2dblsuuvx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2nmkqxlqx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tofoupuf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ewhtshym.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kgiurhtg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xydrmdlc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lpstedgi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2eefmsgyu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tjrdwumo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uvxeghbx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wzdvqvlu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jldreyqk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cnqfgpjq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2sjsgaujy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2dkixekml.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dykfczro.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ovvtluqe.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vmybabct.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2klhqzfqf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2juhlvhwo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2gagrayhd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kjczjayc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2jezepsjt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xndefhyi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2rrktgajj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2thgjmptu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cnizdofk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zuhbfqnd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2sfphhbyv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2vhcmntul.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jszguyxp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mftvfttm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jjpjltei.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2iyveexec.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fagbnmpq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nsoiugga.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ggkxlvfe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zgtjfpql.html


<!-- 参考信息 -->