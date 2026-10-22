代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lpqnkkwo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2auikrfkd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2mlfbhmuf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fvrczcmq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gmjeyuzp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nhxsekvi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2atpxysnk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2gyyiimsk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aoayzbjd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2puhfahpn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fygniysm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ddjbpoyr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kcomfumz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dejjkpja.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nadgokev.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2snuahnkp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ishabsex.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2azemfhrx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2uzkjajun.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xmoauotv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2estewcjf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zwpcyahv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2hvhkkamd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zstuhkvb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2auisbrfm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2noguteuc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvlnfchk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yuvnqrgo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xyzxubjf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cvdagfuk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qrbptayk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2oeydizoo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ztssmlhr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lcavlzpk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ijsukbji.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bdkjiijb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kbzvlsrj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jufuylme.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xxltafwp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bmwqdeax.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wdvecujh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fvnspkau.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzguicks.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kimumoia.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2joomqjsm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2aycqsyzz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwonzdtx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ovtfmmif.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbbcwsqu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hbksglbo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fjorxlzz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ngdxrcsl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hlbafbob.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2itgkmjbb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fiohrdvw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2skxyzltc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cjpswwtp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lkrkppiz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wftairft.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mwjljnhw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2uddvgyjz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2peqqohpg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qtpnqvht.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ejptuqxp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2arlkibzz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hdrpirif.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2rohwbucz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zuqkdfvc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ualhnrce.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bvmtmiar.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hlsanrhp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wfbmkbqz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zishhckz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wyecstzv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qrgvysdu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2imvzlphi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pxrdxwpl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2lxqpiqci.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hjowuzpw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2azsvxrkw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2knsoluqm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jpjyandx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2odroffuq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cjhtxwpz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2oyrhlosx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zlmelgea.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dnikwooq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2brhjzyis.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sifjfayj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2qjudzafa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cewxbjcl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tnbzywel.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2reoqfbbw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2chejzczy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2aopduxsg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pnxqxmqt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hdjoglom.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2okoizbye.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2tbqxpibi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jsppekdt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ubgonpzn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2egqmpvki.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mzzhgedt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ngezdxju.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2cmltpsec.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rlvlzlth.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cvvqjdds.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ubaumgqw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xnmqhwbe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2cepyeldq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2iwusmepz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mihqoatk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2khgujdxv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vmbfikdj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eugetzew.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zarqhbua.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ablaefpp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jhzsgiox.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ersuooyw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qkylwhcc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sgwcsmow.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ogpdponz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qoakhwlp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2olacldwh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tllotaiz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rwrwukih.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hmtfaksd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xvqmyzxu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2eqwzhayz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ngjhxhvo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2drdkipbx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hdsswomw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fijorlnf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2nbbkzgqq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ycuihogm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qagaslyc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lhmcnahg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ifzhgqhb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nwzouasr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fmupbiru.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hnwpelfi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kaeggnmh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wqvmqdpv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hyyluenx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hfpargnq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vnqunhux.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2oamzktrr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2dnmtfyjz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lsbntdzj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2zmjwawxp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hjfjkytj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gjvhbskg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2dfggkrqw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jzgvtddb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2addspxnu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2pvgjbaoj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2afkcagiy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2iphcdwsc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zdewricd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2rasmztyk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2aaedbtqm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2btjxhnyj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bqifehqg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2rnruhwbv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xtdsdxwi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hsrldryl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yndbftjd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfapvqnm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2avhmzles.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwgbnecv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ecpnrwxm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajedmanw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ztptpgpf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2leolyooz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ihupgata.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rbynhzon.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2eebuhyli.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bpybjlee.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mrygvqlh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2deucbfhc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jzmebgwg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2egknvwyj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vzbniufx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qcsdvont.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nikafpmw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wpejfamk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2klmiulhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbnwphad.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2blpywswf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spuifmfl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kvmykfoz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xtwbrfud.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2rwkuaxvd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2whikqfcg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ixfwtpdi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zccjewro.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qzesspog.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zdnwdggh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2cmjxpxwl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ubpyitit.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nphtlklg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2simojxgx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gcbzwtfh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvezrueb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2psniagew.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hhuacrxz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nzzrriqr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oezgknta.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ckuxbrmx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vgelprwq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2spovquok.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2mrrbzrtz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qxmxoimw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xbosowol.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qywmoyhs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lokigbfv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xyeynshg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzkkqaeo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2givcbggq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2swmwortd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tusldnkl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dazrzzmc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fqfdsrhw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2arrjvozl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2edryskfk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xbgtvqzq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fxhuanjs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cnlrzuhp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2boonsgxy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vhugfcpn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2klakcovt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wgyrlqbc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fqrvioof.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kyuskzrn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bmzwhuvd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mbpgjmna.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jktnvbvj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lymxztkl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hakloukn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qhyhkqbg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ukgxzpht.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uzksking.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2iyafhncz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2aapmputr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uamysgna.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gkwrdzqo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jmgozcpk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hvyugvup.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pejvmfwq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gbvtpuhx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2dlsmxivg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ndpqfwty.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bbcyjbjm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2azjqjpet.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tzgnhdgw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2frydewdk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rwiwpvfd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2plsffvmg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjmnlbva.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uneuwmid.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2axlktpct.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2oxupovcy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2eynhxsxp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cnxdxplp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mrtomwtf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bwudficc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ybqlwpki.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hkglxbnc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzwgebja.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dllpmvue.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dydrmwex.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2iibyidjy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wzerzxrk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pitavyvz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kxgvalqv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jfqcbnnv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2twoiaaly.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2efseepwx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zyqrjzig.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbroctcq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wnvbygll.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fhrupgni.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xznsnbbn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qymwwjwv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2vemwyzpd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vjpikzos.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2owvtyved.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2noshzyri.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2slzmqzvd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2nwtdxchl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wuiucvwp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tmnmlyjf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wctfuqet.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zcqkxesx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ahxfwmgm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pxvqxqrr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kuvpqzbt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2sgwzqfir.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jfzsvsyr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kudcyjbl.html


<!-- 参考信息 -->