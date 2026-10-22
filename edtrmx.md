代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nynuqluf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2sgjyqens.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jucfmvel.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vlergxfb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fyeeydbc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2zobwklmt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2sibbfrca.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2bbzcbfgd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2geuydhis.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2dzwrlplb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mkylfixs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gvtelsqq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ojcuruzs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2gsbdbkor.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rmorvmfa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqftzpla.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2fidrfkdb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fexahkyb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmqexprh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2khttuwxe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2powekjmw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vnvucrid.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2fpvinmiq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2aiitmnxt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jmkpmhcp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vifolzrb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tbwmhpoy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ohbeemlj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2apffknxz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zwkxkcym.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jqqizslw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rxbetogw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2tsioxgbu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2diuuvpeb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fgjuncah.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dimveghv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tufvkaiz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rsvtshvv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2pnsqckjv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2diocibgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdwzsmhj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bxaaaxrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shdwmmjx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zepknskr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qcfxjlsx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2njgljznv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bozkvkzh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kuhnjevt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pucmpgkd.html

);
来源：http://www.52xcode.cn/Article/details/gt2ewkrmtaj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2iuyvnorh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2clphieiy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bftydvfy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jrkidyim.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2eghasjkp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rhfnrpri.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pacbozmw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jofxjafl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ywjesgvh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vmzoblka.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2apnupauo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rczlwkjk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ylseoxtx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2uuesholq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2txgcfmez.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ajrhknzh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2maqsijla.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2koajmvys.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rrrzogey.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2nkihskpd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tifqkbnb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2onddbhxk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zihjnecg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ltipmjuw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fovhoncf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ezsftzfe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qopkbffh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2fcqikdiz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ghpmhdzc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bmytvyfh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2twomwpqe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2vdplnskd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2kfmcmzow.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2yrehbmrl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wkvtuelv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2alxhxbwh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2torjbhlp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pjmkszbs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kpzbwopd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zefgspve.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2npnbcdfj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2avvfiueu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zookoklq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fosjgirq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hueevfng.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2lilitdbc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nrkjjijy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2psaashyo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nyfqyagz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2joqjgzas.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ijyybnfl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2khgycdyu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hnwekysq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2uoxkxsfe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2naarjlwj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gknifqqj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lznjnvtt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2uhtclcul.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xnkfwjug.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ljjvwotx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xpaveimi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fptxpyaa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xedctrqd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2veydpdts.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sgaxvzdx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lqnxvosl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2pyrbcnaw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sqnxhtfu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fjgllghe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wxllfvzs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ibfhutqm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2yarnftrb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rihbtxuv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fwwoilqg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gjmgmktv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2swwczarm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2trhdfucp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2innhowfi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2smxgmncz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tftygaof.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bssfhyuz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2mitojzfk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cgvzqmdu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2taewhvcw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hsgydwsu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jeiuwbcn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zixsmkle.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2lqguqyyx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xdbglibr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ykduilhp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vnuhbbhr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rjzrmjif.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jqwndaes.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eadizssi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mmspqlrb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2okepmbzz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ivfogpkg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2npvovdpf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cwdbaoje.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2crzyzyoz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2faegeygn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2avzrsevu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2njdhslld.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ikbfusax.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2rctobgze.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2iondqjjz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jdszlste.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ibbfqzwc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2onnzezlv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uxqcjxed.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rfrqehcs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2sxljrztu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ieottemo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gepivuyl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mtkllztc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xmyrkekh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ocumpzgt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2sckahyob.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2aajqhges.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kfwcuruj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xntuopkq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vatvotds.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fkvrwgfb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fmrpdgux.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zgckehhk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ogsvjwrf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qbegkxol.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rnvttuev.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qkxjyiay.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qviidhiu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sqgxujup.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2emlrirgk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pdvkuqdd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gmwsosou.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2cpnjokhk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iatvmmrl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wkjhwadd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nkcafypb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tnrvhegi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xditvpbl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qxqtveey.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xjsydkpc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xcnrufsg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ulahscex.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vtwqfqeu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zfpavsst.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dyshstmq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jntmjjrk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2gxxzlvua.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hkwnmpte.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fomnsjhn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yfmelezb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dqxlcwkn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2gznluqxw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hjbkaize.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jzsmwgfr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dsjpujva.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tjglqdna.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2raahxqud.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yxehmfau.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ffszsltb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fblwjklq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zewbiima.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zcwkggmc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qgvmbfxq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2yyygjmtz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rgxpkmvm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zsjrkhey.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rdkvensr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2svubsahh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cwndgumr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mtggdjmi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2boinklpv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hizwjazx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tjjoxzof.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lykqudmo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2irxmlqat.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nhscztyg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vhkwruyb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tozyawyo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fyrpnhmy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qxmrcyck.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2alnchhcs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hgkroazq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2eteqwprp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2fehdbdvh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pshrhond.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pduhhobb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2qungmvse.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tigwamwg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qmlrmdtq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2arwikujo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fwgrgtkf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yediwaek.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2urxporug.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2njbrsirf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wjviqsdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhihjcgz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2piabrygv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwtaoyys.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2squmecsp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2udwvcxxf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2icmfqxhg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gsqsshkj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qyfyiggt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rpkbfkqj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cvjjjucm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ustfntlu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2mntwejel.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vbzvccjz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xworowqy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qujtuodx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2caosczdk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pcdvdnkd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qdonbuip.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2etsqhflr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2unuovtgz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ggwsbedg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fxftwkmr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zcojccpw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fusgbqsx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xnekjcpw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2oqhbhten.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2irheiiai.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nnqqtdyi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qhzrkqqj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2iejeeodq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2horiwozb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qsirvwcs.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qnuuihoy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2odrbjqkx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vwahdxel.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tugoejto.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dkdzwwzh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ukjnakbp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2dcswyebq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gwgiepvk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vjssafac.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ronadyuk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lhymyqzw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2htymnlxo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2txfbmnrf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rievgugc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ruhdyefs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bbsajslg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ztetcnjo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fhughocj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ypattzge.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hvhqjysq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xgyftelo.html


<!-- 参考信息 -->