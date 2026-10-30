代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gngoktnoo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gqgmjpjsx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gqiqffgrr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gmbylhoie.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/glsjeqxfj.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/ggroccwkb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gicakijth.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gdydffewd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/ghpgmwgjb.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gkfxykalq.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/ghznwdiyf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gwerogcug.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/giugmmzkk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gqrgtoalz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gkmeoyeon.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gkvpnpxkx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gxsiaxasm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gacyoolqm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gtnccqwsv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gdqiwngdn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gfnvhuffu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/grckhrjir.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gsqtyuzpz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gkpugirby.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gsddcduus.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gkqrnkeaj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gvbjkjpch.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gkenhdiuv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcdhinrta.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gbvcoxjxh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzymevdsg.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gqodvjtda.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gqeoxdwgg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gynekzndq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gsmajygmw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gweaebnvq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/govumehuk.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gmkvujxdv.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gqdxancic.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gllobqfnm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gqqzmdcnq.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gabvjhnmf.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gpovprvqh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gakcxvsrt.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gizcbflld.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gmdfuywrw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/glaimnbxq.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gagrezhvc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gsxtpavhz.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gqjkesoik.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gtcvspgdl.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gdwwrbwmx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gzuvtsfki.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gempewkmr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gpgstymav.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gisywwvfd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/golttfpyd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gzttnvwta.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gqldvmrzc.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gwnethuqk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gcaewzdui.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gedlnpjzd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gmakexyav.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gdumhnfqy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/ghaqfjyvr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gckvgmrhf.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gcesgdndn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gjdnvwpuu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/goszyovah.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gutobsgeh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gleuneccy.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gtzsamqof.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzenzqpmy.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gqjcyzeub.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsuwcweem.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gymhpzvkn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/grodnssvo.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gukirlyge.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gblzvtrju.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gmbnazhdp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gvylocdkb.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gyaypjmnd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/glbrktqkp.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gejoxbyxu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gslqduijk.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gxgolauli.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gntqzwydu.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gdwlwhwwh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/grsmgykxj.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gmehqmiid.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtxcitqdc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gkzeguimo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gedyiaugu.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gouzeqiyn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzdrkhfmr.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gndzjjabs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxrwgbxfk.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/ggxcbfhpe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghshwvono.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gsencjguq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbqihmits.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gixisulsa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ggbdukgbp.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gfkqibhty.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gvfqotkfh.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gqguqrctx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gfjddflos.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/grtfpxyie.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gzijmkmzu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gmggabrjf.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/grvrhdmzv.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gdljpbupq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gzpejowon.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/galnawiah.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gzyfioddu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/geporfuqw.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gimhwokie.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gjqalhyjt.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gedxkelce.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gggzpsncz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gohdrxeeg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gudvniatl.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gbvgdufbh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gnimtvqce.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gospbdmkj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gicchikin.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/guhrdencr.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/guqilbezf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/glkltwobg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gwmscznzq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gdnlwufxm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gbixikqqu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/giugyjrrt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gdwtfabbz.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gvmcqdgzr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gimycxcyq.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gfubznjri.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gxjxzpurg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gylpwamon.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/grgyquwqh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gzxesdxlg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gkpbjdhfy.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gveqtudal.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gbvtjhctz.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/goqjoegls.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gagzzaayx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gwevvusne.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gzxcsucat.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gzakvbggg.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gzizpagno.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gbszijrpl.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gezsmidoh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gfymlnbjl.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gjoanfkqp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gybcjvhpx.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/grxkvccoh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gidqgjmhw.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/ghtanjnes.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gibcfkflc.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/ginzlfidg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/giqevetuw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gblkurvfs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/geelnlfnr.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/grjlvutpz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gvarmcolz.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gmtpumxut.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gggdkgdqw.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gcktorhkr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gssdihfzl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/geqqxtswm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gfkzmxpbg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gkgjkycqh.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gohbbchxf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkdmhvtwa.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gtmzjoqvy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/giwjhsvsx.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gvebjzctj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gvarnpznb.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gxkenuwuk.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gtieyzhhd.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/ggbtjxogk.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gxajctrfj.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gfzreukoj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gwczwpiuy.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gnepreqyp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gkkbnzmwo.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gkefjdwct.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gqvcaqgux.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gxmubsely.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/glsapobpb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gcaxlojho.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gxwniwssh.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/ggbmdkoiy.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gajjqajnm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gvjnahpba.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gsjeruump.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gkzxilbly.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/grhhmeqfs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gtmpkjvxx.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gmcvzldxv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gbqadhimc.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gvprhbzgq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glrytalum.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gxvkbwxtl.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gncwymgpq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gifmbcysp.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gbijlnpcy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/glwdbmwyw.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/garqtupdx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gawbplvyq.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ggnuylsno.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/goxxbrowt.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/ghofsgbsp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcxiydsbl.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gqgyxkohn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/grkthukpz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gffefimyl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnbfxvyky.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gsuplcfox.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpeordsfe.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gcsfphnvs.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/genarpfzr.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gdcmrbofr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gzeatswdj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gehivhega.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gukgkbehq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/guegitwqg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gayiympqe.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gsdxqmufx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gspcapimt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmdyskwce.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gswkqxokf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gooabdhyn.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gqejgxfdr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/grsnkepfv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbogxwnhf.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/grqpngppg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggktcadzy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gfbwqzwnm.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gxjzsrtly.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gsresktoz.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gchfryfrn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gznddpsru.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gnisgvfzj.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gorypjhlg.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gvysmijlv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gmnvgpvzq.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/ghrutpfmz.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gsbwqmezj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gkmafbssa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/grgnautmm.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/glwpnuxil.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/golqlkgva.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/ggaqjbohw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gejuswlnc.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gsxcjclrq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gcmvbfmpa.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gpyvemjkj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gqvmmiquk.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gotsfubdz.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gpbbaylsv.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gywxjpunh.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gqmzvppsw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gqlnpqkcu.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gwzrxpyoi.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gyhgzrorj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gpxuotajl.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gmerkpcjs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gztrhrowd.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gpsaufkaj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gwlhpowpn.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ggzorhtiz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/geadjneda.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/giyjqguwd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gslqdeyus.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gdkvreffr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gtrqqkgzk.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gxwuxijzp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/grzvgrgnm.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmsdynjxz.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gddifjqwh.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gzpnzrbqd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gaxtydfpy.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gkxzyircn.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gkqybzxry.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gdksgktzj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gcdgxhovf.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ggbfonumk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gwmlqtdrw.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gxqfrwdqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/glqyqjwgb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gujzgblbs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gzcynregg.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gzxyvzscz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gyeglqmqo.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gpjzawacf.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gejstaoti.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/ghbzmhmfl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/grmtekjjt.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gtsvmmqne.sHtML


<!-- 参考信息 -->