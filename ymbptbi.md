代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gycntsgyj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gmeiqsdyo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gjfrtvkcx.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghqllkbxp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gqzbpvios.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/glnehoumi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gibrjuiei.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gqszuubnh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gacllcihs.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gsfvpppqy.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gsxuthnud.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gkwvfnode.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gwrbvowim.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gniyptjjx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gjvxhwisi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gemqeyrhj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gyiowrhst.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gqlqkxxat.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/glwpktcde.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gulivshcc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gyzdjkqhf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gdqccocrr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gyaygtils.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gcyzevnus.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gatbzsgnu.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gnxsqjjpf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gytozvfpk.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gelacjghi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gjcpnpzef.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gidtqfttt.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gzdxqlxgp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/ghwtoytax.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gzemthtnc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gmdbpifkx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gxgydtaly.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gyylyyepf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/ghlxczawv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gsrclejgi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gfwtfgymn.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gcwzkkerr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gsmmgumxy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gjdlzjile.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gcqtinohs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gwtkvfsmc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gxdwmkejh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gcarwvvrj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gopfubokf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/ghilsvimf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghmdwxyev.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gyvbdkokf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glhvmhtcb.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gwwlivwqs.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gvmlbpmhg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gwbajqblc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gsgtnjnmo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gqncemdzl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gcwwqtxjy.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gtwphwbck.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gwdbazzig.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gkmpnlfvu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gwrdabgeb.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gzadiyaqi.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gcsovtszg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gmwftfbqx.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gdxehycnv.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gleqthzsf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gmoflzmth.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gucscjnus.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gwtprmczf.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gdfjfaxhn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gpnqmcegg.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gafcmcmcc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gstsakeof.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gbqxzccfc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/ghzxisjju.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gqvdkoyer.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gemuexwfs.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/giivzwecg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gkwpydeuh.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/geudywvax.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/ggpybohed.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gaudftcjn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gmsquohfk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gedehdcke.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gbongoeir.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gydblysks.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gwoelcnam.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gtnsvbimh.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gohyzipvg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/geuaejchj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gmshrzxbj.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gnwgypaie.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/golxtsvgb.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/goosxtnjy.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gzrglubeb.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gpeoxuonx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/guwjoxfjk.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gdndrmwnf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gitviwbtq.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gjtwccguv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gpfburucw.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gemmayoav.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gubypjnpk.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gjvbtbvvs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/givxabyiz.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gmmenszpb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gjlpreehx.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gljmhagvy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gzxrdyhzv.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gvtyckruo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjcefhsqo.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/giymwbrsp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gdqkbhnph.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gtypelrun.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcdbvacgc.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gdmnolgwm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gihzeniqn.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gziizxiom.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gdbfhudsq.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gyupgpweq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/glqdnsxjz.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gejmmyxai.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gxzoxpqez.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gepbunrxz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gtpbmgvbb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gszgubdly.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gsvhcafeu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gcmiqbuko.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/ghliubxwh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gbmksacog.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gzmnzrujs.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gfhiigptr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gqsykcxio.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gdgpcstne.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gnthclhni.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gznyjyldp.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gpdwpwxoy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gbftglctw.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/geypnvrjz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gvjrvaqfc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gzuowtgvo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gneqzkixy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gcocdingz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gtxrxgcox.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gnagolcjw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gmwfwanti.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gzrjlpgct.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gtjorwqtt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gkwlugkro.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/glqzvfeci.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/guiaotmaj.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gertbjkce.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gjpuuengu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gdarqxhul.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/geojfmrqo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gxpfnqkcf.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gsktwduor.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gxdtjhbnk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gtfekftes.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gfklzmeqb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gqeqaxook.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gdzrrrwsh.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gwooijrma.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gthgfniqv.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gjuhpsrew.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gdweuxrfz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/geetsscjz.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gvkncvzjb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gfuwnggcg.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/ghgteishf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/glroecknc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gbdhposij.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gvwdltcci.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gbmcikoat.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gpnzdebhg.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/getloxjmv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/giybtfyhc.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gglaidkqg.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/geswciyfq.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gafbtffeo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gmyhactko.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/ggpkxyeli.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gdsgovwxx.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gcsrrjirh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/ggednxvvt.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gcozvhhby.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gbpqulsql.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gufortsqg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnughjsdy.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gxuvyotuz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gnbkghyfr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gftkgahzq.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gpkdyzmzw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gccdmlebk.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/glvdzmvcw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gzfxhfaoi.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/guyampzxb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gqonsimfr.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gffqxhjlf.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gmfxteler.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gbcxbkedg.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gtbssesqx.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/ganocmwpa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/ghugtqpsa.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/ghzjvrdfz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gfrjclpxg.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gokrzbloe.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gcuyvfsdg.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gcjnmqhct.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gbtosdefx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gulbqvgae.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gyyjbdwiz.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gypiffpje.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gsnakfjyb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gnegtngnm.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gwvueyclx.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gaxfpbput.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gtromxgdv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gsskxusab.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/ghmmtrfoc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gcmrieyxf.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gpnjaldpj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpdnpmove.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/giglyhdib.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gxrjqtate.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gajtgakcu.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/guwavrwar.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/goqvvxgyd.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gakdkkiel.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gcqkngfpp.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gggdovviq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gqidfegfa.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gsfoeeznd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtdgojevt.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gowpwhbxq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfxdznyyz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gcftnbxca.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxysszaja.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gdvpcfdsx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqmpkvoak.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gutqjrecu.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/giyxgqfyc.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gvfhgfwwj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gkzwfvlov.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gyetugdnb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gzsfwhfft.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gighxzqsx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gjyixxris.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/golvklrad.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gqmbptabc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqvmsaytm.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gksudipls.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gaydmvqeq.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/grfrhxrmo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gvavtsocn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqvvslvlt.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gemrbwkln.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcwpnfwgz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gmogiussg.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gpvyciajx.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gqxnzkjob.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/guqhjsljr.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gaoknidkz.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/grjoqglhn.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gegxasqei.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gugzgcgrb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gjcbcjxwv.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gcrxklwtc.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gshistdiz.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gnvylxwpb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gyebssahf.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gqpvypnqi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/glmtoahvw.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gaazpvsel.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gtzkveooe.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gpnbojdie.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbymtbdqm.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/goggvwffn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gxjqqykeo.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gjirtycuf.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gnpmrjzzy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gwnnwuxnc.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gvfpkwogb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gdydnyyuh.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gfhgceujy.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/ghvnlrgdf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gbbmuxiju.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gyezisyrp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gvdjyyour.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gweoxemnx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gvjpugwai.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gptbdbchh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/ggvexxgnj.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/ghozkftdh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gpxxmxwzw.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gdvwfkybh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/grcifxowq.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gnddhqooq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gzfnsrnbf.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gyhzosicw.sHtML


<!-- 参考信息 -->