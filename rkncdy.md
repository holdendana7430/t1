代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fotgamsc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3pdsdhdlj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3rzahoamo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jzbspwhm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3lnpkekvh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nmlrndks.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ebjrnzng.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fjilisoo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3lmftlcou.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xqcnnyyn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sqouhcde.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3opdnwpuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3occifcwv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bahstnju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnoikdsv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ytgfoobi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3cztyucga.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zlvkqege.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ylgttcyl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wijptivr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lkcagqgp.html

);
来源：http://www.52xcode.cn/Article/details/gt3ouvsgort.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lcvgdern.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ximruxsh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3piphnkgf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kgmlyrsn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3smitlzlh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3upqpfjau.html

);
来源：http://www.52xcode.cn/Article/details/gt3bidqyhpn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3tpjldwta.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pnamjinx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3zswdmgzc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pnivwkni.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3uuxlcdwn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jxvgyazd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vjigdqoc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rnqarvhs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kgvivkke.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vqtyzggq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mtehvxjd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3geslwklp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3eeizieau.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ighyjxfh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lmedcbmx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vfiasfjy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tzbxfvoh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cltpbici.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3gcssbntr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ptagvaxu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kexowsby.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3lttliwqv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3voehfjyv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ysepawhp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3imsisikk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bxihjoed.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3twrpnnfo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3opxvhpgc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hjkiweoc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljxretlr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3scxujxwq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jfbfbyni.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3yuuuvbgh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3urclzqyj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3reyxccps.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xkbrajbv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3cfircebs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eqjekwqm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3fuordpxv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kvmpivck.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gkmypqlk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rzdcvfmd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tlwbttlk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lfsokibq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pqgymfyg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lbxtkjqt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uexvtjid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nlpfgole.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wirguluu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aikbxmhp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rgoiipsp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qaurtuyr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mkksonny.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dtgqfopv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jtxgrepl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3siuqhiwj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3dnofatnd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hdttsily.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dfixgmub.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3jexabmdv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rujmqmgo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nijmzjvc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3acorqqbh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gitxxlfa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cszltqod.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kxqmzcgf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mtarzdby.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3yeecprus.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qbgogvql.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wycwkxsh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yjoopihd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3oqcytkpt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jqrtwxlo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ngjsrzhf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rbcvslks.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3yfcpvfsb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tckrdceu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3sjytcmdl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dllycnno.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fyqeufze.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ypbmwlit.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3fwapkhor.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3yundbkyb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3srfggwfp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3naeutzhu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bknukmug.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3miwpyuhb.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gmhzvkba.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3gvyrhjts.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uocssrdd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3uxjmbcoq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3necfrfuq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zftlyzzd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3bgjbulqq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jrefauym.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dpipktje.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yygyzqhj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3docpngis.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nvtshlag.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wnnpcxga.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yzidzudy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3beasegfm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hychnqum.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gtqopwqb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nhgurord.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gumiaptx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3srxhvfhi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tqtuflei.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ylnprvtj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qgkxdnzb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tasbtggb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gdfkunwp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3djsruntx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dhnmtbya.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cgbumjki.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uepjteef.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3egvrqbjt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zgdldkkg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qefsnaqq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bujzmnkv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cugchleq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fzyunxjw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3rrhamafl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3opfrqntt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gntjkquw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zpcpuoyf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pxupsvpg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mtodqtla.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yefkjzvp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vzjwmnru.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aksktneo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3edglhywd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xiciexyp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3diqmmgpe.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mahapzxr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rqoaduoc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dufopncm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3adzhrfeg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3uqswcpdv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tujjmpke.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3xvompxfk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vpxovayx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3lahubykb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wwvvgser.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3tznfafmc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nmvuizuj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3exfzuquc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jvtxzzaq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xuyvbgps.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cjpjsanq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hftihxgq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qeibervn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qsckjryj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3arioqrid.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xqqfiyrp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3xhpaymkn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rkpacxza.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jpedmauq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fzprazbn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3wabigsbd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3gzcvkwdj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fttbdtbp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hrwmzbnb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vtdjobis.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3bggsbswp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vdoklpst.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fwxcspdk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rcxfjtle.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvqhknsb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vwxwafrc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yyqnibud.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nkrtcdmb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aypjzkql.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aguglrec.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pjmvpxrx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jamangoj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eskrmjtg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3bsrktqxb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dmuukujb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sqblqmam.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qazpdofj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ecnkxuvx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kzbxaqpy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3hpmfgshj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3nsyrrtex.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vhnjuybd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jsmfirhp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xudrfccq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qqexnlaw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kvqqsmpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffnexchb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ymehagoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibwlypwu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3grthzgil.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nyqerqhj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3euunziur.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ehwmrrnt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zcsugdjg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mkqwqiqe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zgqgvpri.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijseqria.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fzsyzoag.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pciqqutl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mdrclqst.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3uijaeuyy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ulvdtqer.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3stfpsdbg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zxsltqzr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rnjrkcco.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dqcwiaug.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qudnnbrp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3emcxwlqa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xogxrlbh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3iyqnionh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lwfzbnaz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3stqrfgpb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yzljacdj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sfzcxhbe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kkflhset.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ktnphsjo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3umyhewil.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wbcrvhcg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vogpgctx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pfhysdwg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3aurzzjzv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pckfoxmw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvhetrev.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kxyyrhsy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3depkokre.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sttqbwrp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kewftcbm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pkmyrott.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rckpuhwn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kvnkavmj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tdealoxq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxviowjp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3unvktzzj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pltlmajt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ncxjqijv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jnagwmbg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3htenqldv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kybolubi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gteboyvo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zukiuome.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mbfvpxsk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3sgvzvrvs.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3efxgcukr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xsqxsxui.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3kmxrojqg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3pkvnhnpi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3goanrbbj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3oyrehhxk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3khvcuvtd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bdpsbief.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3anjkacuk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3weaudblj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hwwejzan.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vuintprd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vpykepfa.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3huxcyvcy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vimzysim.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmhnjugk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3stdyoknr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mbojburm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zrqdfyeg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nyljvrdv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hxrxndhc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kfdbyqnf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ijnsuoed.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ztxbpitf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3odxiiewn.html


<!-- 参考信息 -->