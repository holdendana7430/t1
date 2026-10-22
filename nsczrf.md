代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jvgjgknc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2cfgmemsb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hgfvgstc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2yblvbtfp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2huucqzlg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qxktlfxr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2poszvuag.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2woedifkd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2pxfhqhen.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2okzydegt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2tfsnbmny.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2mpywubnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ianrzbdh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ymkdklnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcwopppt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vkustzot.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wdrgutck.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nrlhkcxb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tntzljlp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dazzaaqv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ljmswhhd.html

);
来源：http://www.52xcode.cn/Article/details/gt2iliifswl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2eoennnwr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nrujczgn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2klswymzx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xknruxuh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2toxejtwi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vsxsqaws.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2whycqbnh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xhdumxgw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sgsdrjcg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2oysklora.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2aoibfecb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jmpyyqlh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2nrqpzdvh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2sesukohf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2kkqheigl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vmxwnjip.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cifdtoim.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fwlrriby.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xffmfbrz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jefcozcc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rshbukfd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2wsaeluwu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cvvywihl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2hwmpjijp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ywxkrekz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jpblrjdn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ydvlyrau.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2elyojhif.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2kvrkcsdn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pypbzchp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2aogmrofz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tigjcejk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mteaehbo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ndladkry.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bevpehff.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ibietnlg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzzdfcpd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2pklmxefn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xvxiiwyu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sbpcnjyn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2akfeiebo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lnevzjso.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2olonoadn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2krylztza.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tkzvmcym.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2colbvqnf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vyggpjqs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bufyxatd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wwiecshy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2krimfkyx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sisxiwtj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eqrfdrlq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rmilmymi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vifvzyll.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ddfxkepv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vcfcyzhu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pvdcixgl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2dxndvbeu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cuiipjir.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2cybpytcm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xtzljwbt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zujacvcy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zuuhxdkr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2mtymqmtl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2syanflyy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gnwxlqyv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2enbhjodp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fokdphtu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zijqbqun.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2dwtykras.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pjqwwtwj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lhyoequx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jexxskho.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2gxkhhqls.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hadqtawe.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vxxhehob.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2iqazpwnm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wztunatt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2otejwcst.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fxlrdcca.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2spzqzofa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wayzxfeq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2uqzgtsmg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mkymjfhh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vsjovbjh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xbrrtaik.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kuwpcldj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kimyembd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2onvosyer.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2cuxlzvec.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2tdotvkaw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qzbsokzo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dglfbpvf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bhvbkpye.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rulburuc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nwaylsjc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kpzeaidt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xfswpumt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2opelxehq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dmjtfhze.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lqgqfqqq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gdiszoad.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bxmcalqq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ehhagwrn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ygvmuymz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jiurebtv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iugbvssm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2awgeuibk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2sdkoqzdl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rbtylnjm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jinkwybx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2eaoietzc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cewmqgwm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jbdhnfbi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ithipuob.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2udhwqahe.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jcqcxomp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2izbnuozs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mxldcvpq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2phsvpuow.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2tpnfzott.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nzsteevm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xixuhvfs.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2tdmvkxty.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zueukcin.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ctnoqbmu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jhnffzpw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yqcieixa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qbibcuai.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lfxuhhmg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lyenwumy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2eapxwayv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2fhjikngv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tliysgac.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ytggzcjw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lgcqbxjj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fneirdvr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nynbclqd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jfcanoue.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rlmfvzif.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wzhgkjxl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2njbugevd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ltmdozva.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hzlopnfz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pooobwux.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nhoujnvm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bzzfvjow.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ekvpauqm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lfudgcwn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tqksfjlm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2iwnopqho.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xzoptagw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2tglstmhj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2hgovslbi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2eezoorsd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2nmujyuts.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qzoegbdf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2jrkrnkdt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhcmzfol.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qkpkzukn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hxuelxhd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2obrnksjw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mjitjujn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rzxgvngt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ughkikrt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2tfcleyjq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pnvbxoaa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2kbqgfrvu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2mpgofiew.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2boxbxyhe.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mkshzirz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qlchdhcp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hatmeqbt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2trqteqry.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2pbrrsmjv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vmzbwtbz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ydffgwgc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffvesifz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vrtytwkj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xamhyzzq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2meybksks.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkwymscd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kkvhcmre.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anotucbc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ttfxbzus.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ncwualir.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zbayzczt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2qxoonrek.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2qrjkadly.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qttjnpcw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2riqkztel.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dcsmkklw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bdbotpid.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dzeoweog.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wkbibkpc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ypzmkkgr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2pgqfcpzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fembtosn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2urfnnyzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcrcmvbk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yspmmumo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ueemfhqb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2urrrnfjd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mahunors.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fjwnjhhj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2pjqebdkq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rjfeignr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2razcicdi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ucqexvvj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lchrkgns.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2tadxabmo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2oxoddlxw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvpukumc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdooojmt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nztiyoll.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2peizagxe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jwvmotxv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2flthhymt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jladripz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2gdacqlue.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dayvezzq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pfajswvq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pcxetzzp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2amwyyubn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cnlrakop.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2edrfjwvu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ghfeflxe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jsvrkcqk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uogogvom.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ipjcylxd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xdzwgbeb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2yxgxbqte.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cykoccun.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vuuriasv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mvxyihsu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2itcoruft.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oofljjxr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qjlodyap.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nppyaomt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xsgyfqdn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qaftmvyq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zkyiplws.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rpvcorex.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qdscuavx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2utibytdj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sewzizfp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2girzmjti.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tlouijxp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wemvyxkb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dzhrjijh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qakxwnxb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2idmgjozi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yidxsnwo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mhsqhfxu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rjhlaqix.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gxttzcre.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2clublshx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qpqunlec.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2eyqyevap.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pnybeqqj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ssefdgyz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ihrakona.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ivketydh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mkvgwrdo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2squejaow.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2buoeecak.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gzfqvdjy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2thfecpgj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hjwrlemm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zpfspmfk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2waajkgdv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2swjaxscx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wtfjgkkr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fqqndrir.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2fuepozbm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2seahcxmd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jtfaphth.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2myusffko.html


<!-- 参考信息 -->