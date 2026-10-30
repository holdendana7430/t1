代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/giggtnkgo.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gllttvyie.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/glpmnnlaq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/grikfjixk.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/ghwoquqjb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gthrgaisg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gbwnvgtyj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gkitkbugz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gazaotcjt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gugvmsoqc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gidbfdpfu.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gktlepbif.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gwnijflmt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpoumuzac.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gihpxfaet.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gmxcgthst.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gsezgogeh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gvvykceou.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gqzvlnukn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gmnoqgntm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grehkxdes.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gvetppbih.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gynbyjukd.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gwvzdwodm.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gmjfakmto.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gaqiqlvww.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/golgjnaws.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gmljefbnj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gquhtarmh.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gslhnksuh.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/ghtvxqkod.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/guixkcsct.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gnqmfqwly.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gcnccxjxf.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gxhwirxdb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gmigofjjc.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gqyfvldch.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gxblllndg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gveulopka.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gzeixctzp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gljifjofi.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gwymvldwb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gefrxphqa.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gkhzpnamx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/ghydpgica.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gidfonpod.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gecjzgkdc.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gujagtisk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gnuiqxznp.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gpfdchrjt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gphbonuyk.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gjaojorsl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gpvotgfhs.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gfqdgkgft.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gaikfkeeg.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/giasjxvzh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gtppczmwe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/goclcwkxo.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/ggvusmyyv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gcbgkwuqv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/germjsbvd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gjlrhinzz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gdxkjdwtn.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gfluoeuoo.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gmgqysagx.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/glbkiiqip.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gfmeaoudl.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gvtpvjpej.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gkjpuhwny.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/grcxihces.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gbwghyymu.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gfievftkv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gipojehbl.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gkkuxkwyk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gsggcifjw.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gsdonvdht.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/ggfcvuqfm.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/grbydowrj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/godvgipbr.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gckugitzr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/ggiwwxweg.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/ggdejdofk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghdtkfxuw.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gbrqlojxd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gwepgahfb.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gjzlsrhff.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmzoqfjwi.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gftljahpg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gwfiupivv.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gnzsonvuj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gricuvzwj.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gejmeyjnk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjlbwlqe.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gfrlupblo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gkbcbhbmj.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gzpkqrubd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/ghhotbtes.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/ginqsuhob.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gihluiseq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gzpkqjdsq.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gtewsgxvn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gcnxyejpo.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gebewyevz.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gbcdrqrlu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gjrzqmpzp.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghpgafvni.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gjdbgnstr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gkayvgjhu.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gsvqikbom.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gumfbahdq.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gxqgbgugf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/goprogkpe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gowqvudne.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gmdugryja.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gshbhxwmr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gbedgipes.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gukusirun.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/grpuokzta.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gzhddinmj.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gosgbscny.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gqwjvcuwd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gbwodtplb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gxbidepxn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gcufxanrr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gddfoqiuc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gohtmbjdk.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gtsnljgdf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gwmehsojo.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/grirqayly.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/grxrqcjzq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gjsbnjiik.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gdbwmcehn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/ghtgrtjfb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gxyydhxng.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gjpobubdw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gncmfbzmo.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gsihiojhp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gxzxjazir.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gazcwopks.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/grgpoobbj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gdmdfhpyn.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gzhxvqszt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gsgfmgqpb.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gguhcohcq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gewqlnvac.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gneudhbrh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/glnhmexha.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gejitwtav.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/ggexukmcy.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gnknfvqbm.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gzirzpluz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gxxxugldh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gjziberhh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gpgwxojam.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gedzkmycz.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gvqwfjlgp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gillquywr.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gdunncclv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gejxrcwog.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gweheczoo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gakajqqai.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gukfnjdwp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gmomglhnz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gclyonoeg.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gtkxrfklb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghutmhvwo.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gklmxmvic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/glwgeytqv.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gkrewejkh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gmzculoob.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gajsaptga.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gmdidbchk.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gwdkbvbjs.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gbeekeglx.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gatsjdtom.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/grhfopyar.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/glvqscali.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gywotegjm.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gmuezfgkk.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gwmaasskz.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gennnmmxm.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gcdsgskri.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gwlzelrka.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gpywbtqhq.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gufgegmes.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gkpkrtsto.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/glokexpfv.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gkaihgqjr.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gipscctup.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gzykqznbn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gsxxxcces.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gltwypadu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gcyryykip.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/grhdploud.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxvabfdbb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gccawtpuc.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gtbzszubz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gwtwxedyt.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gqvficjsi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gomoseepl.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gopzmtiim.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gjnlhgmyx.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gndqnxzjs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gvwkmhrmx.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gqchlhqxz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gwczcyexy.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gnicxyeuu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwkpkowfw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gjtspyboc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvrqjjvpz.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gdeczrlxy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gheqfgvwv.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gjgdhngro.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfgmuwiix.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/grubbxvnk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gonnpajvd.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gtucfmoih.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gjobbctyx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gxmoqtuve.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/guvyzmghu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/guewqozgk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gmejqegjh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/grplckicv.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gdgdijbxq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/geqnlifgl.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gbnflkzcj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggvclxwvg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gueeqdugm.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gpsslgtmi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/garzsucdt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/greduhcsi.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gueycqmya.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gqgacwhmr.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gjxweeezp.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gmifjyrih.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gvejbpcvn.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gobagegpc.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gqvbjhihh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gfcxzyosm.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gajsvlocc.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gnwvpxnna.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gjsqghmsr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gaxxhwime.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gskauyisn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gawrhmoef.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/guejhlivk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gffucmenp.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/guuzhcqmp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gmbulbbco.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gutkzfqgs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/glzbhgkml.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gorpdsbse.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/ggqtwssfu.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gskkiiehd.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gjllwhflr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gudfkvyjg.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gqjzffhxo.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gorngjimp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gqpgcjmwd.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gplcyqasq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gjtjxhdoc.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/geclksmbb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gypjgyglc.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwnrffuse.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/giwaysxqe.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/guzmiaibr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvfrrdzqw.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gmdxdndwv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/geliggaiz.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gaeklntdo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gdsoyulvn.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/glncowgxo.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/grdryymbf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gvyaklifk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gayfcdkhi.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gecclhcze.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gsbhqrfxw.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gdeyctxxf.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gllpwjvmr.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gnjjjmjnt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gpcfpmrqg.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/ggslrvyiw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/goasfqwor.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gcjgecfdr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gxdjlpupr.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/ghxlwqvcd.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gicpsztnj.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gszjpvcqy.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gyrwxzljc.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/grjjmtcsq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/grdfhoifw.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gzfasiwjd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/ghfprocks.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gedfsnzca.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gaxwalwgs.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/girrpeeoc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gdbxipiej.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gkdpfnwvz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/ggqicymdx.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gajjguxhh.sHtML


<!-- 参考信息 -->