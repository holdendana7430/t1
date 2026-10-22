代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2papivrir.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nveowzai.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2iutpconi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bprpbups.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jxrfvunj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vitfecuh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2czvvwxee.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sygfsouv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zssitwtk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zwlyxzcn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2eknwiyey.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ridrupjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwgljuvj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2oemwwfye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxefmekn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jdpvxefr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pfieuvug.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2czhsqmpy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ucwlhhmr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ujdhxwlu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qowsbizx.html

);
来源：http://www.52xcode.cn/Article/details/gt2fkzqjini.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tgpclgsx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pzkqtnhc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yjcukqzc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2uwqkvpuc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ocbyzigs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ijibbgvj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2npjtrkmf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wrpxmhqe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hpjnvxup.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2oxbnnrbc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jxszrbcs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gyhtzcxi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qfoydxnq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vuetzfma.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ujgmhwgp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ggktxain.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mgmkaruq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ljehgkdh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dukisbgh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2sulncrpz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zraqljuo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2aelxjqjh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qqrkxjmo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bsbmhvfk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kkdqgrpi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2eokjhnyp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2mwljetqw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xriuktkd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vueweodv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kzzcsfxk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hwbhinib.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2lvmkrfkb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nmzsrzdm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zppyldfa.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ytdfxssb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bagiuicf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tqelvhfp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yrrefglu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2onjaikzh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xkqiglll.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fzlhbnqg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2sbfmqabd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zgvvgbgk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wfycwzfl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kmrcypsh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mklzsmuz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2uaufnfys.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2qreahrhv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hbfyqoeg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fsbfrzkg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pwwiwnfa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jyquhlac.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jsvhqioq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2rcewybnr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ekbdsoyc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2izeafrdq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sqybowec.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ilencpfo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2scnbewjb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2igupkkfz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dtkmhtor.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hionajgx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rcbmtazv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hogmcowc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xwhtaimd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jvywuvoz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ranwfazv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pmbxhkrl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dojkfera.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2uoihzxse.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pwvpbmow.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wkdphrqy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2unvpkrnm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2qyciuydk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2renrxuoj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tfwxdutj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2cwxiwhuu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pqidfaxi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xmqrlohw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yrlbhsbh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bntrodjf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lqlpjdhx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ttcuopab.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2akislonx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lvkuvewc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2syunjaez.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2hljxkuyg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2rwoimdib.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2pzqxygyd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2guqanwwo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rxwdyalt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2eiflocev.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ndryepdg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vrhwfyjr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2srtxpysx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hjkpuqqk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2auzisepz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kmmpvvto.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2eymtlrsm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2anugxaxb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hspwdhag.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gslaavyz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zlcoajgr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dmrmyiqj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mgymuoxl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2yoqoeeoi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xzhavrkt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ershvpie.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2gvnfhryg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wajayzko.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2esaplrml.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2dcdinfew.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2acoikwck.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ryvrwdox.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hiugoyks.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2iwqbjtyk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2obrkewam.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zkokguri.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pfsxmdfo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2azlnvplp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lonfphjt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dgyzdbfv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wmcjoeyb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wwglxcdn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hxrhject.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2iqrfmphs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lexkvsrp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ydyxczmb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xztadysy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lmvtluar.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eskcnuka.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pwwgeehs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2msjjvjqz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bowqvupd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2aliknxnm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ugncxomq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2tmsgioev.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2waxrkhhw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kxadtldr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2oorfmwbp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pxxkmhlh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dxkeaudi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hixkyzpm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tjmxxmvw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2twcqzrcq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2uythozhs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nhffrebt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qynfrzcn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pjvlalfc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rvwhmnkl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2avycidil.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2yjacgpui.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jialnliw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dcgenbke.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gymlrzbd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pzwptwru.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bvthdsif.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2yxsrbyrx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cssefstr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xsbcqdnm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jewntmgr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vuqstoeh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ovpjibmm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2odmporzb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iwnrglzg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ajibeipt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vzlrvoru.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dfuzzklx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2pellmgae.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2oqgwgokt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2louwoafw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2lulrhkwc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2swuhziex.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2cjhgjlfd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2trbrmwhh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxaptnsr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2swntrzdw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvpfysav.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2zcrjepzc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yytahhkq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mpdxlpjd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gvrmnsbq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2umthjpir.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jhmqxfnx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2rybutrae.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mmruafsm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tvpncyrj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zncacrnl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dailyipo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2texrhljq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tgagdecu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qzpupzek.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2worzklgy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xopzmenz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tyjoaphk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xrwremeh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2odirxpbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajckgfgd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zagrtuwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tumaynbi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2njjmmptz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fjzktvbk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pxugeupm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gdacktxo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2urnwwmux.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bnaeiufz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ppqhlddw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ernabbqo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vpxtaxpb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rvjzmuhz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qdahbnvr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lnlbqgwn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltizetlk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2axinapjm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xykarzch.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2iegyvevx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dgndsbpd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tzaezvbk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2advueacq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wliodyzw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cxviyphe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tbabopva.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2cjeqpnoe.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fzskepur.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ayjljbgb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vmbvptdb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hmltejgk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2eyzokkey.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2kjekoiev.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2maecryvo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2byfffdaw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bcvdmsng.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ksfqgzfx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nsvjyxay.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vsaxauyy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2pgocswdf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iyxfzppy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2awggrswe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2knbgulqh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2bswncevx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2rwwfocde.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kkqswivk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vpahocqd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mchxcxbs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sqgrznzw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2leakxfvw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pppvgsmr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dounupng.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jbrxvwro.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lvagpcau.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ihapofpt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tmozzcqx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vomqhnow.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ldvbsunu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzlsitim.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2muuxksei.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2mlyocvbp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qxvjuxlg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2utuamytv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2sifgltfb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jqycvgmh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hjukzycz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qatarjxa.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pqwipqfd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2otqyluiz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qsauvcks.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfuwinfn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2otlwcmou.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hkzzojot.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qqxvhiih.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xwgjoeeo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2nistpclr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ylqvmyoe.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2mdebcnzt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bhrbeyyw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lcsnqmvn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gcclklzt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2pdvwadct.html


<!-- 参考信息 -->