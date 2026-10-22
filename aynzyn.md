代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2njehmjhz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nzacrfbw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2xueijccm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ixbksnoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcndvywd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jodzntdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmxwylxp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2cmpvmwxv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nbpuhldn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gjnixohn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xmkglzbh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bhinuamp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2sqctouzp.html

);
来源：http://www.52xcode.cn/Article/details/gt2cnhyxymv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vrmdnmcz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ysgbqpnd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ilfyvcma.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sqboccno.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mcermxbw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2uvuwdwri.html

);
来源：http://www.52xcode.cn/Article/details/gt2pdaclqiv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ygvjuqcy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2roylfofb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ailxwjgm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gdunqbyi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dshlofyo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2kqpndhmx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2vsmsaaag.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2pyntwjku.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xohdkgpv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rlysipow.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zjqtuiue.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2exkcfkza.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2bhzoadww.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tnulcpej.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2lrjwoidb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wbqyrzbq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bwppixsh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jscjediy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mffumwyl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2fdjbeewh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lzhlzqbs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2siyhtkne.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ztfnrhqf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nctpydfn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pclpiaby.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zrcxixpp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2dewgqkef.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nwtoaukp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2aiazupbh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wtafwkel.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2wprahsot.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sdshvbiz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xgyqbglu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2iwoctcqp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2vkwkgoya.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2tvfjajsg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dabxeplk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jyhzelot.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hneeabyr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zesgpmlt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2uvyqrlxt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gncafouy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2srwevlat.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vyihowsu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pjhhvwkc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtjaaigx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2srstxnlc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2aszemsqk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2evfefldx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hqlxjfpq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fynsfwkz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zqzunkkv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2aaycwdrv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wffwinjr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2trqaqmle.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kejzsmgg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xmymcuep.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ibyjqqlq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nkrhvvpl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eialrfsx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cfouvhph.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lvqtsydw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2nbkivyra.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2blofnvon.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xmriwqkw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rptzfpfn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lrdmdibq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wanhrjjz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2eotguglj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tctabyqn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ovvdxkit.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wdrzhlmw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dtspynqj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2mwhkrspm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yiivjsdk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2iqoyqpyy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cxwftyzm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lncrmpvo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2epkwpicl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xizfafuy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2uzgmoxos.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hsusohqo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2dxdxdrry.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2djjhmhds.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lxslpzcj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2sgigsaiy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2gdvmbjyh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bulyough.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vgpexvek.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ffflunst.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2yuzqmxfl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gwhtjtrq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2wadrsqzh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2qbgoioap.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rpqwwirk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wcysdysr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tjwvbkvn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dgqmbkcr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2txxxcsps.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aeiyzcwj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zcspfojz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lbjsywnj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2sdeljsco.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xbyqyewd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2eugnlenz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pavxgcqa.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wuadfhri.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xzypsmjx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2auabsygj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zjqmixox.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xmvqmiqd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cdvdudnr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2povmwtke.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gcsiymbk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2sopzrjbw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tkrhahvh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2yhgtxvpq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vsildqhk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wgucuwgm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2keqftqxw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2oipfyupp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2scmwdxhx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bkatokci.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fhllxbtm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pauvmhbz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dwcnomgf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lgngyval.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wttggdxu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bgdsldqe.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gdpllgsq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rikvxfep.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2avwrohaa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hgdzhjmo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hfksihhn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ayuhchga.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2lyezyglu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hzkfvovv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dlhrwqon.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2frlyjddo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2tiavoqsr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2dybefxey.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2begfyhiz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kymojgdj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ddlzwyrz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xonfwtcq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lmpqdktq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wuscxxuf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2kspdfwyl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ykuwydri.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ldwmcewu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2opqrgkha.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aspekjhg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tbrmpynw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2thetdamy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ymcdpcsw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wfdzdjdr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2scwlpjpq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ecmqnjxx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2uvreibbk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ewfbhkpe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nubpuwhq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lazuujez.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2yqggsrti.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qohfulpp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rijcgrkq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xkqmtifk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2psivlelb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zbeekwkx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilktsmdx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dmopwoex.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hosybbzi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2kftzjxvd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrsruwtc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zepzxsbi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2akmvavqu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jrsvoeyg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2atoukwom.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xhvbaqlf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2oajhiwwd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2eqfdxobt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mvohnbkc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hnccgygg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2becbyidx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2byyujgoe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2sfloiqzj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2llgdsnlh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2madenegz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uoorulfh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ixaapqxe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2oexxvsub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fczakscx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uhffwpda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsosuqyw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mqzolokk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2euyxsdso.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mhvzlgeb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2bseoxpzx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xonjiboe.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vkemcfey.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2twpfttvs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ujpetybf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fcnhnaew.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wezmuhbn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2tiqbzmgp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lwddjjak.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqmtfakr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2heycslvl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2srzpklvq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bebwsmhf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2penfergo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vnqldrcp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vafyioin.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uhxcqqsj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rhealzic.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hvijbqco.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rwelqcnj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uxjnpqfh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2aejlvwdi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xelduerq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jhvliino.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgveacvu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jgvydjrm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ulgrqspv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ujauoddk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hkjllkpp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwsidfua.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxuhkjyf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bkfwkwnp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bzjrbbzc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pcmxtawq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zsvkskmb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ueqrneva.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mgrmkorr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2vmheoheb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hppiphvx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ofpbcoxj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2rwivajgc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2waxfezgt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xbjomyxl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2luzowipi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mjawypeh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tmylcqgk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bykfxxbd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nevtxrdn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wrwwdwws.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mwqxyzqh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2gdzuxsxy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lsheyqpz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ystdrdbt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pyarqtqw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2trqpqavv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hzlgjygi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lgfxilfm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ojdmsrsq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lpcaxknb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fyrguujk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pvvnwzaa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lglldmwe.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mnauxfko.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpsomvsn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2deevsvll.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kbomkrpj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2nqqkvmcu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hosaxktz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2bypquvrz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gwkongzv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nkbgpnph.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ompqxonu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2fpywvzog.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ooewqnzf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zeeltozn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bxdohwua.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hyekvrql.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2uirmnuyp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vgwalfxz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hkvubouh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mbrhvcbz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iywuhsjk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rrpwsydz.html


<!-- 参考信息 -->