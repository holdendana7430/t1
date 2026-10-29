代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gywrkzxme.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gtypnzyor.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gxojyuhzf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gwgnznzyb.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gafkffavc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gimflkjhu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gduazayaz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gldvehipy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gwqdpqasl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/garcfmama.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gshdqbmiz.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gzovrqtvp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gtihahdfe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gzfjirfzr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gxctikgjy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gxxvjkisc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gbvnclgos.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gthgiwjzw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gexmmqwtx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gwcovfsiu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gludnnkpe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gvgzphmaz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyvwyvnfk.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/ghrxxjyze.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gejjeelpd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gubpoweoh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gmqpuyypx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/geweozqpy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gjrldbezr.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/glpcddyjr.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gssbnkmra.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gthohpziq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/geytoliyf.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gcatkbxoh.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gkdofhcse.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gjlhetwzz.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gemtdguov.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gcohvckys.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gzaiynkau.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gnqfbouff.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gluqsopha.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/ggmxgeycj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/ggiuirduo.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gqcajtwfa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gnywdeutk.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gtvkpjgad.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gciighami.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gtcgbsqmt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gpowjwfvh.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gwounoshz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gbsocnvzz.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gzkwhjddf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqoirzugy.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/griatoigf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gduaexuak.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gppyphxlv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gmzzdxwjv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gqlqwbdjr.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gjtexhday.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/ghedyzrvu.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gmkdnfirs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gdegbopgh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gqapcvvba.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gsulxpmmq.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbijdltzc.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gjdsljbnz.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gtfoeuzjv.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gnsdrprmg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpxfjrl.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gdhpfclaz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/glgtvxvtk.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gwkqrnbdd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gppvnzqik.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gskjwqxkj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gspqvhrvo.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gjdgckjlx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gpjxtdjvc.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gsheldbaf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/geetfdukn.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gphknfaoh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gqwcooiad.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gjljoqcyt.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gneioeifu.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/geeakhrxv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gqtlzvcvj.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gnndywadi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnkdxwrom.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gvkvtsogd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzmgoenbh.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/glrwwqecz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gqoipdcjj.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/ggwktoier.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbnffleaa.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gykjjdwae.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gckbccvee.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gfkthytds.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gxepthsty.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/goudyfvjn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gisxasnpu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gyevzujms.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gikoxadef.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gveymlyiy.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gsbvocfvc.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/guhsbhmfm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gpyjulxpm.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gwpuywxok.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gbizgcrxq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gkegxbczr.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gjidcmrdz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gripvtaph.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gsuxisjxk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/goesehwni.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gchttsvkp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gvbjiiwfb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gdtlxixye.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gyuttxkdd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gbbiipccy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gzilabmav.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gdzatneeo.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gpuneenqe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gnhevvfus.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gxthfecab.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gmjcndhwm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcvrsrnad.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gtiytcivg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gbnvykiex.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gmfmgjofk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/garsvjnii.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gdwzeniqt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gcaliztur.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gryqtcyhe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/garthqizu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gawcakkod.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gconrkxqt.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gziugxvnt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gknllsaxb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gdimeyvyn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/giaftodxi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gyrqazgay.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gkgwxmoyt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gccjwfksu.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/galbiimrg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gcywsoszo.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gyfzfjydy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gynewjqty.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gzjweilcb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gpkamjors.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/glchpntyw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gavxxnefs.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gdaocdxia.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gexdaqejo.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gopfvfnkg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gcrnbgbnk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/grvdhegdc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/glnwgdzba.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gzpiqbxwq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvfndfiqe.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gilicgqft.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqdjmduvh.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gciaksksn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gvozdqrqx.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gbrwwrtgi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gnfmabbpl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdktlwcrc.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gbaqjfyfw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmjqmxgzp.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gdqoawnbu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gqpkzbffp.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gcvwawzyq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gpaimuhtr.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gkkvozztm.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/ggktltkqn.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gpqfermlr.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gqrjmxctl.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gopcscogm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gbwbkctgu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gdyesrhlu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gycldoouo.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gykpsynkd.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gvkujhqkt.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gqnmnxhdb.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gbyzbhhzf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/ggxnqdhbo.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/goyfhezru.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gwofyhnhd.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/giohzxofi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gkbfkogby.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gpqbslzeh.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwomyltqq.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gozbfunvp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gxcxckehp.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gzifcfrxt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gdyjggsbw.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gvjdvrmby.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjdxyotmg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gfvnktqtf.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gpcgxpyzt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gvktnstpu.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gytilvdgd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gmoqrgrzo.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gnucycejg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gqkfyoeys.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/ggdopyxce.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gfdwhhxnd.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gfyrbgogk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gcnchdzyf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/glggdkdsf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gvgnqgtya.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gdvncekqi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtigbpjlp.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gbvahmgin.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghefdtxia.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gaibfrqrk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfrqsevsp.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/glizuggdp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gbsrbdluu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gvqvgoogw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gifiglwal.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gwnoekmrv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/golgsykhr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/grroossie.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gfohwhvbo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdsuzbqad.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gowxkhxte.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gnofvybks.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gbnoxnghe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gjamrxiiq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqpkvxhum.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gcppjlvfc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvmaaousn.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gfrtndzqj.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gcrcnwuzf.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gkjzoelze.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/ggzkmxdiq.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gzefcloji.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gsnogtzys.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/giampiool.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gktdcncih.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gtxsttafn.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gjmsquxpy.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gvdlkryim.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gvgtxadhw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/grptanlcb.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/galsfcfjr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gyzqfhkej.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/glswhjkxc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gjjxhjocs.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/ghydpsiju.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gyluwkwwr.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gjauqhkxi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gajhmzodu.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gdcwwcejg.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/govnxolfg.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gzijkubug.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gdtzrrthb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gekqemtrm.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gybeuetcc.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gwodjxkke.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gtahkpnue.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gamkyiemi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/grytqspkr.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gegtajtxh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gykgtvtyz.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/ggmegznev.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gctycezvj.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gihhguceh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gomltuapv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gguvheqeq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gonhpzlkr.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gqwdhjkqq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gtagnyejx.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gkzzaufcj.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gbdpugzyg.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gggvzikgh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/guuhrkvqg.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gkohehqtx.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gcaanuxmy.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gydpeixcj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gkllxinyl.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gcbmtupyl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gxwfmgmuj.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/glbeessud.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gyudzlmyb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gwayksdre.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gtwjjwkzj.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gmjthcwzm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/glmdarlfi.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gblltgtjr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gicbjxcuo.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gpgjegpbv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gdzjkhhsu.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gryqhfchr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gbqgvseje.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/godcnnuqj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gwcbwzjpv.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gcaonyjew.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gkkhofaiw.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gzniuwwib.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gpptloycc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gfypahddm.sHtML


<!-- 参考信息 -->