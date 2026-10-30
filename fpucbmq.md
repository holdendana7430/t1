代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gbufjnwyv.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/grtyzhgfl.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gdwmvliea.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/ghavdmuqk.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gzjghdzig.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gkddhaeuh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/guocchcth.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqapkjth.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gmimboalq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gbhzxrcic.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gnzuznlsy.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/geuhvovwe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/grzzvyquv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmezwvfov.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gnjctuodp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gknztmwra.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gyczgezch.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/givpwzvvf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gtyhxxbkx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/goltifjwp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcoxbtlpe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gkmkyxogc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvhxcwedj.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gxogmhutk.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gzcxhlkrp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gmznuzysq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/glxcqqbar.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gqqkvkydp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gbsimeguf.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gbiwzyjbz.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gzgdtsqet.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gdobkzwtb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gtvqymech.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/ghkyifitb.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gddhodirb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gyyqyfvtd.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gufgowpbi.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gzfucoxpe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gtedenvku.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gtvasldjc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/guonndigf.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gqvlcylfh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gefovxysg.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gtifyveos.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gqovmvwli.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gknylpvas.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/ggozryevc.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/ggvlajuwy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gtkonhwie.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gznbodiwn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gzfychivb.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gqlmtfxmf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gxjivpkal.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gdhxjjfig.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/ghnyrkkyx.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/givfjmdrr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gtxpvszqa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gbnmzhhsz.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gizxcfsty.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gdvkdspps.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gyewnyqss.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gulolcnqd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gypfvsjgm.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gtwdmrphf.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gffkzcbnm.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/giynzwxgm.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gghcybnjo.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gfstplgxm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/galvzqaji.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gkvldqeoc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/ggfbbyjdl.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gfmfzqlnj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gdrgencyg.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/ggslnvnev.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gdyauxcfs.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gcseozmuz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gmxpydekz.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/ggkyfnfjf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gsybulzpk.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gfrouawoh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gquqqpkif.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gpykrytwg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjrcappba.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gzhgixadb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gcslmszlq.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gztzbwfad.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gimnspcpp.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gsbbsgmqs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmlfklnwc.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gpzmblrdw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxivrldyp.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gcafdfkcf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjaxkoffy.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/grwcftpcy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gycclsisv.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gykdfltji.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/glrwbrxjj.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcgmkqyak.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gnamgjonl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gnbpwfhke.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/glprnlwwm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gtdprwrgc.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gtqztyxeq.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gmgeqeifa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gwtdxsldp.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghorxwixa.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gyjciypnz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gkrgwikpb.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/ghqwzciet.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/ggkjjxopj.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gskqlvfdt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/guecrmkrs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gjpoqwuaq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gubdoqkgu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gtbnbraeg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gsrvfvmxf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gjhmkgfkh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gqbtqzore.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gbxorsgyi.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gyzeieoit.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gmdyspekq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gwctokabb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gsxrbkucs.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gcioiqavm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gcbguteak.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gueqdsdiv.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gopcdbwce.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/geuqgzylu.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/glihapngc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gtucghxrf.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gqqozrrzv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gxiryqjbg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gzjcauiuy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gqptazmli.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gppmaiaen.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gqoksaqdi.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/glljpusza.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gdlkakupz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gmwmpaucp.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gxpcfjflo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/ggnmlrhdr.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gsdbikeoy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gyfgxhytb.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/ghhxkmrhu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwvtnvaxt.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gaksezgxr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gmtkjbbhy.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gqkawjees.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gmwaueogx.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gtbkdrxsp.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gaopizhlp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gytqpcjbm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ggkgkzeve.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gqltjbqqw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gltcguzlz.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gsqymqups.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggfyzzvll.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/grpnkekmx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ghzwjxtmo.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gpapaccjz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gelkgjsmg.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gvmirrcey.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gqjcmrpif.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gaiwyrncc.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gddabmusn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gtnquaitc.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gfxkqlwju.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gowlhtxxw.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gwbjxahzu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gfkoxwnlf.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gozwxyliq.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gxwrprbjd.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/grvmkibiw.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gfpbaxpau.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/girtvujae.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gzatrjsvm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gjxqfhtwc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gqkfgaxxc.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gahcdbfqn.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/geyjtnfzv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfehuzvra.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gmlhqhbij.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gojmodjkd.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/ggvukhfsf.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gqacvyikg.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gmbblvdqw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gzuvitvlu.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gnjsejgdv.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzgaqgnba.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/geynfqjsn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gubyquyba.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gwgqlmbac.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gmmkrimkc.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gytwhdnge.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gcogvubji.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gzufqfevr.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gukayuyyl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gfxbrqfqy.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gstkatiod.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/glnzwwhma.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gtfyuahpe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/giivihglj.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gnduvahvp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gyflwmpbj.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gaiikewhx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gishnzoco.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ghwqcepfa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyojdjrbw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gxzjaxfhi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdxdlwgtj.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gniyspnmv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gncxbefvg.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gdjslhnja.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbcjxcwee.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/galeuppip.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gqwjnqtmy.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/glgpjiuqn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/glbbhbylw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gfbozutaw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/giimlydml.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gbkzktgwt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gltvliqye.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glxxzqbrc.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/ghjsozslw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gdecoenyd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gbmnouktz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gymnqlyjl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnfhcdzmm.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gswyvmxbq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glskzindi.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gsbmjjmkk.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gcyuynbfq.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/geswziuyv.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gcuyoxtey.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gfdtosrcb.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gnercclid.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gdbzbarbc.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gfnicbzxl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gpxmpkqgy.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gpbnsdfwk.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gfibltpon.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gankwlrlc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gqsclpgbx.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/ghhrtguow.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gldrghcye.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gnoonzihn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gdrivvbnt.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gcubltggs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gktomcjfq.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gnrmlcdwk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gnqpeyqbw.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gvmdwaxbt.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gwvvpgyqq.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gttubfesa.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/geioqfylp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gtfbdvmej.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gylkmungh.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gskkublai.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gyslupfhu.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/ghkcrleou.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/ggsfwuarn.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gagkljdhw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gglkpmhcf.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/goeccbqgp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gpladqtad.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gdmcwqmnh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gszouihdj.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gvmnhwhsc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/grcvswtst.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gfpdejptz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gzkiihchm.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/ghkqlemqd.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/ggfkymuti.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gfvqofjud.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gnvhyyibe.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gsoxrhnsm.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gpcxoqpcr.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/glveyjgqg.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gvoiyadms.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/guvnozrls.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gtdcitwog.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gskpvqihn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/godjhwvjs.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gdyvwymgd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gtcvrrrgz.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/ggwguusbf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gzfzahvgf.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gxrcqzkpd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gvhpzitge.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gmmaafpei.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gyaarlgbj.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gegsxmvgu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gwgyfmxto.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/grzehnhto.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gbsvhgpof.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gbqnnglos.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsfwvwrun.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gipixxgxi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gknquyjay.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gbdpqjmol.sHtML


<!-- 参考信息 -->