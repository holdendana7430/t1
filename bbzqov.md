代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2miiawyqq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qawjcgwv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nmdlhrxs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vlbxtrwo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tfzhwxxz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pzyqxvpd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kfzozcqs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dvumtqyo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fyjrknoe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2iuxqymcd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bfimqeal.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2mgxsaeit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucdcsuzp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ncdbqkfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqpftlxt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kzdxliii.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ageydvic.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ekxfajdw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kjeyutzb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mhuruvub.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vyutwuyl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vooncpjv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bxpkvtdo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2icuwdhoo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2setbazbc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sxznfmhf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2afnwnzss.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ubzqgtir.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ultzryxf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2imljgrbt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2odysfnjh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2xjyffqsb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ymnzdkea.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2toomhbyi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2iuriocvr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cadtwasr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rcwszvri.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ljuxzysa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2leccetax.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hbxwtntt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mysondhl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ssurohph.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2owkuuilz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qlqffepb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ktvzuvyl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ktwiqdic.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2osyqxjhn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2shqvfakz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2admwjqcn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2bltxdlma.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2axbtwohp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rzdckxqa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ljcwhwcb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hgydjjut.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dbobjupb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2mamybkab.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwyrwpyp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ltzbemrg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbcpelbu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tioyqlna.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zdskkhtf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ywojkuuw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ezvogdal.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wkbpcpjh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wydkdtkv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mhnuwmdk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2skjkvcmn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2otuhneib.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nssbduzd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fadpvsdy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2iykaftbt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2mjdtuqem.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jcobgasi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2slhuxrtt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ihzuimpp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ucdaekau.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hazqokiz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2uaddzfwo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dmwoqjbb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tzvgwach.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vsqbvgfv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2gwrpxqza.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2akpppoif.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dxolsllm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tqwmrkeo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2sqrywdhl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dhaoazon.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2stanlbgq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jujtiked.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oetxbpar.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tvudspai.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qdnptcop.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yzabcsrl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lskkyaol.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cqulqrkr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2acbjetke.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ocnygkuo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rltalxij.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ixmsbbyt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2chwhdczx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gixwnkgs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fekebaec.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2npjsghhk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tludyptf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cidtdblg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dqiejael.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2xfmoymfj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2olmxsyua.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2iglswiwy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2oazwijfl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ossbjxza.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fgnypzon.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qkxgqaaf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vnhhmmxq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uhwlcbhs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2aamidywe.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dunhbkyz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2suxerihu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2poxwtmzf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2atmiceoh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2njvnsgkx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vumcstso.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fdtjgavw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hqwgfefa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2eguwbkix.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zlpehuox.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cfhpgaks.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2arfdfere.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2clkwdttw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2brwldrjn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2onhifsys.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ytocgubc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pgcodula.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ckfhyccx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dutjbzvv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2cdyoexqt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2uyjzfjaw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2keunusxw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rvcjrjma.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wtahqbun.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zndcdymi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kojwlrjd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gldgmusj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rofhqcys.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2apyicmll.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lyrslfus.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vwshmrjx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wyxhixgl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opvuwftr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2hchykdby.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nadvuqcg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2sscmpjoy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fxriqbfl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vfiqygqd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lnbmtott.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dpugnxki.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wzkaspmg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2itqhkwsp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2zhinqubd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wpbzlgld.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yzklmjlt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hmdcxufn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lqvxbrlu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rjqilgmm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vdegtder.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fzilspzi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2smafbfil.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vvmdjwut.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zvrfkdrn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ndfiynyv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hdjpsnai.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qkmqatfn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aoacikff.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2nxcrfjcz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2oorrlaoa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qfabfbzl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncabhaei.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2urhhlqde.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ryvpizhj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rijqcpwf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xqiligyd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fyvkbteg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lcpspljw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fqzmwssz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vjrziscr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jjbawnlq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yhujgwwq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2sibvcqpk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2founepgu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pnhjjhxx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ssyhdgai.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qccenoya.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2htwzjxae.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2uhezygxn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qugleooj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2lxoirgcx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2byhgnqlt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzkjspwc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ljpvmbzs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wsrgrgyt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bozhlzpq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nnnfmqbr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tdaxwhgs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozuakqml.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mrlpoado.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rthnwplw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cezorpev.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zrsyzbbd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zqauchcg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pcpyuzpd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2anghxcqv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dzvomadi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ukzhwwvc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kgleukor.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2epbtbniu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lrehkaql.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tfjrmcuk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jiyqlrpv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cfzjwmpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mblwaxik.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2gawycwkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppaquqyg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lrovkrow.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2svadetfh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fiowfvnx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rfinmjjh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zhsgvftw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2twtuqmvt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tifdpubb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dbdwueub.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2umxcqxfq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ukfpxlmp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gvwonlgj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jvndumgu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2grawyowh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ypmwppsi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2uvwhidvj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2cgdgrbcl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2cvvbvgwg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ajmeivpe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2eeogyiim.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qshqfmbd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2falwwlhs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2zgilijfi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xtcfhngs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uamlsjol.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gvgvnsri.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gncnvkuz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2uymcnsgt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2astbmhuc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qgnljovw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yfhjppvc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwwzkisv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2agrbhrgg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gyhkvfaj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aoykkxnk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pwfzdzaf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2fmzvrheo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2eypqcujc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2fuetzesd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcksrasv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lswqnfld.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pvoiggqk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bsnkwkhn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ghhcifrm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2cchamsnw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2chyxdifz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2olsdufsj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vugdqcvu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hjilgbrk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fmroetzx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2aiekgrhn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dvylidcb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2szgrogqp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qdlczdnx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2nyfvvadd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lvwqgvlu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qewjjsww.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nsenloby.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hixrjggx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2sqtufnqu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cilrruxx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tdwgecay.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fqsmucpn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qjffefnp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xojsajir.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rfmvqqqu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fafboovl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hsjyojat.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2srjdcytb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mzxyeicn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2sdpfvrjb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xnaweoam.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mfzyfiaz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fxobeflv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fqspdfsp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ozwohtrg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vewjcyqs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tytxquoq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2aoxgtuwa.html


<!-- 参考信息 -->