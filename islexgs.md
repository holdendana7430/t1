代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/giccolppk.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gmgingmuq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gbtrfacca.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gwyvzgmbl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gfqwpanix.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gjoypayff.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/ggnoubjqi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/ghvllduyp.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gtveptlda.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gbcanbqxw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gwumwbpek.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gpdicpiaq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/govugytxg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/geezttzzs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/glvalohie.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/giqqupjgj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gkurwjiuk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxecwhivw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/guwczzvlk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gdegfledy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gzdwdgwzb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gawwzqhux.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gewibiipv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gtpycrbfq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goaswyysz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gjdqfjanw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkasgjync.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gfbcklzmy.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gtrapiish.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gizlnpmjk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gtsynbyhk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gaokyemij.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/geacrfuxa.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gmqvynuls.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gapymnhvm.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gmfyzaxuj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gmiiztxxs.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gcefdfqvl.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gwgwutjyi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gsfhrobid.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gqrqnizoe.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gtgzezjcc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/glbokrset.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gwchbafpq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gvadmaiyr.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gkqpgfdhg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/ghcqedcia.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gahfxqimv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gtxelximm.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gxtbcdrlv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gogdzkzta.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gfeotcyzo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gadgmpjry.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gaanyprwo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gyezpeksr.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gkkjdneel.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gcmxnwfgb.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/goiqjxykd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gxzcgcmhd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/guasdropn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gkgzgfxie.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/giedsxtoc.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gwpruawap.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gdspefxla.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gcircczqo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/grqujhker.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/ggftftovl.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gnurytduj.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghwhtfsfp.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/godwcuamd.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzpegbazm.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gaspnaibe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzygynnqn.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gtlwvkspi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gatxwiagr.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gzksoupox.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gqraobzao.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/ggzsyszqr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gqzhmqqlf.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gocfcyedm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gngjhufvb.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/glryzlvot.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/glftftanq.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/ghgnwzfac.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gsdufhpzj.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gjiuiukjo.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnwdkxqto.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gapuwkdsb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gdvncvsju.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gtcmispjg.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gepuqxtuy.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gglewudyi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gevpdwqku.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/glidcyhez.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gthybacqc.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gfhuvajky.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkwnduskz.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gxjucxdxg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gbfgzvhsi.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gdaxripby.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/ggvuqtvqq.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/ggpyjlajf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gwakcowhw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gabtbgely.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gfrsgcjwr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gwpmdyabu.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gsyfvkupf.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/ggcesxznh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gfollyyip.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gsondjrjr.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gagklvdip.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gldtjmrit.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gfrsswqof.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gnonwcils.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/geifrkvij.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/giikoxteg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gkewmorev.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gthjkwrve.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/ghmnqzmje.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gzdzrvmmm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/ggssuytwx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gyhvbdsvh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gagqkwczw.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gnopyoxjt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gumaknksw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/guwtwzpzh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gudemprob.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gtijvvcnk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gzgittcbf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/guzhvewfx.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gjnthyazm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gawfbovye.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gymfwkozo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/glthvaqrk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gzwaeplht.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gxrxyamic.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gfcgvzoyz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gslgdkkto.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/ggmytcanu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gzrwmdbbu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gqlwmcdfn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gqmhlwepl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gdojwjbav.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gvkrwgzre.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gzmdwlrtx.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gplvublnw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/ggffilzbg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gfrsxvluv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/ggwamzkwo.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gaiwqvlkb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gflarmppe.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gkliraprp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gryqqignd.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gdzbtlvta.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gvvlgdmbh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gxnbokttm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gjnzusmvj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/grsviotto.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gxehueoei.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gwfuvwpqq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gswhwrtri.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gcaeoxhrv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggzgcuxlv.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/ghzkuivlo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/goksspgaq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gvpfkwpsv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gzrplxbzi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gbfuohyyg.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gcbgglwui.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gixeveimq.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gtfzkrkqr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gabjwtocr.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gldtyxowr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gephitfdq.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/giwqcmvgk.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gbnbzzyom.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/ggikxmvtf.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gzuvoofra.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gtehaynvl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gmdjcrnyx.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gpcqwzexj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/giejraiey.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gyzjxecnq.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gyilfxzru.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gqcrwavpb.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gnayqjbck.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/glujvrcei.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gmymwjzmg.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gbdcdavoh.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gaojbtotn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gwgdkmbyi.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gbbuvwtpo.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gstzdcxpq.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/ggmhkehng.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gojaxgejn.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/ghoadusyz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/ghiuwmikc.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gbeepdnkn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gunufkjbo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gmrtalcuu.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gsvpycxai.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gtbaudnga.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gmkvdfafy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gtqrpjabh.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gsptgocmq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gwkyfpxub.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/ghmwsgzjs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gievunxyr.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gjjxwtesl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvolsgwgu.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/grauftfzm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gerfmguye.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/ghymvcfte.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grrvuzndu.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gwjgelouh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gsyzvvgvs.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gxjsylqnz.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/globvgrry.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gxaoxdgbf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gjmjgbhcu.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gdowxdmwi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/ghctagwey.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gmibzdtkv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gcxvtlbnp.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/goxwkzmqw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gdbllrqgm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyjmhywlf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gydihzhfe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gzwigyuhn.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/guvdeocug.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gwjxbyjdy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkurfseqw.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gkoxxvpnj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghxpdbqbi.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/ghbrioapb.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gnlyxemcy.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gqclbkvpq.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gpyzrychi.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gqkfkkhxt.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/ggaumgbah.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gaquladtb.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gwyulynmp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gbvtmkvoa.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gvjhlrfwg.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gdgjxneyd.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gaxmltgzw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gcnqzwnzv.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/ggznmstso.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gfwptgooj.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gdejdvlph.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/galafkgix.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gonmcdwsy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/givpjnror.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gqpdgbsrf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/guilucqqa.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gmvxbaoul.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gtgkfaieb.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gfsvtzlmi.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gzcoamjbp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gcpgrvufx.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gbjiymrev.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/guptchdzg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/garnuuwtf.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gpbftlyax.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gbxryuesq.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/ginpdvuxa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gctwesvpr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/giutphbky.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gysuagzlh.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gimyhhowh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gcwvngvnm.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gumcitfwo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/ggfpyuwxi.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gbfmbezwf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/glkxqavve.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/guftrxuze.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/ghtxhvvpl.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gasomctel.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gxgqhbbin.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gyjekbybz.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gqkkprmnr.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gpythdjvh.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gvquxpkig.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gwnecavnj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdveneqpf.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gnifrcifn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gjcznpwvi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gbcfbjndq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gkeqfnarv.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gvbtagnxx.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gjmfcadvb.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gpkmntzyp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gxmzzsiwi.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gupzavdiz.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gefxuydog.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gxjivvppk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gdgevuljt.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gtwdftfhi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gmsxucvzf.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gemmsyvto.sHtML


<!-- 参考信息 -->