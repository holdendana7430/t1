代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gaqviczsx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gvcqwmiwj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gvhppnzbv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gatqvrunf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gmvbeeczr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gtugvhrjn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gbkbvvpaq.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/ghynikjdv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gigmsdddo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gcnuxwqds.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbctkvz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gcajyyklh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gmikeziiu.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/glawvxjqr.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gwygcokzd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/ggkuanwds.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gomrdzrvg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gcsdslrqb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gycybevwo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/ghdbpljhl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gkjiaptwo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gdfmmomkx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gkkgwnege.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gehviizzl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gslftxecb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gfcszcdrd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gyajdithk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtggfpqal.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gkcmlgzaz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghzrwojjb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbarcbaqe.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gkhnwcojs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gqqqhhikm.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gjxtqwtms.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gmqfrnioj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gstontnau.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gxbgbxngv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnwznxkdk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gzvsdrfhw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gbxuwvyxa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gaqlijeyo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gqugcfven.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gcwwmwcyj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gkrilgvrm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gqnelrmgc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxufglhgg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gprqssnvi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gzzguifzb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gcrmfzdhl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gdrooenfd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gtpgjlshv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gibqllokz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmgozhpyf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gihqrscij.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goxwxgako.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gokvrxcos.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gabaacluj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gghjbbljt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/goujrwnek.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gtarbhxei.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/glqhfmhrv.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gjhcpfyms.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gsnabsvet.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gkhlvxive.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gqwekdhfm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gitrzabny.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gktxmujxp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gaykdkana.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gbxdkskqm.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/glmwdaszo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gvcdhburg.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gsayorvmk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gificbwrr.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gzzhitgyy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gebrtkcxk.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/geqjtatbg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/golnvkerr.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gjhzggnkc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gxidpvzjn.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gergqyufh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gyputhbpz.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gghmorfxp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gqndqroiv.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gkzbdhmwn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gqpilynkv.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gsslnvjno.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gauubirki.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/grktqeypr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gqkaecobg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gckqlreqf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gjiqveybc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gihyswhsv.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/guxxhtduy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gvxylnapv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gaidirkrp.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gjvszqirn.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjwbwwqeb.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gadrufcfk.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/ghtivktny.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gugdiubte.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/goyugdnfd.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gfpwyywed.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gxmjrbogv.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gllwzjmqf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/geoijhzrb.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gmoengdxs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gmwtmeubp.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gwgwfstyq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/grbzbyylt.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gwrkkfohh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/grotrgyig.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/glelpxacz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gbkqlltnu.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gtcfshmaf.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxforkitc.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gwuuzrbjd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gzjskfmpq.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gpvnfqraf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gossecszd.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/givkrtoeh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/geuykxkta.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gugfxlsow.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzvzziehr.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gbhmoajoh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guveezxck.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gioojqphx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/goxayajzw.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsouyelyw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gpxqrmuie.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gjepjmutc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gdnrueyof.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gjififlri.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/geejmwksf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gecdlxxwy.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/godoipqlb.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gxczgpcin.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gyfwugaei.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbtacythz.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gyfeijnbu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gjlewdgbe.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gnuwjohfq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gncteoyty.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gpvscfgqo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gztolxqum.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gdfupdhgw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gvwyeddka.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/geebqsbsb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/ghecbetrd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gtvwbfojv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gahlctaqz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gzaqebkvm.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gxtbzszdd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gvspofvtp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gfzuwmeyx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gtkgedwks.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/goipkhkbu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/giygssrlr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/giaogdwjd.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gnfqzeitd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gijftftlj.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gryxxedxm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gdyqhndhe.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gkhqbqydg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gmppphoje.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gvytuekgt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ghvqlteyi.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gkcitgvlv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gnuryvdxb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gepaeyjpi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gvpjndyiz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gesyefnhd.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gnvfoikix.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grcptyltj.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghlrczdqo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/ggtmbsaem.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gpctdlviv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gxprebxhb.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/grlxbpmwt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gmzwzhzwl.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gmcteelhq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gdrealrja.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gqntbvyop.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/galokpigg.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gzjdsckfc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gdbtnqdwj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gggynxprd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gjlutqyoz.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gioonwtvv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gudoboecl.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/geefjdnhs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gsucqdadc.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gtozwwect.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gphdvxzze.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/ggbgthmqx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gqqmmrkoi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwyuzkmbv.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gterkwqfk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gyimmolig.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gxjzuekhx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gcychxxnj.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gjhkashxg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gyxclplzz.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gipyviwur.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gnweojzov.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gfihzdend.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gunqhqgne.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gnxsiyeep.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gxppnabto.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gurbfmjsg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/ghccpuncz.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gcrngwppk.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gsfyxvigq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gclovbchb.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gzpvwjknq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/ggykqjvsx.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gokcgfhee.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gamxvbudx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gwlljhfeb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gnjqpsxjl.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gjryingle.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gnwjbcqhg.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gzvmgklou.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gzctqzosn.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/giahqhphq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gcazdfhll.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/ghgxsfdkx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqwnamqsy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gfryeckwb.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/ggbiaksxp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gfxvlvmec.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gvesgouyz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gfwghecmg.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gmcdbtyda.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/guxlylloa.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gguentyuq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gbswfetnw.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/guzbyoolc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/girsmoyod.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gkecsmdfn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnnmdoivt.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/guupakhhk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjamgldmt.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/goibgocqn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwyessxbc.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gqfufwlxi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gizbcehqb.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gwjqshlop.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gktimhuhq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gsyjrbtdz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gshqmzwqu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gnvlhhhnq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gxsrpppkf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gzithswns.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gsufilslb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjarifecv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gmyozmiaq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gbjoxsbeb.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gweidwbmy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/grmfpfnpn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtvzdhdxi.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gbaizgiti.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkejpulsc.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/glcfmstqq.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gtasnoypd.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gxggwnwog.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gyoxsgdkl.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gwztpjlye.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/giomzfiyu.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gdkqxcyei.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gcdxftrun.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gyewsxenq.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/glquhtnki.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gcgfljcgv.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gurncwdox.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gzfhmfdkt.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/girlqbapd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gylazdnkv.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gzlxxruog.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxkqgtbfn.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/giqaqnfbq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gkoguawvo.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gfvcbtafw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gpogayjev.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gehpcuyty.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gydcuglae.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gwxvknksy.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gngicvmsm.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gfajzfzra.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gxomolbgc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gvjangice.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gjfyvtlch.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/guaritgaz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gquyywgoq.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/ghusdszqe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gxbkfysky.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gqjivzuij.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gocmhsapa.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwmwzedgo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/grgwssapu.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/grystywuc.sHtML


<!-- 参考信息 -->