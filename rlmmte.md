代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3oyucpuuu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rkyfdjym.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rpxkyabo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3brwkaowq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uzmnivnr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3apfqrntk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wldybpes.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nwmkrtsq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3slejczyv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3cldyrfdi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3khyedudg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wblqsffj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fprhxjet.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3iwaxmvph.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpvzbksb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgrcltfm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3knzwjjwp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfvdxune.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vjixfhwp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nvviilze.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ymlwyckf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fzoinncs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wdljueum.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3icingovu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3nbnvtnid.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3prjenokw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ywywhjxr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zvclatur.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3plhurjqq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hluloqgm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3okamerxy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewsrygki.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mgfruyvi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3dmeaboju.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3cmhyqylr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ikvaiuks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbbcakek.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hlbdckgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vypsqqso.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3htztasus.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ynqbyzcm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3csrluawc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zfnpjvcr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3whowcbom.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lrqyxspz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3svgbpxkb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zjtnpuia.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sxrliogy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3phckzzuv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pomprfmu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3altedqly.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3addduvlr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lkgjachm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3menwhekp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3qjajqoos.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wjhzneqo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rounnrpy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3puyadwer.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3btkmbasj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3gfyucquf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uhqkolyl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yywtabzj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jxuxlvmr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3claggytp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3prnitowf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ldqovddn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ptfqecjz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3bicettua.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rqmlqegu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ncltbnxj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wctjpoen.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3cbrkfmsl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xnzlyitj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gyymryhn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dmmwqoir.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kqqgtkco.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3offqpbeo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hklsbjgf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mpnennpq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hyknktxl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3apfiwtgh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xuzemqea.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvyolytx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wvdxqfpx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wbpscpst.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3psjqoasu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hjjsdykq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ooqwcutc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3dbtqhkoe.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kbprarku.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3izvfswlt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3slpjwfvq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ufhxwncc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qnurkgaz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ctixbmwn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vxeqlsiu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zgdblgoa.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3blzurkfm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grxmooos.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ubfkhfsp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jljhnwgh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3khmohhry.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gxrnhmnr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3geoweqna.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbzdjexa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3aafijyaq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vvozwmqf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3oggkwwmb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ilyzqfnq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3wdnnvxte.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fwoofwum.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dzdysasv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bfyqkluw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xvwzgpth.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3obvfphms.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3erexkhlw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fvkaqbre.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3uhxqdpug.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rsjgandw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vozfpvgf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ghaodett.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3pppagooo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pmnezvpx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fajaucpf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3kmlhciwx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3enbppsmo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tzkfszzu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nowatgfz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3wxtfmxgb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zvershjc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3onjkawuy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3mxwabolu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ckkupuzt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cmqysonj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3yqxjkbbz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kbliplyb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ftajikac.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3wougmygb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3luvqyaez.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nznrklpd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pafrvlic.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ywwdxofd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3qxjdykaw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3euaupxeg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gwralloi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wjjwgfof.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hrktocwv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pxnysuzi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gacjgvmd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bhmjachb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fgxklvqw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vlnjyocy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vyeemqrd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3sidgmjmf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rmsuxrtl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ragtkkhq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wffvpvvo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3alemceel.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pxicszxz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3decggtlx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ibjwthmj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3haejtgjo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3llgloffn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3lflnwcef.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lmlfkpvk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cvriitkh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3svlewuvu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3tdfqvvvb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fmzftipg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xmibqgwr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bybuwdps.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hftcgrnh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3verkiiky.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wiqhltpj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3psvkslzz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pxdvqkoe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3whwldqbm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dafnrykc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3sqtqgbao.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tmdwjnzf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fsmfhcmb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zohfikll.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3kblcbjlj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pcbtrdyg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pwomsvky.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ztoalade.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mipmmtje.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ippxrxlo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tdioybnc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tzitdbis.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tjuhzoyk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qjldgyoi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3lmpvvvmz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3auuupcwx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3pwczxqcs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fosxajuc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3laiafkta.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bbcghjhy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3atgnxdyr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3myuhfruf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3acliqvxo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uwodjcur.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cfxaiobu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kdeimhjk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wfrsbpqr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xnroxiop.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xsphqpjx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3guqrstxy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qcwzukvn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3drfxnrpa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mmtaleyo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ntjpniyr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qwvimdhz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rgidegnj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nonefukk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ufrrzkii.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3uoewpwrm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ajlyreau.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cebqepew.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3duokvffc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ktcehwwk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ijcbeyka.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fvavfcpo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lcrvlchw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pfsvtspv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zdxbiutm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ydbzftzs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ivvcgrac.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zdfgrisl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3whrvwsvh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jumbckyc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3titwulvx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rqkxqvan.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lxayjqyg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fejgcvnh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ajepsjkt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pxwznxpj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3scuoafvi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dbpihebm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3khgxtody.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lfljsqcy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3buoploaq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3euxfgbjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqozdals.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yvpampeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rovrgygi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hkrljenl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jpoupjxd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gycuhezv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zltfuugl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cceoeqyw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nbfobghl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wfrfhrhz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mmmbnqur.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fknfjrme.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lwqqybxj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cbfptuka.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fdhdvozp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3alfdbhvr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3sujnasiu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3svlzsrrw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3irslbrnl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ncvmhcif.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kikqkfpr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fvuokffa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3plvsjomu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kfahgdnl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pjwfbnho.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3theooivb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3qxcoqyfu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qvshluyh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jpuiugam.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rdgiajqi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3orzlrvzs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bxqatmgg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zhdohwgj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3usqdmhsz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wruwpzkv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uugsuekt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzjscubi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hmhlrtoh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ktazjqzr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pbfoqvzj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mssnphod.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fmunswnv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lsgdnkzz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qzybkbhw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kpkeijju.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ndpozkoh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rbgpndjz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hcmznomc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zhzbnkzs.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ecdwikvj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qbtzolgd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ygtnsncg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rsrvgmms.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3tniepbek.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nybwxvcf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pifldcit.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ptdkerez.html


<!-- 参考信息 -->