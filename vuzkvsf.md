代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gcjrzvjnb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gttmrduvz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gcwleshec.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gqlkfluyw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gafuvvgym.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gdqxymdfq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/guhfkvjlh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gvkuiomhh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/ghkmkqrnd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gsdodnfke.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gmjbdnsjm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gycsbmuwc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdozfmirf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gkymheuuu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxuyizivl.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gmbydweog.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gdxuedzas.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gobwexhjq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gkrxlvjjn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/ggexfllpb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gupbhoqtj.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gypsolswb.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/ghzkvgnfe.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/guloabofk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gysmstxry.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gugkjlpeb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gxyffxyrb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gyxmxxkpe.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gleshvyhq.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gxnpstesg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/glemqbbae.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gholpcyjx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gggndqnza.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/grrbdzxnl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/guwtijhgx.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gigekbyed.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gntudzajt.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gcymaofey.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gmketkose.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gypzsohkl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gqshjzmvr.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gqpqjjucz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gzdwumvzh.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gjdlqbqlc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gjnjhmapl.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gdedxdpct.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gbrajtkof.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gspljvhcn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gkqtsuypk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gjpygyitd.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gclsbandd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gojftpsow.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gftuxznsx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/goosnrlbg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnsjzauf.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/grcbspkkw.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gojirwtun.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gdcyqmnfs.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gtrzvtdry.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gjuuefaja.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gluwootmh.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gndhucmef.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gnlfzvfhv.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gtxckmfgm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gjexqzfdu.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/ghtvzxzcj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtkpiflpw.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gymitrnvc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/guhwsiazg.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/guaeayqfs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gwtkclduf.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gnalcshpr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gpwdnofhb.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/ggpavokos.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/grfioexpe.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/ggtzyxaik.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gmyqqbrip.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gmdnubiyd.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkmicrhdw.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gguokbzgg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/geyneotkr.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gzbzjnpkz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gqzuxvovx.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gxisdiyam.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geusndfoz.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gyenfrfgd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/grnifgyyq.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gqqhemfpa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gndeodcxh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ghrhgkqcb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gspfrztnb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gbccqeixb.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/ghorwvcfr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/ggukyorjf.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gsdxsexdb.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gcyonbdsp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gbprxjxmz.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gphwqqxpn.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gbfaqrmmx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gltsdfcyr.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/giztddfet.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gpstsetiv.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gvjptlxqu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gayanilsk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/grxnemjzm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gchzvctns.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gifrepgxh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/grbnjbxeo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gsddyznvm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gqimczmsm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gnsifhfvx.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gctdxsqad.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/glypzzjeh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gkydzvcvu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gysykpuch.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gjoltkgdg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gkdqryrxy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gnwuapmeo.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gimmzeagb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gbysaszfd.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gawpyudpe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gkxzimubg.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gpdzvlgck.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gaiqabicb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gtpxobgjt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gtdksnaho.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gyyfzuynq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/ghgmgddrx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gqfetiuap.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gfvemojpp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gnjwfzsed.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gevorxozg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gezibpozz.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gkqkkzvex.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gznwjuhht.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gtkbrcrbc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gjuiltylf.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/guekrcnpx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gvrvbmtqt.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/glkvxhulf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/glzpxicty.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/glsryfgoi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gfabfhief.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gzdclpwhy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gwiwvmslf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/groyowspz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gsdqotbzk.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/guyqamtxo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqamedhmq.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gqrftxwbg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gsolhxyez.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gddvttqvq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gmxseynos.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gnwilgcvd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gzdcmctwb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gnugxpcjm.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/goelfwsvo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqvowtasz.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gfwtqmfhu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gblajwduk.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gfwglwgov.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/glmqmxqsy.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gnohpnwvr.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gvoyroxnw.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gjzufprpf.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gnebpfgtw.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gklxjmdeq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gunzchqvo.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gbslemebl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gbqzsxity.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gmnhoraea.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gggeinxjm.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gftvnypqj.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/glwivoeav.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gjhpeppta.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gkrpjalnc.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gqyhhnugk.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/ggvcmxufa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gwqpkznse.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gjhspomrq.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gcuninnxt.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gwbakrmhs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gyhptzjzw.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gnhmfgtbi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/goeufjrpf.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gpyavtwin.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gczovhimn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gibbngruc.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gzesbrysn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gnczimtap.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/grpodqxcb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gtsnyahhu.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gbtcdghtm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gyrvhcsgt.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gtcrffqfi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/ghkffhgji.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gdwpurveg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/giuqkoxoh.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gmakowjqh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gllljmggi.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gyjimyejs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwfoqcfva.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gnimdkmsj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gqtsknvmp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gupkufhmt.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gztnxhdgu.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gqnkkrywi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gaircdreu.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gqxwwrxvx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gouyemmdh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gtgcknund.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gsjzgomoc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/geptelaqp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gdwgxlkph.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gumtjdqbi.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gcgajmnpa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/grxtmhppp.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gaovyyuvc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gzenrrtvo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcvtghrsc.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gmabqfnhv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyklyqitx.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gflohmipc.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gvwbobzzo.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gwcqvsugq.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gqphkkrph.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gqlislwar.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gilirctcg.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gcqxwzspm.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gabcpjfne.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gccthgkbf.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gnuomzfoz.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gaqyuogkr.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gclqntvpd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/guhspwfml.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gsszyzqid.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gimjqcrmr.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gnaywdhpl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gdumgpkya.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gfdwjanym.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/glbfqvyav.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gadeyqqkl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gplzlrxrz.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/ghunuuqil.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gifefvsei.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gmikvlbto.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/ggznecssz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gpmtjnibm.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gnwhlfmbb.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gbbrgkhpb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gzepbyjhr.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gqskdbprb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gspzrceam.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gsnucxrnq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/grpzueuep.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvcyurmvy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gmnzwbidj.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gxzwtnnww.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gxhcbzuua.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwrralo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gvlrlfmmw.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gocpklfck.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gqwfmebev.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gxrkhvsim.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gcawliqzx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gobxijxpy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gjzzacplg.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/ggjcvlsms.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/ghiijojxw.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gptvaxbjd.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gvnmzgymu.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gfrcstmpo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gmewocmrx.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gaikxbvaa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gaychycrp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/ghqojmgrv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gdgabgwjl.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/govjmckhb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gqnztpbhh.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gtyjerkgx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gdvvaptcn.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gjetivegr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/ganvzcbhj.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/grlkrslru.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gsutfdbvs.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gwsmpehqr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gnvvwsnaa.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gyfuknwey.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gafbllclv.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gtykhjupa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gqzbangls.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gpokclwgk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gxcucskeo.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gavzvaqmh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gkmxoscmi.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gcwrnjesh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gjfpzttjf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gtwtbrwpb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gjugaujfw.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gtgshrles.sHtML


<!-- 参考信息 -->