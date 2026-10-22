代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2eofbaupm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aykpokdc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zzyfosyl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cfibaydk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hijceeej.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2cocwqrkl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2awheaxlh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ppewpbto.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ipcjuewv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xrxvreki.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2phgbwqdc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hgjizofm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cfoownsq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rttfuyrc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oeyynbov.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dgboetll.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2nvgluzlh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ccjmxjvx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jtaizzsv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rznkogeb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ycjltvvd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfzjfmuj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtgosedz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvmawosf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2sqfvchjs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2cjwfchqw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cdpdspgo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fierwzll.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2uqbkjzvy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zjoykxvb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2brrnoncp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zidkyqxa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pyrxyxwy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xclcismm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zepyjsky.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ahqvnuua.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2pczmnskm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yxwtfgsa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ioyeruan.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2heennurd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wemdbsvg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wgdvzubo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gftezfoa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cxpvrypj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npljvkef.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kadwgpdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdmmirii.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fbissldx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bthuecvz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tfykxmpy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2afmfqoey.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2haydcrgf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2eznmcofi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mknhyesh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2avoucgti.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2twpluzkh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xyvkjtfr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2juwntdrm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qoeugrnm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vngnwsiz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uwuovxzk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ikzablnk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wtqgcoer.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2whpmodtn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2unyvttqw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2crftjgxd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2uzryiukl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2yhscuknt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xytwpztb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2txthbqia.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rjqglkqo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lrjwjyun.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qackccpn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cwrorpjt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fjydenwr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qlszzdpe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ozhtlmhv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jbethemf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qtwwosiq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dpkywaqu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2flureuhm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hcjzjbpw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2hyxnxjhu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tdhtxfzl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ojomwvcx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wwmvtzhj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dwmjqtpz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ybggqrln.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2efrehpvp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sjcpvcwm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ayzhvoax.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gtnwhatn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vryodpnm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nesilulx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ahhqtyip.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kzuzmwfc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2gvxilcsi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2smomqfcg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ycgoeqzu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bezewwrv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dfjtddap.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ibtbljcr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2yqeuastn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ngfoixmu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lelayome.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hxftkzap.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pfvwbtld.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2heqbxved.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ulkybxjg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dosdwpud.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dijrpmrz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bzzcddri.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2keawgmni.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2flpxdthm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bpolazst.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2iflbwatr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2supezpsl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2polrsusy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lklhjaxk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vdxmtizr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2syoqhzvc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cozojrcr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uqqopbzq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rwrtcjls.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2oardkbsq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2aztykztz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2nkqezwyb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hjouoijw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hybqlfua.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lhioslnq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bisccgqg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2emyhizgc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zzjxzbda.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qixncknr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kclyotvf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ousxrjdg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kgsoyftj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2norijawu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vnkyfudb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2uqfzrlxt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2oyadxmbd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2lxigsrdm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kfggjlsu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2pozertmr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2emfodcmi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zrlvoqqn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2vjpdzwyl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bdirlake.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hqhzlnhx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2taldhgxj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jpwyvyvt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2hlwxtimi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rqolhhjk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2uyxxvumb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2shlijfap.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rsbonhbs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2yjgfakns.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ftkrfbyw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bbjdfxjt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xukhyobe.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cjqsndof.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mjkznluu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ggngmygv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2hnklnrfg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ueuoelwk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2cikmgyll.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lymijicn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xweciwvr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rdywjfct.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ssvkllws.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2irgslhfd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ygdwkioh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rttsjwap.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ntyhchxz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2kgztagch.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2coccgkrf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wyybqxxj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kqfvrpjn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lbaorjbw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2uurnwpvs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qgkmswtq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xsbjuuhc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vwatjdyv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fbbclahi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iytwford.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ukpkmdfu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yblhnega.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lywahteh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wulrzaih.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fjcydqfd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jlwpmhuh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zqojepvf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2dixggrvj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gytpzpof.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jtwdinie.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yfgfjswc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2gsfobucn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2pxulzduh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ioqudyek.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gdpqwrii.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bjeljajy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2frfkqykh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2burqabhn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vgauqhxw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ejaqyhhw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2yygsrsci.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nkiacfwg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2aphhbclq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ypvnbyck.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zqmwnkxw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2sjdbbyky.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tvukwadd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmetduae.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vacnibar.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2evjwoatg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2oziitzkb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hvrztcxr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2odtlvehz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zdtnenly.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2djhjlhpq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2krzrsutm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pizpqoys.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2axekjpif.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fadsjwxt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rfozlguw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bpbcruqz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rdqvfrej.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mgpmyuxz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2irygxwla.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opilqbkg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sntvfjog.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gkfkdqam.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yixjpkdk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rmignulw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sgwrffsx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yeuybysa.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2lxzgfoln.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nssaqblv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xqstblod.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lcnmodwz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qcmeterm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ftlhfplf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rsaioipb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ytlajlqq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jxbpmhij.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mqpnycxn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjbzauga.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rnjeqdxa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2flerfocy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ymvpswxc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2thbearac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvfkkjhu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jevijcqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dljvjtol.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2wjshxzgk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2counwark.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cygvgycl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2svnnldrs.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2sjbivana.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ppvrorxg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mndizfdz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dllkgbar.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2mohttaxc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2esgapyrm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ndnknoos.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nlkedcdx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiffcwwl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mfekeuiq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ocagfrrm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kqlzzcia.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bfwrmgcf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gjkczzlw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rhmwhlet.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fciihfjq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ulfulxuh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fbzgwinz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rttyrbpc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kiemtdqj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ngywimit.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qilhqjva.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pfjykmgk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ruqvhunb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ekjdcsne.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2noygzbhy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ykplyryi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2pyyxzvzc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cvnesvhv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2szrqdxvi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ojhmzgyw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bgmaszmm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2emousenk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2axgxdsrg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tnzsccoo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ytvlunel.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2patjpgfi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sonxtmbt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hpodgpgi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vhfgshax.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bpxdmkpm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kswzfjmo.html


<!-- 参考信息 -->