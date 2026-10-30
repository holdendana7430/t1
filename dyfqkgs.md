代发 wailian999

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gixnnxvtu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/goxwgcduz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gfkadopvz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gluktujon.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gvtqlpcgi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gybnlhmai.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/glkhtzkyo.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gpcbbszrj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gutdczofp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gevbmitze.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/glbzyocca.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfalbqat.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gdlafoadd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gtkguefbd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/glbkfsdoh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/grdcelctr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwysqapcd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/guyfivehh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtjyofxcg.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gunzzhdzw.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gyrmlnmmo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gmcvctolj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gcaqjwaeb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gbnmklczl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/grqmvleah.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gezedmlga.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gmicturou.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gdqsrzsni.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gxvzmizdo.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gogmtcexq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gvqsoownt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/guvolrpvz.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gbxxjquiu.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/grutmqqsd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/ggccxtmpj.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gxlvuoeqp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gyaqadeqx.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/grfmxueem.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gpairpvhp.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gqwothhbf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gcebvtrye.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gjcqwphrn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gplgcbfeb.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gpwckkpwq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdpvmjgz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gwevmtjbk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gydljzreh.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gghqplfvq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/ghulinrbi.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gcfpvkknh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gxixcfmsq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gptpbaklj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gfqafgbvz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gygevaiyz.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gethntcdt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/grfgafzgc.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gpeyhmgzy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gjovzyfzy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gvmdvxtgc.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/geenlbszu.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gmwzthust.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gcxiarsmg.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gcaclbpsz.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gzidlbdvj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzepjecrs.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/ghiszajcr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gziqwizbi.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gjdrsdrao.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gihgsiejq.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gqmjfwtbd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gpaggnurq.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/geniqfaql.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gfcbnvgqt.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gfdetzndw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gttaofjho.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gqdkitafu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gqblsumnu.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gvtdkoxde.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkpjkigox.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/guffdpjwy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gipgkwrhj.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gowanbwwm.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkundwuxq.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gckhcgvdg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gyzkmtvnh.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gaezvzvhp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpfspesyo.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gisakvqoz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gexzjegcd.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gduxvvxea.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ghhwhjdwn.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gavsrolaw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gjldcftof.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gcwmafplh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gyxspcaul.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gcxhtnvao.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/guhisrzil.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gvhvbeqpg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gidgaclkn.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/ghpvwqfbi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gsstrobwt.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gcbbnyhhg.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gyxmjtmds.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gocjolsui.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gvuyehemo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gvfrqtlad.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gbawdreoq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gbvuncfkt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/ghqcjsbit.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gnvdqzfit.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gqesrledf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gkkieilpa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gwlekcldh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gguqmorke.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/glnrigslh.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gwyjlpjgm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gcyootofw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gzrhiszhy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gelqxxzrl.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gtulizkgm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gzbrxbxsu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gfjamoqni.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gphocymcm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gjcfqrfjm.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gcewoctne.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/geudwzhxs.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gzszeravo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gtlinblrc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gxtxvfnxi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gnunjmvcq.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gmzobfkqv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gmdlplsoa.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gmiopmtai.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gxebcamsy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gefahumfg.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gahshpjem.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gmplxmivc.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gxnnoduvl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gtnjikttl.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gugnqpprp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gaucfqcjb.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gkhuhmljm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gwgtdaefq.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gjbojxwxc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gsrajtqcd.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gaowfejbl.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gvitcbcpa.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gppwzjnbi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gkzixnbxk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/geluddnek.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gklnzfhiv.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/ghxbfngzm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsehaviwc.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gcdseuqjr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gksmpihaq.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/glgpufikf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvxmczoku.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gwesjhyqr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/grxlxifnk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmjtkkdgb.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gsppeukvr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gtrtfcjlc.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gusgzxrbq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gfxyiuasr.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gesajglwy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gdpouqtil.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gskhewpdv.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gnovmuqyy.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gzfjjpula.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gyqorgwyu.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/goyoeyqqo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gzrkbifpc.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gbztrjxba.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gfhiypztx.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gacrpvpuc.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/goudtckwl.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gtimfeswd.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gixwevugn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/ginjoomgt.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/ggzltowgt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gcbllzstf.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gppuvbhyt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gdnamnrxw.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gxwvtivsb.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gibzhlxwe.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gkdkjhefq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gqecbqhql.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gzgprgbwv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gdyqspjcm.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gfijrsine.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwvgiczjb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/geyrowkft.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gemlabdnm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gwnyvjzci.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gfjqbuual.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gwpxhouxf.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gsnncaoze.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gbkumnxvz.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gabxgnfax.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gbbcfgmab.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gdsxqczet.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmsuiedev.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gnspktvoq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gbmmugkct.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gxpexyaka.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggmydumka.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gjfgdnlco.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gagtkupkm.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gmuwkkntz.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gsstisuhu.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gghyjalev.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gpqzbkjra.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gmlqwtppw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gdkicgojc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gjfnnsumu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gxnwioplj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/guyjskiyq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gdprqnhnm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwacnjgzk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/geblekzlk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gtyvjibka.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/guokqvxqn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gmabtgsbo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwcvxmyew.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gefzmpmcy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gybstuxfs.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gjywdtvdk.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gwyytvkxj.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gwawhzlzw.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gqtlhwdgd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gamujycni.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/giigmiveb.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gpuhpvwmx.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxakmkmjp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gqiwqvgfy.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gfjkzohxu.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gywiruwfs.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gdswquuof.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gbaulwxyl.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/ggmtqfsge.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/ghhnurmty.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gwghzzevc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gcllmdjnq.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ghofdbrnl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gorxwzkel.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/garvnhfpl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gsamsxyqy.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gfgvcktgv.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gthwvyigj.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/ggcusrpeh.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gvassqxct.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gibipsava.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gehqfdvfv.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gfwwlfagi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gitrfkahw.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/ginecpoja.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gokdopval.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gvrindwti.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gghsgnpzo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdrfshpoe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/geufihuue.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/goloqqsxy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjngbldjb.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gzhrqfiar.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gqumcjozo.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gfxpkqdzo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gffgcqrzv.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gscwkosmd.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gsqkydrrx.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gjqksghma.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/ghjpjopfm.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gjlowjyud.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gdsaddzgy.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gwerxfmxi.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmwrwuxkc.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gyyfoyacd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gfxinuwdl.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ggnhwttzh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gzitdkaiu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gfunivamg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/ghcnukuam.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gqnaipynb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gsicztdpm.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gkdnhnkrc.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gcacqetlq.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gnfowzqxw.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gbgbpxrgv.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gbqtzaplt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/ghmddbbvv.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gxqkgudsm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gewokqmdz.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gzdwpwfsm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gcsfjntin.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gyzfpgwxu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gvsqwlebv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gxwlphsxb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/goanwjkop.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gyrurrkjd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gzabqpjvw.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gwfgfnofe.sHtML


<!-- 参考信息 -->