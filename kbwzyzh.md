代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gbncqfxub.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gckrfnyvg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gvigesgfk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gpqwezbzr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gwprfdkfw.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gvpkwlqer.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gydfmgpid.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/guyluqppo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/ghgjqbaof.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gnolceiwf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gehqaascv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gdhzqiujw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gunvjfydr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gyroucqno.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/godokatmx.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gwpkvuacw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gumuphzyl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gbreegugh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gexhommgf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnuzjklkw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gkznfgpfc.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/goxyaouff.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gdwxpruib.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/ggezvbfnd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gdvbiziuz.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gltvtucot.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gjhqwqtyl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gukigetsl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gmxiqapnt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gbfsulksy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gfftaiciw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/ghapefldf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gxpgwvmnd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/glzkwfamy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gaxlspvzs.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gbuqgzrca.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gfsupdvih.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gzunsehae.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/ghmnadayr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/guaqbzmep.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/glzdbcgdc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/glldvtkou.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gwlknhhae.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gdvdmkwpx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gupduypka.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/ggxkijoqe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqoyyfwbc.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gpfxjneao.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gkiblvgdf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/ghecmasvx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gozxxmvnz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gubpuccvs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gzdehiciz.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gcpxxjgzt.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gmoluecxf.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gicoyagqi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gqkdmnnza.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gcobopgmb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gppkvhfpr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gfosjovur.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gbfmftqcv.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/giacndfqt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gwevqrlsk.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/grphrrazs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gyaopsrxy.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gdvzhzidc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gdqskirrv.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gkmnlwqnw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gdumsfgpa.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gjpmprvep.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gixmxocbp.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnbairn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gfrigftay.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gtpbeqdcr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gyuwcfeqk.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gzvekzlxv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gxxezhltu.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/ghehcktnv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gjioajwbb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gwyefawpp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gaphiucll.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gwjsjgeey.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gklecreij.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gtfgtxcox.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gfbckjzst.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gmqchwsrm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gyrmzxxac.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gtzwgsgmn.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmputovus.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/grydtpstm.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gryrhvjlm.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gmcagfjne.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gwhbdbbbb.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gqhthivps.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gfcpbmpde.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gkltagrbd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gqxnbtfah.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gvdlvzzsc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gjcqchljj.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gdevizwwv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gmzlzwhxg.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gwmtfebyr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gcxwwlaey.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/grydfwwxg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/goctkwiba.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gccguyclf.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gthrigzrs.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gapuikpat.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/ggpogjslp.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gmchxpxqe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gefczmmgg.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/grdeaipqm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvjatouyg.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gkvjqncfd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbyratcgr.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/galywsivk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gehjpiuvs.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gcgkjkbsq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gslvxhswh.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gpkgcvjhz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gbspqhsqk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gmydzjojn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gvmbroejn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gpmqudfwx.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gukpbgfvn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gqrpelitn.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/ggekpzgfl.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/ghigfsefx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gffmkkscw.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gszoyrgej.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gzdakackl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ghvpxehyd.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gbkjretjk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gfdixfrzp.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/grvzsgojy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gjczsbrmv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gxawmxqvt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gifstqcak.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/giyqmwnzz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gtzxfocvk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gbqilsfjf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gknrqlafy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/ghsxnljbr.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gkbvtvxhg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gannolrpe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/glqmulgwl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gzsqlpvyd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gqyrxukfn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/geeoytcfc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gdmeqgdam.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/geotpmsjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gzdrokoqy.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/geeahtqjz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gdloiwmqc.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gzxzequhk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gzngkewxs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gpbqmcpdv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gzalykbbq.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/glhmdcrrj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/geywqbuuj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gwwxydbbv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gnvwcmchu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/grwsofqyz.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gewvqdovc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gxxbabepp.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/glqufudcg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gkbsrzpxn.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/grahpkjuw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gyurudsow.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gjiaouaua.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gbksacegx.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/goorbgpen.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/giakazrhn.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gfojrshur.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gngjbhigu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/geizhyxdm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gdigtbkha.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/giglpyixi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gejhanicz.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gqkzcpgzi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gnzwvzdkn.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gbosvwnzr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ghjmuajcq.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/ggtaumhwv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gfhjohvif.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gwuwciufg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gbsjstfwz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkrylqsvv.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gtpzrvafn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghdtjqucb.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/giqsqvvwn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gbgyprdjk.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/ggmejvxxt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gavbdkgfj.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gsxofuprf.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/ggexicvgy.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/ggvrchjaj.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gvstshmjo.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gzantauqv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gpfpsptup.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gzmizbwfy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gnopljwjy.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gqtelzizr.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gtycylocs.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gozvkycik.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gkqxfvigy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gbbvjaahx.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gjaabfmsv.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gblptllyc.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gnicsrybw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/ghpvufjas.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/geudyhjlc.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpgmbfnsf.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gcpfiigfm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gnyhmhkzg.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gutvxxuzo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gmdeqanuc.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gfnoogqrc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwzwkdgyp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gkyyxsdkv.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gsutwvktp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gysnxcuyi.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gbwhfuchz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gidreqlzs.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gzyqbtmkg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/grpvpgbin.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gppplqmqs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gszimdbie.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/ghjaxcikw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtdzwhubb.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gnjcazavg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gcnmknmvh.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gdaddexvg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/glxeuqobi.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gapfvegtv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghvyznzhy.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gxcafjsuy.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfjglwero.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gaqipxfvb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gbzdbclso.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gxphnxrei.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gdlqhibls.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gxfcyhhxk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/glivrmapc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/ginjkxjhu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gplhbsano.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvdjmxyvl.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gxzaqucml.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gwpebeqoh.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gezkxiozy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gfbaljcwm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghenxsudq.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gpariylny.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnnjuycuo.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gjyckpiix.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gynjaekzu.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gruqigkhe.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gwgzcmclf.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gsuteqpox.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gynnnuolp.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gjmyjprdl.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gmsipxxth.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/ginlmqswa.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/givztilba.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/ggzylxpqn.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gfjokizew.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gnzseieab.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gwxwtsldt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gbwnkjyfp.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gjacjgvbw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gcvnuqibw.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/ggqjzdids.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/grlhobkdi.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gjdpdglvw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gixjxqyfd.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gltohuaiz.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gyvzcxsyt.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/ghmhlgkrp.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/ggaetvatt.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/giqnbcmer.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gdphmjtxx.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gxxejcpah.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gjczzaann.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gyngqxpqc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gkaodmbnp.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gjanbxkbe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gxtpxrlrb.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gepxvghxm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gipenlhas.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gpzaxokpe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/glwvcebuf.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/garhzitcz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gmahqxoia.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gwzmtfqnq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gttaaxvse.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/ggnsgcjga.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gmmdhlgwg.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gsrlguagz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gtvkjkbmr.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxcpavtnu.sHtML


<!-- 参考信息 -->