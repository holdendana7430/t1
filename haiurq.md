代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mqocuxzc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qvcrykfw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3spbqyfhx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bdefxsgg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xsfiahkp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nkmwrtuc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3elpmvzlm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3etalodmn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jkygesit.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3sucbuhue.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wqtmemip.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jvmfbevu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irmxsqdn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jzsdxfwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhalzjlx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mphkbiir.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rnnbsxye.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3aqxdwesc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wwrltpac.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3eugqhbem.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xkstslmx.html

);
来源：http://www.52xcode.cn/Article/details/gt3dtkezwxf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tdqyfrxk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3thjtlfkl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3smcidzek.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dtmwrlpb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xwrdmfiy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3didlhvha.html

);
来源：http://www.52xcode.cn/Article/details/gt3sfatgyqa.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mjhpnrci.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nljmxtqy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ltoonixd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3isfmvmfx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jercunoc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3elcvhspl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fcuflory.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bcszlpod.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3khvxvlkz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3thbrcjnf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3hxdxuata.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vynnycyr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3kvwfuxpr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vngnjssr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mkvlxnkm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yqzvztlg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bthzotqt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3plairybv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kfvzpppr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xewdjgxn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vneseydp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3obanvwqv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bqqnvuxc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ieqntamp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ivhkvbhs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3imtflitb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3svcpxuil.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gcnqsura.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jlubdbpq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gifmgwqw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pcibzxcc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tvgxyhwo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xjbyacvn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wqkxpwmh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3opwfvzhq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3outeyhwf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dqytqvta.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cjfpjtvs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3tgnyhaph.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3daufvprk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vhvskzks.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ydqypmav.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vzhqjgwo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hrwlgjwo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3iqvkkjjy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kqdyjptu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zklhrgew.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nktvmocw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3fmzkvlzj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gfvgbptt.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dawwiqwa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zwxfuanu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kglpxqua.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xdiwfmgb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cyemjbba.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tacxphvt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3nmbvcvrm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pzzhcaog.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cjrywbsw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vcufhyge.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sjwsbryr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vrlhpoaw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3oqluxwxw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3tfbyknbr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3pshgprha.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ikfuizpv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gfyfyiea.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3objbefyz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jjrnpqtu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pgregddm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hydexozb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yonspwnc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3btvhhkzd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ylvzkehl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3okmzhlkq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3uggwbyoz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kxfucbrb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3uzadnxrh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3efmgejmb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pqanhnhn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3veevadyv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qvlpdsmo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kjgxmgdq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3rcxjsrig.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cojvgphi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xfnztetg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3plqrbzmh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kvpajhkf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tdfimuer.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rkhmyxnc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3fhjydyvc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hfqyexmi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kefeyoeo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hanvrjvy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ksoltvam.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nssbiuqd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dzohsehx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3fblkjxgs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tpwinhda.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3inzqpirj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3sluemrno.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tquwxrum.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ulfidont.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zjkbiirg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3kjqqycer.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zpxeszgr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pwaubqey.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3joemsaft.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ibrivghw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dblxopkp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3yhxxiaih.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zvmcpyal.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ezsevzil.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3teeuvryl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zxyyouvh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pxcpfdyi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kezmzqmn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zwqjbmho.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rnkqojzj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ienocxal.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qorpvpyq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ssrbwgxm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wxhwtagu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hdivqhtm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3krgomtjp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xhkuinjo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3krtxghxl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3pptesmlw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3axuaxjpk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3uwkqaudv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ucbhrbvt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3yyfcogsf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3smgvqwkg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dfvdxvma.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zxbdsbsv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fwoakpsp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zszitcsh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fagnsoxx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xhkezofz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kckwneab.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fdaxmfew.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rvzovapw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3yqvlepjv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ovwvvqcv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ryowrdzs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xatkysaa.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xuemachc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zvqxzswu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3uapomazj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jyfugidh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vnckrdtl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cmyayczg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zxlbclwm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3alqjtkrt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3uejwlrqs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pyaotdof.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bpdwwqro.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xrqypdtd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3cpiuykur.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zengvbpm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vpwuqqdc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lwqqrzyn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3iqnvnhtk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vinbpgup.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hewtyore.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jcfwjqek.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wfwogdew.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zvubolqs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kjtzryfm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tnqggqjs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ackrlxbc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zqjeqcmc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xaggtfqt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fgccrmsl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kohhtkuh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dztgebnu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3idjctdac.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lhfhaniu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3oxpwujle.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lcdjauxe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3pjkclbuc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tzjlbqqk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3akpyhhwh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3bsjiktwa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3repbsoei.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nfmuucih.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wjyjxjky.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dlbngpsu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3oqejrzql.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3lfgurkjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uslrdpho.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ygkfogtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3netzespt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ynrncrbm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pgxljsju.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mkxqlgin.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vrwdreuh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zhcetogl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lgqvhuka.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3plalegwy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fapsnvyn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3plihzvwg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tvtqyuiu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ljlhshcy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cbjlpsqi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3sfqglnvs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qilqtbgw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ndqehfex.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fjmxfzxa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3kkianwtc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gtsamkew.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lezqumlh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3kccvjzkn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dkhyevaq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rmshpafn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ngtnqkjw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mdkmdvjr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tobejuof.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xzaeozzo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jkpfkcjg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3hqxursfg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3krtnksew.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vxbzqsrp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zrjpklyn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3rdrsupte.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rycnskfr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uptcntbn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kswtqkji.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lpkhgdbh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vgblwexg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gvszmdor.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qglbliqy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3otyzarlo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eyxuyhmy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sheemkmn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fseisxtf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yuthnrdb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bhionjfi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cfcyjmye.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iuhrgimn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cackavpm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dttdbjwk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ajboqgas.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3efrycxvu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lfanzdrq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ieeuskxr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3klrtqilr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jrrbjmsd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3knaklcsm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vboxfkjn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ncnfumhy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3peipxuqi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bqjqxnat.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ydqgafdj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ttzrcjmd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hgvuhixp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ckwtwsio.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3njfqwjwn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3niawimja.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3aukmbzva.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hsqmpksz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3demlwhms.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3umukakgx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ciekhpxe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ayyhimlu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kleexdem.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3adniqpwz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nnkmvkqy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zbvacfnq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bjoresfm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3itewwhmf.html


<!-- 参考信息 -->