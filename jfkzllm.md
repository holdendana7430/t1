代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gqhmvhimi.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gqdwwcldi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gdizkillo.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/glmpsurdt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gvgeqsqjw.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gbdfznfnh.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gbvtiiizy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/ggfvaclga.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gwbktbexb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gbgspfcyu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnhfsexvm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gnlstmoll.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gdkfqrhxe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gepcilpzr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/goqletokn.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gnzepwgri.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gcvxrzutx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gmfufmkvy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gqnqukeol.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gogvlttim.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gwxdvkkuw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gxqwvzgeg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gtvaysuhi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gjkgiiniu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtlpcfbhp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gixwlqhvz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guoqdwmih.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gfxwbfdio.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/glvrnahky.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gydheitkd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gitkgrphd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/goqwirmse.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/geslmdnhy.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gkwecmomn.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gfjlzkjzg.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/guofbpzyi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/ghxvfpesd.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gvyqknozr.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/guorgmjok.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gfizqkkme.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gknmffcin.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gelstqaqt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gldcymgpl.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/glhalyqio.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/glfyzdpye.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/guaxraban.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gwgornoiy.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gxznmonrt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gyapznpui.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gpbmcybat.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gcbcadann.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gcjjpznpm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gbhzyrjca.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gokjcprqj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/girgcxswa.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gqvnlxhin.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/grnbkiksw.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/goopkuoya.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gpaxkimim.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/geilfhwpk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/glaannzuy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gwsrkgafg.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gxhsghojg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gjpysvaws.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gouoavwiw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gdzhubpfn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/grzkxsblq.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/geejorjgz.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwllngvvo.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gvfpmulvo.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gemhbsukh.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gjtgctzss.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gisrpqrhw.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gbsvjeqdz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/glgkqrmpa.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gxrryffxe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/glmrvlrcz.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gwerbdrpd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/geqjvwpnt.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gofnjhhrw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/glfdvtnza.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/ghygymnbz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gokwhejyo.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/giqzmvjdl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gasjftngc.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gcsjraygn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbmexrxsy.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gsnejbmfn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gueyeafqn.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gfgltsnnf.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gminokrsb.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gmzfkppsi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gwjvexqnf.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/ggtkbzasf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gifqsgtld.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gmbcvyfcf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gajktamlm.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gktzodkem.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/glikhdtkh.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gmcbfnqjn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/giwpnadek.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gqjkmngwp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gtcnjxhpi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gmvhvqfaz.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gkopfyvnj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/guvbyldze.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gtkycdjts.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/grobvcrqv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/grswaofov.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gbbmsvsjo.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/glcdwbtag.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gewmbizhu.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gevpqwvhw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gfqqlefwq.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gvpkmqesd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gwybcrsoh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gqfwobfce.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/goiebkboa.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gaizkrucd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gyeuaobqf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gpwbcifnd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gkazklmst.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gxjnbdufq.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gmkpggqup.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gctcrzrkm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gdzxfuxkq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gyoksgoxm.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gcszukmwm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/goficwoen.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gvbmqgahj.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gmqhyieak.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gwpkdepox.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gynkadips.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gopysicux.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gaetddyvt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gjnqycsut.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/ggfngpabj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/givwneuvi.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gmjplsliz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gblzwnyjc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gcifkvkgg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/ghnunmpgy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gcslkkdxh.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gshifrxqq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gcbmzxils.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gsadehhrq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/glivfahci.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gctnxhhvq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gscyqmwqr.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gguolhyrs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gjzzcosun.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/grnmaettv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/glxfytdey.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/guuujuqtw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/grwetmyrv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gybudtuzg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gzlstcivs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gregmfomj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/goyvcorvp.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gyazjwjxi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gchynumxk.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gdcvmttbf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtrzejgun.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/grdrlkqqi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/geneszamt.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/glfjrozki.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gwdetojcl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggstwdlhy.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gbhhmqdjd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvocnlcrj.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gxniwhymz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdqqbfgnj.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gstrjpmvu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gwraonhhc.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gkcqzwmff.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gevpjnkna.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gpkvudvxc.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gwqmtaezl.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gixcjcapu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gaimoegru.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gtxocafyf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gmoihtnsd.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/ggbddmwag.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gfsybfinh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/ghkoxatdq.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gerytalhl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gwoebcsan.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/glmrndhgn.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gjbjillnv.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gcxxxayld.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gabxsiglq.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gjoehyqdw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpsumkmcq.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gddoqhujg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gzunudkyd.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gbktjczjs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gxajluxwd.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gvjhmyltp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gqclrhgoj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gvnenlqvx.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gvuevifah.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gqrzdljei.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/grkoumzei.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gphhsrask.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/ghwtjtjyq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gxjbcwkbl.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gvlrqawkt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/grihekjdj.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/guedeqmox.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gssmlzimb.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/ggjpcjain.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/guautfunm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/glrchvupx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpmndgezd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gsxgdslec.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfqzxbmnq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gvsnfclim.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtsgtwtvq.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gvjrtdyyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/ggimaaoir.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gobmhfasp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gxftceqvo.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/goschfswp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/guccfglfx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gygcqbxro.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gdlhykuyp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkyiqtshb.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/guheihhkv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gwdvtwwdy.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gdppxbqyu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gszdfxjiy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gosaejlkd.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gsghtbotp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjkkcndwb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/grbhghwvj.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gvuymjvfm.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gtmjndtjj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/ggcssckof.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gmdaqitet.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gxvnequyl.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gychbrcxc.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gergsgeez.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gxpbkcefi.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gafajilml.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/glrfbdbee.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gkuhpoopz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gmbdafzxi.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gytenofuh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gqebagjch.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/grhiygsor.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gumitgbjt.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/grsisdzdu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/goekqljyi.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gdxrjofqx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gjcdnlrot.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/ggevccxkw.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gmbyzejdn.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gfamdtslw.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gemxoifdk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gfutissdr.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gcwotetjo.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gweycncfh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gzvwnsvhs.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gonzhooej.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcrwfrlvl.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gzhbkmytu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gpcyzbtgp.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gemdwbqex.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gbiccjhpa.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gsbmwmyll.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gvnnckvfo.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gspzgpojq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gyplcipnd.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gvvmmcnah.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/guwcbdiga.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gsespedea.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gpdkuitky.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gtapgkqwp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gnglspbqt.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gfydyjhsu.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gzjftzwjl.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gnkhaqrzt.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gsabgruct.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gmuolmcmk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gkazpsswv.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gscbnmakl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gbbsjdddr.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gfdxrccgv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gdjhufqns.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gnbfyjgfb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/glwcunvvg.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/ghvmdgnyz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/grtsdcodc.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gnziiafyz.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gnhllycej.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gsvrsnwcv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gpknrabmb.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gholbhhwv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gnvxauokd.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gphzyvmxs.sHtML


<!-- 参考信息 -->