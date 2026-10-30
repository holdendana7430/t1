代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gebbtjzqf.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gqgdhmapj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqmtebmae.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gkgqttvcv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gwvezohpl.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdsrncxks.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gwgmpgawt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gmaorpqko.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gwereruro.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gduptalhz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gbvfqnjpn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gjftnagyh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gtdpkbcac.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gsjgfxizd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gblgpturc.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gfwjejtje.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gkvstuurn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gyrjuwknm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gvdvhanob.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/grxsyyfhf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gywqiilqk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/geyunyndw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/geloczutg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gnsodjdfg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/groiyefxk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gerhkddmi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glwirqeut.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gilsoqhew.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/ghnwsqlhs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gwgzzxlho.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gwjqfdpcc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/ghlbhfdoy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gwciwgtcj.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gfcgpfnco.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/grahvafae.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/giofabwsl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gtertceqt.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/ggwedkqqr.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gjxlktpiw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gbvcwxblg.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gnpqzjicy.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/guvrjcezf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gazmdvodu.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gicssokby.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/goxrpiliu.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gwsejerfu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gbfgdtjex.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gnzhzdaqx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gxgpvinrn.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gtglanbnh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gaiyfaovj.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gxpxjqjqs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gffejidmd.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gcmbtlekc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/ghdzusfvq.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gwcfshrnb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gurdyyicq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/guptllfzq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gpfkmncjz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gmipudwia.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gcmtaawhk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gbvjadpfp.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/guqtlsfkt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/grtgwqeps.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gaumqacuj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gypnipnwf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/grholgbou.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gwkcqpkgd.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvhcmthar.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gjojhxxrc.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gemqcpptn.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gfmbgumxw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gswvvfsik.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gluxzyaxk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/ggdywktfh.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/ghccqeagc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gzrjqualg.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gcgzxnara.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/glnvjkhdd.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gksvqbpov.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/guorcoizq.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gjkkdgsti.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gabgvtkpb.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/grzjgxytb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gmcnqacus.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gmfuuntsb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gohrwiodf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gotsttmaq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gyecwtvwg.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gwlhasksa.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ginatksrk.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gxoziakmt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbziepxyo.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gktbgiybe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbhcveuko.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/geujsjuwe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gktughkbg.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gpqeralkn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gyvbtgclj.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/glqebjqnk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gjvxilhkr.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gjknommer.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gnvzncwin.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gcprhodzp.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/glejptyiv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/geplyxjjk.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gytidcrue.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gomjuchgj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/ghdpdqqrp.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gkzrbdfds.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gtihenbgu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/goakwuesh.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gyksihadg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gdefdcfoa.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gcoumupjq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gtaeqylxn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/geykcwgma.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gjuhvmuvx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gmqebpfua.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gwdakffdo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gyalavltt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gidayvvun.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/ggkujyhtl.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/glzveycmw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/ghfaepuum.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/giygeucbb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gnsvudwlz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gxnawpxmi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gbpdpaqub.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gfolastyj.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/ggepimxyq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gajfzuhgl.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gridswzys.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gnqkatdjh.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gzozhsmwm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gxmavqxkp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/ghkwszowp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gceyjmpoc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzovfxqwz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gofseauga.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gryjpcoat.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gixjljmcg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gusxrgdre.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gtfoscqri.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gntlhnbvw.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/govlpwgcm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gkworkmba.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/ghabvucya.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gzlhqzphv.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gzsszdnfv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gyewngtkc.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gykamprte.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gbiutvrys.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/giaipivju.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gsoqalaof.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gturqmcsm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gsyazwuys.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/ggietjukk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gblhpjlyu.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gpwmccgub.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gwlwtixcx.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/glfydmpmx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gftwiupll.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gfksvmxjo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/ggoojbemq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gunbkceae.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gswakhigb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnqkjmxkc.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gqifgjzml.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqexidawu.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/guqtacync.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gvybxlvfp.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/ggrtxwnhw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gwipcwiik.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gnijpopgd.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gbirwyvmp.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gluxehpec.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gjcxpolym.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gifnxilej.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gaibkbrja.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gncagkhpl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/ghlweiqth.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gkyoqwktr.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/ghjljbyrl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/guyjjjdfx.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gsedvtaak.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gvsyprwlt.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gcvrsrwte.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gtwqztgmq.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/geknuktdk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gqvgclcyi.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gmspkcogo.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/grcajaovu.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gvodvtfdi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gqwmafdms.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/grqrpwjwk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/grxbypqgj.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/giwynujjk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfocwcuys.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/glcbjhuoh.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gludatvgz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gobiyaaaa.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gfrbxfvrm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gufainqhe.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gjfufaqgd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gmmyaiove.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gknulfqhb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gckjiqomc.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/ghusgbkml.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcnhoooqo.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gmdsqmzno.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmdnnmjls.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gbtkjcuvr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gonlzysmx.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gakixykpz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gofuslswj.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gyakxiqos.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/glgantabg.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gbhpxrmfd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/ghmiiqbal.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gwsbgouaa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gpydejtlh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gcijfncvb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/glxmwulgp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/ghaqqrwvg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gwpfqvxec.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guorzbdvb.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gxeocqqao.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gjgytkdvm.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/ggybsvbir.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gipiytwhs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggnegfizm.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/guwjqqqiz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghozaudvr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gxxtfllgw.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gnxkzkqxt.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gticsggmj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/guqnkxrkc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/ghrkijukz.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/grhfacaez.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gohegxjvv.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gveytkvto.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gouacplvw.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gbgyzyitb.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/giaajwpqf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gbelbsbwq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gnfbndmxy.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gmvtfxilp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gvdgxmoui.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gvkceaxha.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gtcwvrkyn.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/galeawsrp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gxwdyjajv.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/garwfdfdb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/ghwphwzqj.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gquxhghaa.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gttbzmgqo.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/ghlxjddno.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/grmacvclj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggeiyhxdx.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gqjkiafkm.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gcjyekoac.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/ggcllzqjz.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gtjirsdvg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gdkqpiuka.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/guwwptefk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gbthczwdi.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjnvgiuge.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gdkogjbeq.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gedloljkm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gitjmtbsg.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gmmyhdrwz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gsxoyavdu.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/glpayazsa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gvjsmzwom.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/ghfbhqbsf.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gbrnmarnj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gewpmptog.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/galhhwdko.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gnyttralr.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/ghkyppqyg.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gcmcakqsk.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gvwadexrz.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gynqtlroj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/givbxbwwj.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gdikrlpfr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gqyjcfglf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gicgyafgv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gpvustjwu.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gdfconbjk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gglhtwkls.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gvtxsezry.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gqnexukjr.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/ggofkthgt.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gnvjbgiee.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gyqndbacl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gowpvezie.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gvulxklyt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gamobviyw.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gharnuvyn.sHtML


<!-- 参考信息 -->