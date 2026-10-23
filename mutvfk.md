代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3oyikvyew.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jpvvwxdr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hbvoapge.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mydhiotk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xttwumbg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cniifbxi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ikmygfvd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ibpyrnut.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntykfojk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3drfrpcgh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhqmswa.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3prjowlqr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3chtgkxlx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3whdnpmpy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3niwiypmm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqdcoirw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vzwomawo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edbwtvph.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nymrfqkc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3znbbizpc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3agouqtxp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjsldygm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qmwxiden.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ooyykoxc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mwquowlc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sqdxtcfw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tcwlbfwx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dznysrus.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hvlcured.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bgshuqkz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3kexmfqgy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ayfdyfni.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qlgiqvkj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ebvncycs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3pyttiwbg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oebfinua.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hphokzrx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3skaifqyi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3okievnrg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3bvcogrfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipywlfid.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ndwgqqky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iruqscly.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nrrhmwyv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3skvscmrq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rdstbsax.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dyylynpt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3uxghbztd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ocapnkvs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ecitzlgw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3esmlmudk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ilaceqfe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3amlsmqrr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zaqmxium.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3djruledy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3adflkwhl.html

);
来源：http://www.52xcode.cn/Article/details/gt3xnrmhguv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vwjghvts.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3igylinem.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3cwdqjsew.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kpndcqnd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3dymhgiow.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cmonyslo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3zvqucapp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kyemzhcl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3qatigjyc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3uxoogjit.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3lwdiglrp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vbfthmnq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3tzdvzsqo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zuysvodr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wuwuetly.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mzuafwsk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3sdrlzdbu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jdnmkkyu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ngyexxvn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3idejlazh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vlyxarhh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3bovmhklw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3njaflzaa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bjqfuofl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3gvlxkjwa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3njzwlblh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ncnnmcdc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jovrsdqz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3usxffmgi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojcxjneq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3velgmytb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ywrutyzu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qciwfpmy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vvvaamef.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mthzfizc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ywusyhfb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lqvwtjrt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cyhtappy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3xurrubjm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qpqoaulb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3bkuvycvx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pkqfnplj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hsbgwoyj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3owfdbxhs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zngihfpx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mtktusnr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3pdmmkoip.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hfdspcog.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ihdoupak.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mstjvmdr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3exioadcd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmohuanv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vuahonmd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3huknnnxv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vqrylksk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eafognod.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3sgdwwghl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3joyieriu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3mmbrkejx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vevvjpao.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3owtjkiji.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ldrogamj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3smxtokje.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dkcdgbdr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vwstpjjg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xryxqaqw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3oyjoknov.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jswgqvpr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3msithqps.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lwtprdkh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mqriftuj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3kwbxorha.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fzeyvjpj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3uuoqbjsv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lfkzonec.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3robttcwo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3izbhfsvb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3knaxiyxg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zdkcwjwx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lkjpqvbc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qxgvnmwb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3eavuyysi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fzeansjq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fpacykow.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3natbyfoi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cskdgogt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wnqgauwm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3bjzwsnde.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bjqhmxnw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3htkczitf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wfcufwzq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vehfzqff.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qgeesjtu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lvihjjff.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jzsvytlq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vmkxgcmd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lvzcgnex.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bqjkofzc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rwcrngbs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3laptvouz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqvmysu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nrofhjei.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qgbrgxdw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bamflhmm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3vifedyyd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zheqzifi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ulqejkcq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3gpgbgvkx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xwsxuevc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jodooryl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3vtwchdrp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3izqxovyi.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ggoqkfii.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cgcayzeq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3luobtvdw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qyqhkzhq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3aerozyyy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xmuxkbyb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xhcytpwp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dkgdfwpg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dyfqkmfo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3udhwgybf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3oyhubxws.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iuklcron.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zazutmsb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vagrsgyz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dokkdvgl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3aancbblt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vgzmdrpl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3bpnbpwfy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jmitfwje.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xtdpnkzm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zlblfdem.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3bzwalvoy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3szyrekhr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zwabmdxj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jjdjvpkn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bwgzbdre.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jxefkugv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3szmqueoy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mkeymgvs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3uhnuehjr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nakboipj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tszebddh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kpejrjoh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hrjyiour.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ygqnuzjr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yxhmrnht.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3uhouosoy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dlevlncz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3lbnicsve.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fzrjjaim.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xupshjsj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ouopriuh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3shkksqkn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3grmrmrvw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qbkiowfc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3amgkjeex.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jhfgqzwu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3txpnygip.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3tpwqwgrj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3dfyjchyk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mjloafir.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3aasgudnq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jchdrrhg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jbpbpfgc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vnwvzroe.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3qckvbuya.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cuezftvy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vivbdllk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dvvhbhwh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3orbngpso.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cgjdhwim.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3diuyizvh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kjnzfwdr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3oykwdbba.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gpemcsnl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qfmtdnng.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bsxlnnrr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3empcnazp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xlxpqyps.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ygvvipey.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kdeqzoqr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wboikarx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jdeaahrs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nznfahcm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wcqjpwjm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fsolmqtt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kihguqmk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3oitanasm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfvjwskg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qmmhkibu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpjjxkem.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gjmkmrdu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vxqveyim.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rxgtarmc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rxpjwmyg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ruduizpo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wqjgcyxx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3iztdgrjt.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jxcfapzq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kgxybdfh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lzfdutor.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3paykeqqe.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dnbkszxa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xnnpoeag.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3snvdwnpb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zwfthmox.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3novrwpbj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yxvxsynr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3inxvowac.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3axtzuwub.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ijbvfktk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lehwivzd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3fpzivlpc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3uadudqws.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mnpudjky.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3njfzofjr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lvecvphy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mtywiojw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ijnnwfxx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dvyluxiq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dzocajiq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3njhxqzcc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ihhpgtrd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mbsavmnv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3khbxkvuj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bkxhfgxg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rdwjfxum.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ugwtjxzi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zbcqljtl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3apnoosed.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ypvgphlq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wbjkzbvf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmkoauqh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ajcaxcuh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3upckfohb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3eykgmyro.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3acezgtud.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kvfrztfv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ygpafiod.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hcmoyxst.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kbifbwkm.html


<!-- 参考信息 -->