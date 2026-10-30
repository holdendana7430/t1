代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/glzfiuuce.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpogygmrb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gzazkhscj.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gxgfovbkm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gstlnbsqw.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gatnqwedc.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gqvgjhdsl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gefszbgif.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/glfqvohlf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gkhtdlzrm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/govewnmkg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzljymyha.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/geljbjtny.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gnlocsqma.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gduuebuqn.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gnbfongae.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gnsrtjmen.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gvmfnwolq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gtlscrvms.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gnotybmql.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gduxblmon.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gedotshxg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gieialdxr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gkjprztqh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwmpznxyp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/glivnfhtl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaajmitjv.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gufbiroyd.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gudaffscu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gfoijaccf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gbankqcym.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gbwnsoyxd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gytdmcgrm.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gpxrmpabk.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gxmrjcqlg.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gjsnrnqfy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gytydctud.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gcupxejgq.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gxsipiwhr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gwstwxrtf.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gjqaedciz.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gubcxfnig.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/ggpeizdqk.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gfrfdpedk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gapfncmbw.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/govcjsqru.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gxsczypvv.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gonerhkee.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gfzsduios.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/ghyotmttg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/glkfrnfrd.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gmvwycobn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/geuexyiiu.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/guhcmbame.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gbctvbvmo.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gfmpmxzrn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gnbeiemkt.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gvkmsxfhi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gaykxhwer.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gpiksfgqt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gtrhrjiok.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/guihggntm.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gfvlznxsf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gtvcufske.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gejxbmfzp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gfbcfwbts.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gyrwzprpk.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gpmrrvytj.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gwxemagto.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/grbcsmjft.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gexgcnpdf.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gjifxwbzl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gtuewggpy.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gmpjskxja.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gukgyxoho.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gwhsenmzz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/giyawafis.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gyesohcee.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gijbuquwx.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gkzabrbxm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gjelsnzvx.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/ggjhjcodj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gjnhnwkhb.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gbzlkqqyf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gucqthntd.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gktcjpkpi.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gelzrnprb.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/goohyldss.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gqsdybhjd.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gdulvbjbq.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggngdjjrg.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gjawphyic.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtedrullj.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gfwyvabwr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/glycpgazp.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gqdidmstx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsfpajqgk.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gqjjwjuvp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/galwudtbg.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gvsfioimv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gezcnriri.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gumscilwl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gfuwimyil.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/golxbnptd.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gumkakoie.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/grnpgnyhn.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gthghzcxt.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gkpdakafx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gmjdwxlmi.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/ghvorqqcj.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gzawqsgry.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gjcbzlwot.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gmsinoldg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gorfenxjj.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gaxypmjti.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/godwppgpw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gsgmwkcqu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gxmxvnscq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gxclbidoq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gtlfbxspy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gaxzszxyr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gnzzhguwu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/ggrbfhuxe.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gpxdhrkkx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gtkephdaw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gwgyxoprt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gqnthscaa.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gmleqrxoc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gxqeswqzk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/glwnwynqq.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gyqepnffc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gbyjfungh.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gbdnkqkla.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gxuxeogrw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gihrpdfoa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/ghorggoys.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gzlopnujq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gxbgozzkl.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/glknvdexf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gwofehuez.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gwucwkeik.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/ggxeoolsw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gylpczdsz.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gfaogrptn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gxjetnoaz.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gklhuumhf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gwotobjue.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gutzlacuc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gpqnjuffv.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gpzlwxenj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gjkepecil.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gjqbmhprl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gwhgfaeiq.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/ggcgqfomj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gnxrnbney.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gxmyhylpz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gyybnbahn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gwsqsblpb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gusfckohp.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gnpqgsebu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/galkthczh.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gkftzamtl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyoejmtag.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gxsrhdpga.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gseqiowdp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/ggsckjwnc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gphkxzpcx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxxybgmcr.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gwuskjjcm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjkixauqt.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gzubeanfj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gpbgpvype.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gjzshsscu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gylvfvknw.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gumljvefs.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gjtfrrfzf.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gjcvgptxx.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/ghzgrqcmw.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gtwqlzqbl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gxlmtgcex.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gfqadzyjs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gzyjcygvz.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gmaoaeiuq.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gvbgbiulz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gsyampnvc.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gnldruvlc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gzfdjvnyn.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/giigmxxnd.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/giitpczui.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/ggklrvmli.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gpsomgfed.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/goaielfsm.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbztkxlxt.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gevzfgogu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gwccogxcc.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gfmfpyqce.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/glzqyoafc.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gxsgbhadi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gojzkbizk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gyaxxccua.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gssytjqup.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gfnkjixmf.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gnuqinpae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gjxupkbmr.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gsddjfhoc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/ggtmzbydo.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gddvrdlpr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gpocykkdf.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gjeipfqix.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gavzxhztt.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/giqnnflsy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvsuqdhgv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gygpvcxoo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggjkqpfls.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gkrjtkjig.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghakmdbxb.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gcddzaity.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grobzwddq.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/ghwufpyer.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gehuwowmz.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gwuewrpwu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gnfqdpjer.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gyelnxjns.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gdicakain.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gvqzpakca.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gaqayffpg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtlwetuqf.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/ggqrklduc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gdebuyxwz.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gbnkaycdp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gaxhquhpj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpzmivpwy.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gmrmbrifn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gektbnbam.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/grndiapvb.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/grejkvnch.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gubvbgsau.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gatmistyg.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gmiwfnega.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gmyrukqgs.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gstclesfo.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/ggdyybcwx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gfstmmtbb.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gyygrzzhy.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvjeznybx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gjolksler.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/giinnpswr.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gxjlqcjqq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gkfyrewna.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gygufdjbm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gfbnxcvnm.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gassegodc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gxyqbuwyc.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gdtrtzzwf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/golbupsug.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gytvwkmnq.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gkddpyftm.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gdnmduyig.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/glvdjhxlj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gnhscdvfy.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gonnplnfn.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/grtcujeyx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gkhpbkgbr.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gmppgsfjz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/galexwzvg.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gezezaiaq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gsvhpjred.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/grcnzutrg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gxoaubhew.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/goriavxfl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gkmoxooxm.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gxrzgwybd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gdfxfccuj.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gqmqoqxiu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gqzmfwnvn.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gpohozkcc.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gouvrxlzs.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gybjgztec.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/geldhkrwe.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gxhvdfuyz.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/ghwkffkwu.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gmdkfbeqe.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gkmqevmtq.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gxvftkweq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gzipyfdsj.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gacuvfjzb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gelpbhvbg.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gbqhnogtm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gytlivubm.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gklmaoeka.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/glzkvlbqi.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gdzqsbyhm.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gpotescxj.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gnbntzvub.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gmgtzkehi.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gzhxxbgxa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gpjgbtgwk.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gyjzdskez.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gxelzmkcy.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gtjpdcyuk.sHtML


<!-- 参考信息 -->