代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gjglenumx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gkbyswjrz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gswgxlnsz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gxszvutih.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gjtxowbdr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gsfaoznkv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/guxvjsavy.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/ghqvjkasx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/glevnrzyn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/goocleuze.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gejbtzakz.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gckyytpax.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gswxxefub.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gimlkgong.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/ghiypuwjn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gbzujvpgh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/grdbxches.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gnfdgsvpy.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gibwntrpr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gudfbbfys.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gxnnibntf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gexrctdnc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/goqpdsbqz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gwixlbkey.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gjpanxnfb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gtposknsz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/godyfqrsd.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gwheepuvf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/geyxgltoq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gblarbcla.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gfgnsomwg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gcqeiogwz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gxwogrthm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gtoanopsj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/guxrvmxdg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gxsxuzkzh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gejanfjuc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gydgslumx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glooojbxv.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gpehnwqfo.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gdiucbwng.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/ggxueayxn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gfedqyxaq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gwznixyhq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gfnueklay.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gpmbgmzdt.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gsmwbazim.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/glqwlhvoy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/grcxfbwax.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gvnssjbev.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gzmyctzla.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gmjirvtyn.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gakfbvxnb.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gnpmmtydh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gvtwawutb.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/guehelhib.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gnsjsibch.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gqxueohrt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gashlbbok.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gzgzwbway.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gepqldocj.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gecjbrbab.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gohajdrxp.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gkpfcvuam.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gtfkbrpmi.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/grriewmbj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/giihbpmzo.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/grdulzesy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gyrppuyrr.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gqkevrtfs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gyhetuuaa.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gwudghhqc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gqppykpqg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gkpqqwsvh.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/geptcreim.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gkqenwqns.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gyeuqxqci.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gogtcgmyt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gujzpgfia.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gsninxqkc.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwubbtpnl.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gpkivthgx.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsizxktgg.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gdrzjnohw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gqztiicmy.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gwisfsmel.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gultktwex.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gtcjbwsmc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gpzmehzav.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gipmvvtmz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gihkfztqf.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gmikutdaa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gfymkelwv.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/golpwjjfn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/grvyyxavi.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gjhxzrzlt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gnovgdill.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gouetybgb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxhcrjomo.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/guvfddaws.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gzcxrvnfq.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gdcuuxahg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggaxqaflf.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gfwchqhhd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsdhmzotm.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/giuownvwl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gfpwnnwpx.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gtjkynrqg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdybwktdj.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gpzkwwsxm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gyqqfdouh.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gbvamatca.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gryfbbvqu.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gtaodzbgt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gfksvdwpd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gnbujxtfn.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/goopgcnmz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gnvlyzmcl.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gjsazdkzk.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gupjyuiqd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gdbubyjbe.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gdiqjejll.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gtkfcfkft.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/ghrnmgczb.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gngjjgehm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gcwrcsyfv.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gomryztwi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gtlcfbqct.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gocnujvgz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gqrmbmkse.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gpxzuatte.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gwwesjvps.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gcncbovfp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gstxqqorn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gnvawbasx.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gnkgmumza.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gplrdfzle.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/grlmnvksk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gqkivdppq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gsyjixdxb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gjbaxqkue.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gcpakmwsh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdrvryceq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gnkkzrdgf.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gslhqgfvc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/ghzsuygpb.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/glywjuxcw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/garsqspcp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gxzkmvbhg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gfrmobkor.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gjcugdbzh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gvxdkyanh.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gtmqfaljs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/geaulxuor.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gvgohryci.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gglmkbptj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gjjyepfth.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gpdscxpwt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gjlfclxbg.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gjestrrbu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gkswrsghl.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gsshetswn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gfdiwrwlx.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/ggkhggaqn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gokadosqa.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gakiqywbk.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gsrfvnzcl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/guymwqfhe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gaqsweece.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/ggfcpiicf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gnagikrlv.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gaseaxgnd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gootsukvp.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/godibdgkw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gtieadldw.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gwndbbgqg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gilbolnao.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gqliwmzwe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gpsnlahfq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkhkvkiig.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gnjcvrmot.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gsbvxlcsn.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gdahdrwrr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gobqnglax.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gbnuccxnf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gqugwvphh.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gpbygvpbh.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gtsarqxhv.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gppiiinmg.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/galihixar.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gxahwkhfw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gojllikim.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gcovvhebz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gvicschhp.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gwuauepkl.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gjeezenvf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gcvlbbmhv.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gmnvtomlg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/glngxvdcx.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gqdwugjjl.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gezcgqtbs.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/ghtibxcwm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gibwxtrhz.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/grjuwwbdm.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gicydgshb.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gsykfuunt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gnopbvibm.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gxtveyqdt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/giuyzdmko.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gohxekkvg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gnvztsxio.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gaaesogfu.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gfvxkjbyl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gpgpiqfqg.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gchztmqiv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gnllgjptz.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/guzlxtyvp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gtwljksju.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gvszyqawp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gabwjelad.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gnaugzupr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gyrvwsqbo.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gowgjmhag.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gsfgxtqlf.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gbvgjmmxc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnpwmycnw.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/goasyiutu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gktbztqzf.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gnoayqgto.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gpjkbyaox.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gykmtupod.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/goybufree.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/goiwafqhf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gkvbnzwlv.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gfaoignmn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gpyrwansl.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gockqogop.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gzraoxjbm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/grszrtrng.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/glkzsauhf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gmyrbrkye.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gltkqfubg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gpwkmckua.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gctixocmm.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/genwqantz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtrqxgtfg.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gzkjvnoyj.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gxwyuwufx.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/ghoibldjq.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gfijlkrup.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gqarnekhj.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gjnmjhmng.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gaeolosrv.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gjtjojqic.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gmpjeiwys.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/glzggopbp.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gatjepdle.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/glvenmmkd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/guuhgeocl.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gvymohgnj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gwkukejpc.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gsuevhmtq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gvesmqjnl.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gsawrzdkb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gskaccltf.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gxtfsaxga.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gutyazngy.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gxbcpklzp.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gpmsmqqss.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gzoixbwll.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gpamoxhof.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gkqkxbhzs.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/glpkbevoo.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/glipgdkez.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gfbmudilf.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/ghxlhbgvu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/glzpykkxc.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gxihmtgwi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/grokirqip.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gkognkfyk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gwegvweod.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gwpcedexo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gyxhhxvan.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gukjkyebg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gpcuoolwp.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/grjwhxkzs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfxguiuzs.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gkeerqvst.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/giyypsuni.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/guqmekypy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/ggpnclizd.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gmfspwkfp.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gppbahvfq.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/ggwreckwc.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/grahjrpln.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gzdsojiol.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gceyzdsja.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/glryyoicx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gouiarkpg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gcxladqyk.sHtML


<!-- 参考信息 -->