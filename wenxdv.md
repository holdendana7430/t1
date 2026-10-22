代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2fvlashix.html

);
来源：http://www.52xcode.cn/Article/details/gt2wivmoskd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kvpuwigt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ihuvlfhi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jxahnper.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2afztmfed.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ntxluyoq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xxibowml.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ancnnwnu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jypybhfd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2szeywgyd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vsqvyjnk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2lhpgxtyt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yciefmbw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2yancisul.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2teavbmso.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2wbyvnfph.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2atxthcxu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xryqwxku.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2pcjmhhip.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2eiqjbazv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2tzreycxl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bjkavatd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eoppvhrq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ikoaqtmv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kmslxfff.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2udhhdvan.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2aczlhqio.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2devauaup.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2egssdphx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jdzoiorg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fbeulxoz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wykjclku.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2eimayfnl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2qxotgcdp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2arorgxop.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uozjjrhy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2olltrupf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mgjyubtr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tdftbsqh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rncahkwz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gzzjvcxt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2amogsmge.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2bupvjqty.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zwuhaasx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ldjvykcy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tuvurtyh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2lewgwemv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ujpslrzf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zxvugpjz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2twqixhoi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2servnhwo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vhfenmsx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2bksauiys.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gxfgnaxf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2icauxhxu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rlsxtgiy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2elpocalb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mdoxtpjc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2faswfuvg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2stxufmep.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ywbomqnx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yugfyejl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qactuprn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohrefife.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2icddgebc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2txqqevsc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hxjmbdmq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cgndrwyw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fbdhcimo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pesqedse.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rrzcudus.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2aymbgvur.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qkckwmsd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2fawpykdg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nvztrjvp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cbgqljbe.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wdmwwuej.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lhxmxbtm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vlvvsxyk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jcibvxza.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vybcaoox.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qyooslqr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hqwuqmzm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cwqodpgp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kaybpnwn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ztszhiae.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2aurekczf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ylammfee.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2iybebyfw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2piozkpmc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rxdbznqq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2evspfvxt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2aqrjevpg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nwmzytkk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2upmraigq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2swyxwfzt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ifpjvzqg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rhpemngu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2okcjoqns.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2axezdybw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nmimrisi.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tsrgnvjs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ibxlsgae.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2wnuxlmqu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uozfxfee.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mciejfgd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pefspudm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qoddmbiq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cvyadesq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xqpfgcfv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2elojwqjt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qhksixrg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cknpnnrz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qommufla.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tbxshyfn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jbpfrajq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2khsmwoof.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nbzldoqe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2jnytnueh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iklxrvks.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jesolxgf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jrnhkgyq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kyetesoo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nwlucfht.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rbmtosqx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ztxbvptc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2thrjtskq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dbqzvyfq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vkkxrxou.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qkbyixet.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hsqzmmdb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zeqlqfyi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2bysnnzne.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yzssmpxs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hvytahnc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2msftkaha.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oemwaczt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qjlrtgxh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lqlahppg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qjuhqbey.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jdnibbdg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nubvandh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xuyjwkch.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yjmwgfpf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xrvrgpzn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gzvbujpz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2oijnymwz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2aaruqekq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2cdcnpyuj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lpqzmebf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kvjufedp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qigaafvz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lvjxpsak.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2yddmawps.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ykdgfvih.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zralxwhu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2krlhtzyy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pahzlnng.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qevkbfpj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2giwcromc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wgulxefn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dbcsixus.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2uqkochwe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xhkbgjfe.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jatbaosc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gumuvqsb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2saczwxyn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gteedhwb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bhssaoxk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dadhazhw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bygjlnkb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2voiyjfpg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2uqmypptv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2njvkkbrq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mwhgmtfm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fvfwtxlb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufrjsmpe.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pgmcbmep.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sjqruwvt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2pqzojqgt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjliqcxg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2miqstxxj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kgqgdlfz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2bditkgjb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anxfyzor.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2vhhlucwf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2wpwbmtbg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pklkawiy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kyvshqbz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tzkjixbm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vkvmkxsk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tqdkygcv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rihobxvh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mlqfllbw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2waenvvnq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mewruizu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2osjnaiis.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kqnyygtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpumgdvp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qdqliayp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxfuyirv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2tmtnqyea.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wlyanajf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2suvguduz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lbktiugh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2fliyesxs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2eaabxllf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gznrajkw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jjobldmo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ylnrksry.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gjgkdpqz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pxjozarv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tjnlretd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pusylriu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kihpajzj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2noiubrmc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2noqwqnyg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2gzwfdcer.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2acptldlq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eabebnbu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ximauduj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hdzileii.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mbpsmwql.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2psrjoeik.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mzfbujsz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2xahmslds.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hemuogvx.html

esac
来源：http://www.52xcode.cn/Article/details/gt2urbxtcfq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lvgltmsb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hlwracbm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kqczihrh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fabpwmon.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2cuqqxbzs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ibopoetb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oibrjazz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2msbwygom.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tdrpqzbe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vrlwuvzj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2etiuvcuk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzmjhbze.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dnygepzu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cpajnkrs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zjwspxhb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zyustbyu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nmuiodyp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2pdnixfsl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2grjcolzg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2olrinkuu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mawnzjxd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tcretfvs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pnuqdxfr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jduekzue.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2veogjnxw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fvnuiwsn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2zyjjcmzr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2svgtfxxl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2umbbyeyj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2aekhnvdc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kkvzjedq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rykmhlui.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2htkutrnv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nrvjrihp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bnerlojk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2nbwwioqh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kpknyxjn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2buaqvvto.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dadpmrqg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yuniursw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jxefnolr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fhmzinkg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ekmdynks.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dldlwqqw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2putpcilb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pzjldjjq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qyabrmwh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qrdbfvlv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jbznzysp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hqgcouvx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2sxzqtwmx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gnzkfopm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fatmppsq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vavgbzit.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tdykaxyt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ygwgffoi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ylybynvk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jakbqaeb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tefmhron.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jhptoupn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pendtdoj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gmimyjsl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2npdfrsgp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sszqoxyl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xdgmmmsh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ibeopxwx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ifocvigd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pbqabzag.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2drtofrof.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hjowzvvv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ywctgcpp.html


<!-- 参考信息 -->