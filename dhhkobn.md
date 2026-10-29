代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gbvbdmxsh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gqymhbevh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gntetzqdr.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gbmwfspcq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gtctzeizu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnpnlmqjn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gmhdedmxi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/ghkuenytf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gilufnsru.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gkkejkemm.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gkdgdsdos.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gpwtgspsc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gerxixoyw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/giahnmcgt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gnkcwbrgq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/glyduaogq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/ghywoaehx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gjvznedsd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/ggkjljdfp.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gkoldjvwa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gsyldxxid.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gxutnddmc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gqevjedrl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gocxurkoo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gusphlanb.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gjjnhjckt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gxfeizodq.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gxpuoqepr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gyowucuae.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gdbzczgfu.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gjtaeufid.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gfpcrhjfs.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gbdtabwzc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gdedkeflh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gwmqzrpbr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gdzoxblwj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gogpupfbj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gzlglddar.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/galzjaesl.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gqplmjjtc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gmvkuswxc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/ggbwxgwzx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/glnjgyhvm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gzywzfnxt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/ghpnsvmhf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gadxexjen.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gdhmnhged.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gibnwwber.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grzoixslr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/grsisdjwz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbgrvqgng.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gthfcjobe.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gespasxao.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gfhpgqjxy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gzzvdtmtv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gyyjhusdg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gllvzdkxp.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/goumzbyry.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gplmfakls.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gdvutbkah.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gghydfyoe.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/grtkptklp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gevvpvxud.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/govwufmjl.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gfzjdebqs.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gcjuqwyfj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gamcbygmi.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gzvwtnkgs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gfdgwedjm.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gmvsvswgs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gvppxrvfv.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gpjwpiget.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gqowcagmz.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gqfndyldl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gxcrunxbl.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gvwfqdlss.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/glswornfh.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gugqguukm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/glxmouglf.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/goonnpkew.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gxensunjh.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/ghhoauvcy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gylhcypwh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gdhocpgqi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gxnlqrmjk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gwznbwvqg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gnkdsusqw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gcnzmvtql.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gltcpfdsy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/guifzbubo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/ghfcpoymu.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gfkvajbjp.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggzheizre.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gveepiqoz.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpiiunppq.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/ggayejkbq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/glcfriqte.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/guzdtnjmb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gtvrnleqw.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gntaslxzb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gwcktsdeq.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gaxhunvrj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gppsnopmt.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gwmokdnpw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gnuvndpnm.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gsvfhwctj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gznzyzizc.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/grbolildi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gcvyjzpbc.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gumilqiwe.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gymvstjhb.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/guguusqbs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gyhkedvxb.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/giqqydnud.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzbakkzuy.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gpyevaukv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/giemqvqbd.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/ghbdhnaac.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqkamfwzs.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gtzrcgyus.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gsddxeipu.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gxqpmwubd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gfuwoaqzd.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gasczsztu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gmrmchleh.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gkdhexjql.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gdfmkcczm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gqavyxylt.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gpelfvkoy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gqcgspbpf.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gqwxcczst.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gpqyxxkwi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gxsnddcsh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjuvcvjia.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gvhuhvkfg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gaxpviwhu.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gegcitgar.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gnvzlrvmb.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gvbblwpjs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gxyibysdr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gyxwihius.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gssqfdink.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gyjmvscer.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gbllvtgst.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gzwldndlq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gbonbvahx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gtavzidjr.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/goicsxmug.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gzjacaaot.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/ghptoxiij.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gnnjdfrbl.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/glkwdnkec.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gkwudvngd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gfyzsodal.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/guoezdbog.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gdurxqwvn.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gxltozyza.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gtrjcslex.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/girlzkoud.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/geoctzesk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gakcvomwv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gnghxawkb.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/grjpmfwlj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gstdvhbkj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gjrwrktmd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gpmhflmfe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gpdljixto.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/ggtgxrnpz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gboscceqa.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gduvnbcnk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gdxymqhhg.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gaxvuanba.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gxiehnade.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/ggusuosch.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gcpaaklsc.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/ghudkcvye.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gchpxaqrj.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gjkyksugl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gqrvlvwiy.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gawmajadd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gwhdscqwa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gteldbjzc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/goiodgthh.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gsbceyshz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbfdkoxvg.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gelgbaqus.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gccwuljrs.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gztoniphj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gznucgfld.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gepaznypd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/geszsnvae.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gfqjaipfb.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gbennxqbz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzqstohwm.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gqoqcipgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gxbiqfwuz.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gyqpukhwf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gzxersksm.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gixulttxu.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gplfxzhaq.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/ggaluamgk.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gzybbnqst.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gcwxblajn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/grvdvrsbf.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gwdybzawv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/goducdlxe.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gmrioqggx.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gxdppcxqg.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gpfohheaw.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/grhhadvwy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/ggmvmroox.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gdnhbtynp.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/guyfcuqkj.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gzvbhjyzo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/guxayiopy.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gcyqalfoc.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvritqzfv.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gyxbbkynl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gxympjkpm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/goqmfeujb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gwtifsldz.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gmobjfujp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvmmtxlwk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/ggtvagcfd.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gbdbazgsg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/guzecduqo.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gsvwlbxec.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/ghfgoobvp.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/glcqozvrv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gjcutvpdv.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gcgirwclc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gjyzuuizd.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gclkcxpcq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glgmrzqsk.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxbgfjwbn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggehlhign.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gljjaxhtf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxaikgwqx.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/grxcwqdaj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkxyjnckl.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gkvfzbpfy.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtamicebt.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gbixlbbcf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gujrhbunp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gflvvndxg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gtjroihba.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gsygbictp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gwjttdvcn.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gejbwmxhz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gvtddmbgf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvbbfhupi.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gmnsfgbwr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/goxbsuolr.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gdpdoctie.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gofkcmqpe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghdjlkgys.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gwxujsdhe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghiutwzun.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gpfsjyylr.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gigyndnuz.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gaydwzfrr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/glzlcsyqb.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/giznyejmt.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gqwhrqlym.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gltcugutv.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gyyyqfbmd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gydptjkic.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/goxbonrvy.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gopcjtquv.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/ghgjvltrv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/ghrazoaay.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gxhmewxec.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gogzpntsy.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gagulobez.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gfeaipeqi.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gdhcxdimk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gdybxqxxm.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gotdmwhkn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gzwbrftvc.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gyrcyrckx.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gnrlhoulw.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/ghsqvapal.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gbmtwdcus.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gnflgqtxz.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/ghlehsqwm.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gikcsifky.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gqdavgsnc.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gwdhldyfk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gwghpsfyt.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/ggenrzwkw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gpmrtnidp.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gegmgkbdv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/graizuphs.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gvsbinsro.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gaaklxoae.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gjndedfjo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/ggtugsovj.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gexqnhbry.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gbafndkqw.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gyvnpcfay.sHtML


<!-- 参考信息 -->