代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2etfdnbwc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mtajzjao.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2sylfhspa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jggfeuoj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iqignath.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2iijuwxsx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vlybmzbj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nfxjchzq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hekgxfcr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dppctgor.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2oitinvlo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znvbhvin.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wrruiwik.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pkeldjat.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bydftdhu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrzachdh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ntemfmgl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zdphntsi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2wccbyywf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hfpcpadu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2bekipbhg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tikfvrep.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cpypmnqw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdhsgneh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2yotdnnpl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zvuujmlp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wndbmgfv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2byvmghxb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2dxrrpcpq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xchftbaq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gjebnztt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ssmgfwuu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2yhzcyzeh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ugssjfmp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2tfolhsdj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jzwmeokh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzfmungh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2nzahtqqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xskoysky.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2iiekcjqo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2itorbglb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lmugxjft.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fhjcdbxy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2wqvsgalc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2eqpymudh.html

);
来源：http://www.52xcode.cn/Article/details/gt2blqorxua.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2thblzcab.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bxfpetcw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mlfqnfqq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bfujnleb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zygegpcr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ljrdrfru.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kuzhybsz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2rvjnurdw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bsbnxziy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vhsixjyg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ggnifyht.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2aqptwqzq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2osvizacw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mejeeaqe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2urclztth.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2utewejxa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jlxcwrmi.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pxbodcnl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xryywrvd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2dqaaufxb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ifmtiyou.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2lypsqizm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lqdadxil.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xflsotae.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bponozvz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2yvjociop.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2avkkvowd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hmjpnhhf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qoqhesjn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sxmkqgou.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2olxrzfat.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hgtllozq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ivyhlvhe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ktmplmbi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xrcvbbmy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lgnxehxn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ovfmvzak.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kijdujhg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cwnwdhbf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lortiwoq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2tyzngqhx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2uzpfhooh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dymmxrhe.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gkxyewhd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wzmtqket.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rwbaprnp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2iuvbdxlq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2spspidkr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pfufwnsy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qnvlsdfu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ljgubgtc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ljtchfrg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ezsrauqw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2trpbwglg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dffdafux.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dfayhdlp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oiltrdst.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ditypowl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2spgtpxca.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fpyrwbdk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2syrclyuq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kcaepjzx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2csmhrshh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jsypcmil.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ahawwuul.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tfdtnbqq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ubtelpqf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bjogmcri.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ajhyjpnb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rjztlldh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mdkuwmzd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zsoaclhb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qgnkigzb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lfzrebbj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2lynuyueq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kmapouly.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dneirglm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2oprdmfkq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jjhuztpb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2icswwcgs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ocfdhgot.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2opmixngd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2romhdsiq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bzccscdk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jqmcjqiu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bkbsmwlr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xzqpvjms.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2opxnynwp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ghrbyqjs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xrqtggdr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hhczhfvd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zztsycvk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ndyqpgff.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2brlvyigj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2afanuuqc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kwijbopx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qemokbfj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2idnbddmh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jrbrbdtu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2scrpbimt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2btopmmud.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ehpmfufq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2rcycugjg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nirdklqm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qbwyfsai.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2uaqdhlvr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jjmcoghh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2akkzpxdr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2okciyhje.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lowhkhax.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pxceyagg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2skavyrbc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vazgkixo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2uyeasxmk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xonlavol.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vdnxyixd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zdvrdvlv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2cyjzozes.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tdizyycm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sfvwzznb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2icmsuwzf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vmlbuyct.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ivtvbqlv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jyxwdcfw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2popbofpd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2bojzwjfg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uayqtpyr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2skrnphzh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksnmiagm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2uwbokcgh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gmtzszxt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xaptttgd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2onpoxozg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bzjaqcks.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qtcrgkjs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tpioesrs.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2giyklwqg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kmzqxhcq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2dgydcyzt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vecssbyd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2loqtucaq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dugivdtl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2soshiubr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ksoxtxkj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ewcvhevm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qmuytosw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ouzjnfbi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2cmbwunho.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bctmaruo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qdxgoxin.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vfxyxmci.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rmakkure.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2oxyguiyk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tffhiivl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ouirxztz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nvdoybzb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2udvumxhn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dkfytddj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ujlcfsbh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vrvsissb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2whlrlaxd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gcxkjbnc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2iwjjkihy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zvonfldy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eiuqraou.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2snyyciyr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yavtdsks.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2fqmxkbla.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bcbydkqz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2clnwzxmu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2lfkdgdgm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mqybtsux.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yvozzxio.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jwmmyanf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jqsfebng.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdfluswc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2myunmfzy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffzgdpvg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mmkzlbxm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sjcaxxyl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mnlhmkzt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eianwgnm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mjtiqkel.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2niovtjls.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zcmvingx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2nvruqhqt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kunprowv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2viuhltff.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2svavupav.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sirmohrg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vmvfpytk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2namuokap.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dwzodnby.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2odsyqwda.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ksayblsb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yiosqfwb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2zowvhlxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbjiauod.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gwodviuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akzketko.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ekpgnpwr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2sxcaovzk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2snhbniji.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rwizrqjs.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2btqscnyj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2roqjzenb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tttozzyb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bneehbku.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vmrfrgrf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tklxdmog.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hzfaqerf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rymorlop.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2arydtopz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jotttniv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gnfewfvb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wmytyvgv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2lomjrukl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lsyqaufp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rlfgscsa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vbyyindz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rcajdgve.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2cjbfmijp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2sauospue.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jqmvnget.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ukqkwkli.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ijwtvsnh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2oyceqovb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gbgxyspm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mhgqcydi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2umsibfdy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yescsmdm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cnbweeds.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dnrgxlcq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfxmbmgl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2eejwuffy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ebidqwol.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nlfpoelv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2avptusnn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mlboaedc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pnvkjevj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hvrivyzy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zifpkjvy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uhkxypre.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nthbozch.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wiatkcsg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ihtgdigu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ujdjmpjw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vivpdnao.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2osqcupse.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2azsimtpk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2woaodqja.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rkhaniid.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dyyzcyby.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ebjlrrjn.html


<!-- 参考信息 -->