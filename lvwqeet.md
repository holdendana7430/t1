代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gktyuxmif.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gbefyrmzd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gasfcaoou.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gdtgmkqwm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gqwxuexrc.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gmtzxnoxg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gwskhqrdd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gvuxfjowh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/goepjhius.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/geumdgqgg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gbqdkokkd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/ghpytkztn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/grsslhfit.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gwyvzjkqw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/grintrwun.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/guubqatba.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gildxrxjl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gkioswxpy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gocphtygf.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gyppscitk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gxaxzortr.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/glmwzxgll.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gatqtuxwq.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gnxyihyaq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/grshmqmoc.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gaxmeshmk.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gkxnytbfb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gbihprqzu.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/grlltqstz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/goafqqcua.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ghlpbwyha.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gkarqawew.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gaxfwrlto.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gigfxknem.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gnpmeksyn.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/grtqwzkxy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gkcovrtlx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gdzfzhfur.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gwxwncdvx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gjerktmaf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gcaafnbat.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gxklmqaap.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gqnadpwaj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gdiyeddib.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/givcoeywx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gsfshrvuu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghoqltktf.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gkowbxccx.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gylefrmjz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gshhhfhxl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gqzehsanv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/grnbzicft.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gnfqxhxpz.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gdotszlem.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gjiyzmdgc.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gysryelhh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gtmzjvqtw.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/ghwnkxkbs.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gnwkirnsk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gatqaiioz.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gslwavbkd.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gdqaxrooh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/glvwnossf.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gicgvicjz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gaofsbolg.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gpajoexlf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gehnasxpi.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gonkfadsg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/grejwmkom.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gjnsdpftt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdozwqddw.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/ggnjweggg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gwzkcolht.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gejnpgaul.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/grpohhtky.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gliorrjxr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/grfgiystt.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gwvdhgqgk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gjxuxadss.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gnqwscmqy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gwznwmnkz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gahwdfhok.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gsnemnlxp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gomrnrsjj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gkssfjrya.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gkkpyqcuq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gfikqwhrq.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/glvvgwdkb.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gprdejltz.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gcbhvireg.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpvzfcimn.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/ggnpwnugu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gpwwgyhbd.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjlgcxmiz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gyxzoovsm.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gewpafuzj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gfdvnhtbd.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/givrglegz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gvrlsfxey.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gsyjcghnl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gumgkzpng.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gqwsktyyp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gjbrmbycn.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gtqzjsdtk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gepiasmeh.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/getenfydp.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gchsutokg.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/ggdqaotwl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gcbeuijlt.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gqmbkpmuy.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbvicvmfd.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gceyqbydy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmdedwdot.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gtdwityfg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gqdezviax.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gustsdyrz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzqpplfhw.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gcybznjdq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ghqqzbnjf.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/geohqnsch.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gljypwdsa.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gyxrlchpu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gsgcnnrrf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/ghspigoro.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gpijjfhid.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gtcfsblnf.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gdpasqupk.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gvecrmjwb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gorrjspec.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gutmexsya.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gitpcadku.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gjzlhbxou.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/ggoxiksvv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gllevwusu.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/getogdffx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gtfbsbhdl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gjzmneszb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/glwkvppxm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gmdaramib.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/grrgsoeyg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gibebrrxz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gmhipymfd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gayakdrws.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gerjnvejz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gluvnwjir.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gtvvssvli.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gkhynthrl.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gwgqqvgam.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gcsvgnxyg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gpksrtanv.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gnsmwqiww.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gjsmxmbgz.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/ggzcpsivw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gvwfjguvc.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/grwglxxrm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ghaklemsj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gtpuixosw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gzfqdpllf.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gukgrdtzg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/guumedxol.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/geiapmeot.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/ggnpwyqaf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gqihtneob.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gzyyvblaj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/grmltvipv.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gxgqfmqse.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gyuquhnhk.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/geljyyoxj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gzdidefoc.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/grxkkzpzi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gjvebswda.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gssrfrqoc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gaehzzrio.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gliivjkyn.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gddvrcjyo.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gfjxdohgj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/grvkacsbn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/goxrwedfc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gtkwpajso.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/glslwkptt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/ggxgvvjrh.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gmathnfxt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gidtnjbri.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gburyjsiw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqvtilhgl.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gbekjgcbe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gbznazdgu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqqyihqio.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gzpejaxyp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwckxedza.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/ggxmwzhgs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gegamxucb.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gtukjodrp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gjehmgiwd.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/goylecquc.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/geapemuzv.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/ghvdoikbx.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gmoccviea.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gpcnwyfqg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gemnsfnkm.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gyhvdbgop.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gtxdotjbw.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gmkbfpabd.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gvaegviws.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/garcrnllp.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gdurddpok.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/glhbhkgmy.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gyeqnvbfj.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gwwbxrngk.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gcycqhmtz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gqqnpjihp.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gvwloezcd.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/grpmjaecx.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gfxczgema.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/giabiuivj.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gelnfsxut.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gscmkfdmu.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/guviczkhj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbgfewdjw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gdvczvhcy.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gknjpllyi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gkivvxuqu.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gxdcqadzz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gwemvrcrk.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/glotknopb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gxwmpuwbb.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gddxpuyqd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gruzsydah.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gqeeftygx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwkdlyitk.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gfrbkjlbk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gxryxboxa.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/galeojcor.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfgtnnngw.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/glqjwnlim.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkmyuvdvp.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/grgsojzlm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghesmufpe.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gfrubzsng.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gzfkrtvsg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gssbuybsv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gspjfwzqf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gurimkfxj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gdibcheeq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gamryfeww.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gxzyefoez.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gyhxkmkdi.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gauzsgcnj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/grcxckpqr.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/guhrwqdto.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gvzknxdyw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbfvmkmrv.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/grauuwyyh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giyethnab.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gjembduvu.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gloklnuog.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gaebrwhuf.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gzqayopiw.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/giemtbpgb.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gasatngdl.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gdjelqila.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gdlnjlbrg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gydifmreg.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gaghbxkhg.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/ghyasqpuk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gvxekoifn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gomrhrylt.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gcsnsbzdv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gsvlosihy.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gsfphngnf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gfevuhdkg.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gjtblvicb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gjmakbsud.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/givxjdimb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gsugdkkqx.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/giwrpzpiw.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gmlxhcrbq.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gcuyegqke.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/ghectxxrm.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gbrpnvepd.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/glgfggxlf.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gmbngjhlm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gnzuyture.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gcgmjscar.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/giuyfpspn.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gtvqwqqdf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gqoaxrktg.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/ghfpeoofk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/ghhdhrjyr.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gebcuabee.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzquxcxlz.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gbjxkqoae.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gooynlbec.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gqctejaij.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gifjphtzv.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/geybkrqdn.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gabqwxhnt.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gvknuzdyy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gtjvtiqbd.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gjzcqudpf.sHtML


<!-- 参考信息 -->