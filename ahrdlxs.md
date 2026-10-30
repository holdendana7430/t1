代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhavuofl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhqoknfb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fanxiaobao.xyz/Article/details/grlaxvckx.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fanxiaobao.xyz/Article/details/gmgwyzmir.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fanxiaobao.xyz/Article/details/gurlvjvyp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhoyafsk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdopneabe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtomewbmq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwvqgyad.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/geordzqch.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fanxiaobao.xyz/Article/details/gelfnlxss.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqwtmcqr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjzzxjex.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvymsbkpq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcjiyhter.sHtML

[Q01] 创建表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdpfhtlx.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/gadplukpq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gqltezrcj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/goeirjskb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfqraeuy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gpeevghsz.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/guianojsh.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gjscwnhec.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/gromoonzy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/grnghmdya.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/goeccfros.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqhteauj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/grmfsyjns.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoemznma.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/gvegwjzhf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gympoqfrn.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwgbvtkea.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gmlhyroxr.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/gpazmxsye.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkskxzul.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwgugzxl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmnbmlho.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gguudzywc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkopbrrl.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gbucvgjur.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gesmmtqbw.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkdgtcmz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvfqpppo.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/ghnargnni.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gpbzxeodj.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gsysswzkb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeaiyhre.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gopsrjcas.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfesqmypi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gkqzanqbb.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/ggzxiqfpo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gvpmiynlm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfglsmgrs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhuhwyr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gqbdwpnfj.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/glwuvmidi.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbrfgdocf.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/ghahnnqyu.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtwtgdana.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdggjwygh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoiuqqtd.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ggkqzvreu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/govbmgsit.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gqbvqmhdy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gmuftkegq.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdydxkas.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gugblpntn.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gbqsezgzm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqwxcnfw.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfxjoatxl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gfqdmclmo.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/ghloexize.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcolgcxa.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gzimkzhyx.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgmhipfz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gngxiprqs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gxhdnyqvo.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gakpxquax.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtcaiited.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gppzzicca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtcufypii.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gnddkysjq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvswuysio.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gsyeegxla.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwscsvveu.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/grxdohoag.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gccmexbom.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxuosaom.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gguiymsvv.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkamrpedi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrervoei.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/geilcaaem.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpugpfrvp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsjwpijw.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gdvwrvuds.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/grpjmttkc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/glkwgbhsh.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkovhryj.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwygslrnj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/guskyuqjp.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gmkmdnsfv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkmcogjp.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gjrjptpwu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/googtgqoi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/grutoaxmy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbhwjyoc.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpzotosc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwkdmxui.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnickscxi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gvikpfhzr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljqlmcep.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/guronpgpd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/guxflmtut.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gpkbgfkgk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/guvjmgmma.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/giqhzzvqq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gwcnfzlcc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gigikadhw.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwrydduh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpqwxagh.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gjguriqrl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmslkuri.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gqykuaako.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkgdrmas.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqxntjtr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/glppygqyu.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfiyvwsnt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gjyivvcxr.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ggostjscn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gpvgkscvf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmatscswh.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gwwsstims.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkbkrbuz.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/greuafysi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysmhmwgw.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhvluxvj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszkqynyx.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgylihkv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbtuqhzx.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gtslzuxfk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gviffjczt.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gxxrcqidb.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsngqaxr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvvuexon.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfqzjgpb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmucpfjn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzxnzomi.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhexuydl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpcczyph.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gplqyfipv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gvirtorhe.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gyltvscnp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/giruifydi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbswxehqt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/glflctzbe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gufxgflet.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmtqlagz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxrjibil.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gphjxnhdl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/genrajptg.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpkuriww.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxmisfxc.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/guphmjlxi.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvgmtaed.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwjtwxrp.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnzznyrq.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtohkooiw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/ghdegsygh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqecbnsn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gsssmbpuh.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gufitmoxe.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvtafreh.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfdajrfe.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gtfwvmpbn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gzcrwpanc.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gezlrnuzf.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtamdvma.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gccejwfwj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjbeudbk.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gidwkjkyd.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsbbgzpz.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gyaqkkaqt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gkoxpiaho.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gkypoitak.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfdsnmpr.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gejtdbfsn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjthqoqop.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbysowav.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjtcjchl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gozfszajo.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gexzmmrdc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gzhyoczaf.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/ghypylrve.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/grozhhjdu.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmplfrvas.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxxoiycq.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gqodqkege.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvvmrics.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwainhfub.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuhephfi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyeuiora.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlmsublp.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gacophfis.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gplknchnq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlysevko.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsfscjyd.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhcydagv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaacpvyvu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzconbeyh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gocatmetc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmowwutih.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gszwksawo.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnhmfiup.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtelvaln.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdjgrckkv.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gmzveqwoc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbfoaphy.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfytxupzk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gwrnqxuek.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmdclocs.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gixyncvjh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glvfjamgo.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gyeobwvtz.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/glghukxkj.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdrodqnj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxxsxzpm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxskkdlw.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjftxczwu.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqlmclqa.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepsphraw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkuyhyph.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweczjmbb.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxjwtxlyq.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcdtsgfzm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidppibsc.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtfpdkifj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gobcdohix.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gvczpmaqz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gfkjfmdgy.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/geyofgdra.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/giywqhrgx.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gqskkjdmn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggduacuxw.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gakutyzez.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpegfdnsn.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gihsaavbg.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/guynbnvbj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/geximkbrb.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gqyhrrdkn.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjbompjmn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geiipvqmh.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gjacvehcm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwulpghrj.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gglekvjid.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpqytmilm.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbnpwide.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzwhvhito.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsxfpfal.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpeeonjed.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gprflwjfd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/geweslsdl.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqxwrsxd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyyopkkeb.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgnwpdeh.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeuglmzx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gubquxemh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggjoxvjjo.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/guhmvddxj.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykehcqkh.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gxhvnephc.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glzissblo.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/glpbtpgqd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbirrwnd.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlgiokhi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gceydfjsa.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjkxrddg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghyilpnzr.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpufyabra.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqwbfikl.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgugibjs.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gmjoiheob.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhyckjeo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gbyrwcydf.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzoarjbwa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzxbawvm.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gizpgsgjc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmhvavol.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrzethsq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdyebofh.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gkwoyegkx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glklpzfbv.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzhayvco.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvzatvvx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdykqbqus.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gdselhkcs.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjgvzkxg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzufdjurs.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/geggaduwu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsqkpjtw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwpxxere.sHtML


<!-- 参考信息 -->