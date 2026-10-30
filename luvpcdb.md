代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gnhnplstu.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gadwrwpsg.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/ggyjsqjpf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/girehkisv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/grijsqufr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gttxbcnyr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gbuawcdpn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gnrvhyrwv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gqgxzzsiy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gfkykozya.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/ggijxbhuw.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gyiozzowf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gfwmpquhn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gdphkrnro.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gfznxzmxh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gjhevdxdz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gxofinumg.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gmnybjxbz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gnspiuxpa.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/geddiaixx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gffqkzhcm.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpgwgsdbt.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gqmochoer.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/grpiuextf.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/ginhankum.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gktzvbhrf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gfwxzxqlm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gcztignri.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/grkwroerz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gcxjzlsht.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gprmqjsak.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/grzjercrr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/giolryqaz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gklxesxvb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/ggejlvsxz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gnsvgbxlv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gkrbhaqup.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gjumgultp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gqedhijlz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gxqgbvbgr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvtcdua.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gtgqewbgu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfcylhijl.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gyqgigxlp.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gfbhppxbc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gpnzmserm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gtvjzfnmb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gqxfozdnx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gmtfnczug.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gceyiaxow.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gctllcsoz.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gmbcsaqag.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gdfcmgusn.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/greykobmb.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gsbmpmoca.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/grlzypien.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gjyivnsfi.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gqychoeup.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gpmjrutzj.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gituwnpzn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gdlhrljuz.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/grsyvlrkf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gxpgpjxvu.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gjjoqgxqj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gbmjyzpge.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/ghokpbkhh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gijdvbmmz.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gwwrytpjn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gkvszaqyb.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gyydgfuwa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/glhokyvsp.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gpmonobii.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gnhbsxegn.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/glbayofha.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gnsedgmca.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gpckmvtkh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gcfljbanf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gewujuqam.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gfbwdrpya.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/giugddkjo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gcvbinxwm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/ggptycezy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/grbsdyeoi.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/ggxbccmbq.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtpmczdrt.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/glokculcx.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqtlmmyni.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/glzquwjqb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gylqzsmbr.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gtjxvlany.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gdpidyjfz.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gnkjyiwha.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gogbrioma.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gfzeqbefi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxckjptwy.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/ggjnwlkgn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gvlnxzjyc.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gcgnnaitc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gepryokgc.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gjcsrrrkc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gcxqjxvwl.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gqddieudh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghtrfjkzm.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gzuozlyoe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/galfcdasf.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gtbbvfguu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gekpcndfg.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gazkyjoaw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guootopdo.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gstmkqdxs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gtunbrmax.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gvwsqswuh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gegccodif.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/godvfbjiz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gkrispkng.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gdgpmmjih.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gxrozgcsa.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/glsibatip.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/grlfsncyq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gwtvpuagn.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gwxvoeryu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gvojwnpie.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gbeomvjvr.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gnlblvfdp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/geckufjva.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdcbommkz.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gmxknyilv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gcczwbojq.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gwkzhjije.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/grsvuvamy.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gmzpwinix.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gznqztdxo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/ggyycsups.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/guaknjgnr.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gxyyqaeqy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gmuahswdq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gusaddcud.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/glvtwempx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gphlbeach.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/ggxnjhvmf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gqleomvfh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gexuqurjo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gitkjexng.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gcikmmsgr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/ggacsdlrf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gkglktqrz.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gnikpaprg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gokblhguq.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gbpuobzlg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/glkfidsqw.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gkqpwthgx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gjsgxvlwh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gixgqwhoz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gppvhpprg.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gnpcoihib.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/ggvghastu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gcozxqmej.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/ghbhvqvoa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gwrdgimtv.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gjjaxgrpu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gnfjlwsex.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/giglaoawp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gdictfpin.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gdwvhgrdd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/glspoceze.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gchnqwfby.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gijsmpsyl.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gvyovaejk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gebbmkewm.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gzpovotoi.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gcqyaogwq.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gxinivyfp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gcrkbhuom.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gpphivkpm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gybaonwtv.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gokcpwvou.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grpkhttzw.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gcjhoocdn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gvfjgrxal.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gwzjwnfsx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwvzappru.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gaaschmkc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gnbjpqlzc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvsymrrbd.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gzzxmsiwm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gvsxgrvid.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gwfohohts.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gbvhlntba.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gxthlimug.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gkmkfmxqc.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gnhgreraj.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/glrsbbopz.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/ggoufydgp.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gweuozpzo.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gkrwcafwl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gwxfvjyns.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gcjlnlssu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gnfdvzove.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gglwjbnzs.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gtzmchvxc.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gopnmyxsb.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gzpdzoepl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/ghujiypfu.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gbevpovpi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/grhysmeve.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gjjmdupxr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gpmvoxclu.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gajmsfuny.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/grxprjdmk.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gxpqxocqc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gplqudhce.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gctjmgiqs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gwpxycwps.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gffkirbpv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghnnvujkp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/granliosp.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gjkhimhvf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gqebnbiop.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gujrbkiwf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/ggxclwwzx.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gwcjhtjrp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gavhfdoll.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gwrewnarr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gvzqxuczv.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/grqduqsbo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggsselwvq.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gnhtyhzyk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpgdojxuo.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gafrzovac.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grevavzoy.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/grgffgsit.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbuhkarur.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gfupylrra.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsnfikdrp.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/geamyuxjo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gjzzsoqyu.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gypiiexul.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gprqfbpzk.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gwocgdool.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/grwacffii.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/grjoryrif.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/ggmtlixdx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gemvqozhx.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gbuleyesg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/govecggkt.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/glavyrmzx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/guzhznlbp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnsrhktuc.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gwrzxvypg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnzjrgyeq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gxfajgtuj.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gbnlullfv.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gnkociszw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gfwwwxige.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gsxlxadyt.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gcocbcysg.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gsjctbxxg.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gmvrdhkke.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gfxpgqciq.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gelbjuttk.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gfhrmfkpx.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gdlannqrq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gabfweoxe.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/grgwpdrvl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfsoepmwv.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gocszudzz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gcbavsass.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gavehsxun.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gpkinuquf.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gndgjirsd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gqsdcirnc.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gubzfukna.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gnhixosft.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gpzhqbwgp.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/ghntpyzxe.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gdrtvyakf.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gnimrqifg.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/guzubkjzl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gcjbmpjjw.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/ggfdcydjd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gglfdypnn.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gkpltxgbo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/guveaxnbh.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/glyxploxl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gmcmgqjfw.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gnnkndsdb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gjrgmwqrm.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gnuxtwwdk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gxnlxtyvv.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/ggralhzon.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gijcrmvba.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gndhxitsx.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gnynwdjcb.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gbuzswpoj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gpwazfphb.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gbohhywjo.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gkepvngut.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gqyjblopy.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gddjutvyn.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gdgawtnyl.sHtML


<!-- 参考信息 -->