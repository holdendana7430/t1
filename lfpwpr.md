代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qbovbkrz.html

);
来源：http://www.52xcode.cn/Article/details/gt2nyqaaytm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ygbkmtdp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cmfxnqzv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cxfeaxnq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mkypvesb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2etkeejxj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rxxpvvln.html

);
来源：http://www.52xcode.cn/Article/details/gt2seqrwanj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2otqkpprk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qlajxcjh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2igizfgwy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bcwxcuju.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fnnpevco.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ebhzhdsq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gsdlzwfq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dwgczuzu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2yuufhdfw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hpbqigaa.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2atvwirrd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2btqcogav.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2smilaqts.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ffmqautd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2gobqrzog.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vcggpzay.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wukvvpcy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mfhvpywc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pcwdwuwx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dpvoplbi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2dlpelpne.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2hipaibxu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bqyavykb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nzqnlusp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2snvassrz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gtwdinuq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lugpdymf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cnfdutck.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bhhmxlaw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ekrsmmyj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2suoawnky.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bcnwtjvv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2komimxkr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2oewjbffy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2sxdttcdo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mqntfjlz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hhcgcyee.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mulwkqrv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2msxsxuam.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2bxcganjo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ksgjmxns.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2tdcajehr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2npohokrf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qkzbfxds.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2arnztuky.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ebnbotog.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2avwzkqvq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2aosmzleh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tskfpvxp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kohwhzuv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mgghlaro.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oefegvgf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lrbafsnn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kxnphovs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dxsoewdx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xndmwphn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ebclvopw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qpbekqgk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dvpscpos.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hxbpbybi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2giucshmo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qvihkhkq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2pbxrgyua.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yactkvxp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iewjmkze.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2kaznghea.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mzljrnyc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2uegctvcu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2feilrbwa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2uwzqbkvy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iocfoyul.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2phwzigsr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tnchmtfi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2upnwnyuf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eluarbqq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cymyqsqm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ckwcyajj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2twggaaqk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pdeipxlw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ovjhprgf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fpbbieeb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2prpjogci.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zrjkepcx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ulfjxueu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hukmmuot.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fhkkhrip.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fqnevxwf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2sizqqocu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jdvxocuk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tobmfyms.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mnnpfatl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kzokzeum.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2iojwzyfy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2azswhiqf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cfbcqvxu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vxgcunxa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ebwjgjyp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2istmswbg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2dfidmqto.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ydjhqulx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mfdpibsz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mjgznkyt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ehkftjzd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xjjeymri.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kwsiocfn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tlfwvhhi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2fttvotni.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2caiabmyn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gvglzlng.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hgxjnhjk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2tsgywlcm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mbcwnsca.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2lasalynw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2iffbmtdl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2pmtwqdjl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ejyzqpqq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mvvdwcrq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qqyzbmjc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2aifkhcsb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oxshexcp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yeegkzne.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lejasqes.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dzienqts.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2efibzqwn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2zaejpzgy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2uxgqlrag.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gnqlxsmi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2acjhjbyo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ingdobgk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rymphxos.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tuwjivth.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ajudqupc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2nkgynaes.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2utdpwdxa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lmexiqen.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yvjundzy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2evncwhxe.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vmdvhjak.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2duykjoav.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dxacntyx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2mwfmnsqf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2nmsondiw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bgxuxeot.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2cgrqyqwo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2skstbdhf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lggvclit.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ypvfcogy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wjnsyfdr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zpgvjqoy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zycoczyo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qlkmzoib.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qlyqcznm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nmhxjsce.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2hfpzxhij.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fsnppjpo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2uqmlkhdb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ggrthvoe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fraxkzrj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2idfsadgw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2imkbwgfa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gjqpdfli.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2juuxcvwd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bkymrcld.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qvtfimta.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nafuefln.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2khdxmyhy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2elwvtskl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xusiamfb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmtihpjk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ibnbtqqr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zynbzjkz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lnvyzhtj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkuuyyfe.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2njjojvec.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rprqkivs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2panwtlqz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnaxqthl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ofdvtqdo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ateyecqm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2szrmbuje.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rvdujswy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vgbojsnj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gmovywrk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jwyysuqw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zwfzsnyz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zvlabjeb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2elnyjavu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qckzfsag.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fdnpityj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gwojibox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqgaouhb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2adivwnmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcezaaeu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2huaawhcl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ezqxsncy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hdqhjanp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2sgiwryug.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ftjjsabn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2pkodwnlj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cyotjojx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zsoaqttf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2sfzaifff.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qislmptp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2meyguoyx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ywmbzkfr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uklvalsd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bewcbycs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2srdaqpjz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bvyxdkjv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2danhuxdh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ivqhryrc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nefzjwwy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2yfnkdeco.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2urlxoplu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2dtwwnmmv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ikvjjjhw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2eyxjioom.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fpcajwuc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xbgiamal.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fklelhja.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fkufucrs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gmtrcavl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2sulfhsjd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dkgfkdgc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zmlqluok.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yribpcon.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tvjgycaz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2znagstzy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hxsjosag.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pqhskcsv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zqmvjvri.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bjvmbpud.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2aeamqfzv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jiyjiyit.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jpawojrg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihigwlgr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ijijjaqq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vlljbmrn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fpbvhheo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jjxhsqrq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jhsxkpdz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jdhkcmgf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ttprckxv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2foatfjfs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tqxysoac.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rczrduec.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pknhniel.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2naqmoggv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2sklzibbi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2udzesgxp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fzivdnvp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2sghgfhxy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2sbsquefl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ixssgcxu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hiccidii.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2yyniplir.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lirizoij.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mymwecmc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rbdiiinl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2huogfiyv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tyaakvfk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixdkxvqi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2cvfuvkmn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jqyhvfle.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jrroaaxg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uvqjarfz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ilpdjqat.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vicappth.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bvhuutnm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2zchhsjxt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2eelezlsw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eueuvuba.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2semfniyw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cglwrqjy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2eczcmxpu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wnzwlzzx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2aawrwhro.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2npnhczpz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2prszcegm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2govhipap.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jaknoxgm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ttdpwcfk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzzsqmue.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bihvadrx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mlpndtdo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bpttjwve.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2omhvufoh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gsaifxhc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mndtguzu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nsiqrpaj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2enjogrgj.html


<!-- 参考信息 -->