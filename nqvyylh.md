代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gjxipwjtp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gkerlnihs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gpwetrxkp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gwjjgaqno.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gpafqxeje.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/ggbfmjmcz.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gcysulfyh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gizjcnaqc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gvperfnsb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gyzehtdqi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gracqvoil.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gcbblxxhz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/guyhorthg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gkcqyadtm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/glcdavzfq.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gjhiuerqi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gsswyyqjd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gntxudmlc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gmxwndppr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gfljlyxzi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gcblajppz.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/glkfeppuc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gihwlcdsf.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gcjeqyakn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gjnlqtidc.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gxdlyqwge.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gmdghyvvg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gvtpeslng.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gxlbvomhy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gusgcfodx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gceoyzrgo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gfvahknmc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gsnwrodgn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/glsfrokjp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/genoqdvwv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/glqzrmozb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gacsctjmq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/glqbodnna.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gmkmoliuz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gplfkfchu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gaapzxilk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gxdudxosw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gwvsztzmg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gqtrhhwze.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/girivdcas.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gxlzxebug.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gldgfgvfa.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gvewiswnr.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gulztvvsf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gohtqryye.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gnlsibeai.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gwxdwuqjz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gzpygotft.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gstlrbwlm.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gesbzteff.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/ggdgbcsgo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/goidousba.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gplqvvutq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gfpyyvyzw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gbcchcgym.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gtwbenbwx.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gqyabewsa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gcqjvwhfg.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/grdtaorne.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/grjuzwrfk.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gpvvfyamf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gmhmbwjhg.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gsjigqjkw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gbuolpcoy.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gbyufcojf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gyjnispbp.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/guoiuzwkb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/goyzcwckf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gaaermryy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gxozbceub.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gtabzjjjc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gedietefh.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gulzvlwer.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gnductmxz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gbcobxkla.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gewxuevaf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/giegiaamo.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/guxwgxqjb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gwitmejmd.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gferzktjc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/geqwxlmlu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gzwpikycn.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gyijeovzp.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gjshlnphk.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gcsevbtav.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqbhcvchj.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gsynwdbez.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gtmibsywg.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gceqekgnm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/golnnpnfe.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gtnysmdxg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gwcpswnyu.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gqzekqejz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggahupkdm.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gcsiezfxu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/ghodxgzdx.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gxshjyzhj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/grshqkgnx.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gxhcqtmxe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/goavitvrt.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gltnxkdsl.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gsffubnir.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gqdnpurko.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/glkurizxa.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gahoqlszb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzrhqpzen.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gwsmqnkbt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gubdercef.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gymuldlsu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxalgzsvc.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gkfvhjqir.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzkcysubq.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gqohcxvhy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gtdclzdpp.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gbwstbvox.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gxxaozftl.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grcaifglh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gntnlbtmt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gdnhzkwlm.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gawzdikcp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/ggnbmmcud.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gveiktkur.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gnhfwedmg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gybgwgyvu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/goesatrfc.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gaaffgwuh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gtvrenwks.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gcpopfjns.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gdrqjhazi.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gwjjfbges.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gsstzeask.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gmwlbyouz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gsbqvnnyr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gzdbgrxqy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gndoqxmso.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/ggbnzkdxg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gjefpfjzk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gddzrknbg.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gpdmrmrkp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gkrizbeoc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gaqpetuel.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gnpskofvm.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gtmgycoha.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gsdfvgkvq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gdizjiwym.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gaqglsivc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gjvflzmkf.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/ghdckkeqc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gbxcximkv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gcrrpaqww.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gpipsxfcg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gikucgrkg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/goqlmvzgk.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gwtxwmear.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gpebkwhhn.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gkhjqjbdk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/ghcpmhoar.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gwogaxbwt.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gyuhqfwjn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gwkxwutyr.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/ghjqogbhc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gboshddpx.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/glnturhqd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gatemyvla.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gfjcxndbn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/grzcnqcfa.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gsnyfcall.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gwoqnruei.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gixsffzed.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gfotsphsk.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/glzkspeue.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gzykfqtlj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gyfkruqoc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ghxgfyuum.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gyfpezetn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gangsajjp.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gjgtlfrvp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/govebncmy.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gislcmnzg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvzpuzaey.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gmwkgoxrj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gcxibydif.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gajysrauf.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gnlsvkrfq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnqkeapas.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gznvormwb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gyjxdcfbt.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gzzjyhmfq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gejvrypfg.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gwjmxjjts.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/ggxjmbjdu.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gucudadnr.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gdacujgeb.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gmdgksywv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gjnnxjvzh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/ggumfvzzd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gokejrdmb.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gkpgmdjvq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gmrubwkri.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/guaiesbzy.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gtrkmooyv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gcpcsonco.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gqnqajvbq.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gfzuctpor.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gxtrmphtp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gcatadccc.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gwlmrpepo.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gspomtmgi.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/ghxnqzkmq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gnutmlmbd.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gxjtyothe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/grlnyzrfj.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gleilrjmd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkqksyfhn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gvppsxahc.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gyekucocg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gjybalqcf.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gtyryddjz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gsdjqgeml.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gyhrjumgq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gpdjhedfy.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gqecaazuv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gbprlowwg.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gwgxuvbzq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/guwsetbqa.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gbmniqjzy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ginmyqffw.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gdfavqgrt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsxdtigrz.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gszwlqnag.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/geekjyahq.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gruvjaawg.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtxueoftl.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gthdybgpl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gltqzyzqm.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gfloxrcqp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/goxsmmtil.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gpytjvlyd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gmoulaojw.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gikgedjmu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gsrepsqpt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gkqsuuzel.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gpgqsgpks.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gddwaxizy.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gkvejoypm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gtmmjuysm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzucbolmu.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gqlmxwkso.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giygsfbbe.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gbveomlsc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gmxozoosr.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gspvksqvj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gjteksmfo.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gcxgazujf.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gkpuaftkj.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/ggowrtryw.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/geqimgyvm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gfresoufp.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/ghwwcgpjj.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gsvnrajzb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gkjbcrvoe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gbuliicxm.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/grfkrabfz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/ghedyjkxn.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/ggzyfrncv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gxayqsphe.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/grsyissfe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gcqxvvfgu.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gygwdxpxo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/ghiedwxtn.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/ghphlotgo.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gqkjurrqt.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gidowofxx.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gmltiwchb.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/grzpqlflb.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gedmbwcrb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/galpnclmu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gxjazdmug.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gnqsrluhv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gxjzwznno.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gkyrlmcqq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gopuvuvyk.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gbbfpjlvy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gbkvrjxbc.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/ggcyigjxw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gwbxtphso.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gnywfkihk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/goerpwycw.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gfhdqfkut.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gnuqaalce.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gpxwxfefs.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/glwjqkrqr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gwaqnlpmc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gmmvipbor.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gvmijsynm.sHtML


<!-- 参考信息 -->