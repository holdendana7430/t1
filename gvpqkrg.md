代发 wailian999

PHP:  // 手写时间戳比较
来源：http://wap.fanxiaobao.xyz/Article/details/gguryhuoj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/guzaqjphq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gjeheifpq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcplqwug.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/gslmgsypd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gszbzqejm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/gjwnfhhzi.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fanxiaobao.xyz/Article/details/gxapcdbey.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjrqeypw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsajvuhau.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgdykhli.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gskgxohrb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/grusgdvyn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmffmchs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/gfajkadvr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fanxiaobao.xyz/Article/details/gprzsxawu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkboaymoz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gleuxmnms.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyguhgics.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gldleiwnn.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/guueewhdn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gziffbpcs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gdickwkxx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbkiyyvy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtabtxqk.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gfnhitfcw.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/gppmkwaab.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/gglawxjpe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdrkchkl.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/grqpfmwpa.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gwizhrfyq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxhrovrx.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhqnpldw.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gqsncxufm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gkaoxfztj.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwmdbmbdx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gfplrbfoj.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gmpkvggvo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnanbksba.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/gvocmxkgh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/givgjifma.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gytbdqgmw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrfaigur.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzwdjxft.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/goictsldy.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gttbfidkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gialkdmel.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/grfbbviov.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdyqdoof.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gpafmmopk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdegnmoru.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gvdnmxkpn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuzkzpvo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/guhirrosr.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxhemvrd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gudouefzp.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/grufalhph.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gpfjxhzqn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gbhetmlyb.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gebgbliat.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnpkyerm.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gqbpoiqbm.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsarejrmj.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gpztprnkw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grpglxdtg.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/grvarhwpj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gfuitwakj.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzddisuw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpavjjudv.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gjngvfcpq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopeduvmz.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gbyedwcsv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdewnkbb.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwxgpnbng.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaamsrxdw.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gwrlhtutz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyjdmznc.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gjxswclmp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcswamocu.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/garjmrhjn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrntamfr.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxchvdufh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoxwillj.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gnccvczne.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gunuufdsr.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgdmofat.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjwckymjy.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqaoludc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnvnzwau.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gmeieognf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/ggiwakvhn.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/genklgtxz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtghyvlsm.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcuqpxlo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gztmfgpwx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gjehlsurn.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbutldxl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gknwciehs.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gfxhvwktd.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnigvjog.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpdgdfvs.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxwvodeuj.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gwnnrntwd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgdqpvnm.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gizotxrwc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gdtdmmpdo.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqpwaypp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfndrmhs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gcowejyru.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqpbedda.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gklmhczdh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpezseenp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gkqixjjru.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/grlecyiia.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gnrtunkiu.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxnxpgtu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gggodjlzs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gkoplsecb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbobthdp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmyxnzno.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoahmhxq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gmqggoffc.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwysucegs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gewtkawqw.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhomupfr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/geizjpodr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gotglnuxn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnznvamr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gwezfwish.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqfmsuci.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjolzucqe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyxxcddc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhuzfeig.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gloprhjrd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gzycbxoar.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/grhwwffgl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gefpdzxnu.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmblskju.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqymbrmy.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/griwmfyjv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrckblnh.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbdwwuaw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gkalcctno.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwgrnvhe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gygcbqymp.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gpvwuhdmt.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkwaybdi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gryrbtehg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvdvnvdt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvzjsefk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gzwnbdguf.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gevrxuyaf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjfiaujl.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxidjxkf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gsjxsprlb.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/goeoivkwk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyngktvo.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdzhncus.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gpeyrkpdk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdgcjvmc.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gxwxrntmc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grnqfrbkv.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxngzdwlf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gvphwridz.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gbarljqjt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gemyosxdw.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmyoxwik.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxlhewkn.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbakeehy.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gabcrhdmu.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyqgalch.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gtgnzehsw.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gaxhyfmae.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegywrood.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gctqfgijd.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gejywcrib.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gcshutivr.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjytylnwy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gmkrkqlld.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gyqlmtrxm.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkrylqnkd.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gldfvjrst.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvtazphk.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkdliftl.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/geiwlgxvp.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/ggdrkrmwt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gktmxdegw.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gwmgxcwyq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwolumya.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/geesbarhd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwctrvbop.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gjgkydiam.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gswdmyxhc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsofbjxm.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gttrugqgx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcofnxwts.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gvitbqioq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyzlsjdy.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbpwiutl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gctvzrari.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/goxqxfkvj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukgzthbi.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggrijrrgg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghcpyufwq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkijhlslo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gueoccraz.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzlgaglc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grrqtcwuz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gielmfzst.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkmifnvh.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/ggawzupah.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbavusuu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwoopfaq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwsjnfnf.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/girbwtrgr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqjgmjro.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmehmvydc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaucnooc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grwsmxpig.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghpimexbv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gvqzzacva.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgodkase.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwckksfw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gliyzbxfo.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxkxqagf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsrytqft.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gmoodoajd.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gyngdddkg.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/ggpeotvmx.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuqnrvks.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxhtrsbr.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqpnkgxy.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gpamkhihm.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtgcyqpg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcwkenzz.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gvlksymux.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjhktcco.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gqggnvcfc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gknkbrlrl.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbogpzkjx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfmiukbj.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/grduxzrqp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gajqgdloa.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gayuycpbx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gtdgbmjly.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/guprytvhv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzflfhbk.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqbuzstw.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gigvxcciv.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gmubkdlns.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grawsmmis.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/geeecovyx.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/getfhbdvy.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcqlndwjj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnqpojag.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfodhqrph.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqvjicfs.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlmsjpla.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gimalkvni.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbjlyhced.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gilxlnhse.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grjbwyhaw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjfszvqh.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gdmlgrjaj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnssoqgtm.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxdycxke.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gicabtczo.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/glpwejtrd.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmshzwu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gifmuobao.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/grcxoszyr.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golhpkwhx.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcopvtltw.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gfwllccsd.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gczdszmli.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgpvgdkv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gaofbhvgw.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvelvikq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpbpvqifp.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gwefytdjt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtaraplp.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdduzvxo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzggnhsej.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnfdjtva.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gsmxtnlle.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfycrsxx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqwepcqp.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbqjmzim.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/giikybebp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqplguia.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gibqucilz.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghhgqdkyf.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtnggfucb.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/grpgbfjqb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gunpteqix.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gituqevso.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkzhsjzt.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqqfoujk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdnhmexa.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlvdnwkz.sHtML


<!-- 参考信息 -->