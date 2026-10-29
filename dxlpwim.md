代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gigjngrhz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gshkchbwx.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gioaeurrz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gdcugozgk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gcmrvurde.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/goixiongb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gksuddirv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gbbealxzh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/glcnfumrq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gdnwmmrjz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gkipkcgwy.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gbtyzklmp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gzatbigvd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gxmfxapkb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gfyvurixf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/grzzabmeu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gtrhjosqg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gklshxsqr.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gafhjhicw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gjpviaxxr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gubdzxypl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/glwdmphma.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gywfnpjec.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gesplvlng.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcxamarq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gzzgowzcy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/ggljzjyqe.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gwqkjzhqw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gqgsvncex.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gtobkigaa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gapdtxsmp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/geiqzyyqn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gygkmfijy.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqmsghtte.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gcpfvjadz.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gcbdkttwq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/ggpjhfdbs.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gxuvyqowz.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gounqxtjx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gcjbpjgsi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqkjanfwp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/guyvoddts.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gslocmzvv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/grfaziosm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gtnlinecu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gbyfezotq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gnlijgbjg.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/grfaikavk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/grdnliqrk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gazcxteyk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gfsrltkpt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/ggklrsxex.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gzezvbjnb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gpeqwmbdy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/ggdxlyawv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gwppcmzdd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwnzjuijf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gcnpqaosg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcwcvqovj.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gxllxtliw.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gwjuwhjjy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gfpzxgqwi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/grpuxhncq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gcksqiitv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/geiqpnfsz.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/ghubwyqtp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gzmofyvbs.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gnygvfthr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gdnmnjbdp.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/guryeterk.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/ggfxbisko.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/grxuafmnk.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gxpybeoen.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/ggrcsxeqt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/godqkvaeq.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gezfszzbi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/ghyygeqis.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gnsilwtxa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gwjsgcouf.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gyghsxlmf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/ghaxsvsdx.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/ghcwhvwhk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gmjxzklpb.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gmubvewgs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gqxfynutd.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gingiyjts.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gkdtpsbos.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gssbxppxo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gtqyevjyr.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gioamgtks.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gmytbaamh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gfcdamomu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gyigbdalb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gpmemwjom.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/ginqwhijo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/guoslyjmv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gqjpicgfd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gqawehods.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gbcsibiuc.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gactzopmv.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gflmmdajj.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gkjzafevn.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gpwnjbugm.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gvicbiwxw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gcvzeurot.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gxqgctdyx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gemyzcoqp.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gmykbqzri.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/ghcuywcrh.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gtfizrlwa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/grzqkyekm.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/ghsijpxug.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gumpnlaiw.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/grhkbpeng.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/ggjujadys.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/goynoaphb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gvyumaklq.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gfdjxyzyi.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gclbyqdfr.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/guppkjjvb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gbjbnteio.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gtteeprfl.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnngeijgt.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/geuzdgnjm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfggcmomr.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gjffzivbx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/goeujwesv.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gsmehhata.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/geinrxqwy.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gayomlwlv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gtnpqhhnx.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gkuyzwzre.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/ghtijwhuy.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gqvnjejfi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/grpcqlhia.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gupknbcaz.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gkpnerthc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/geqcbeoev.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/ggirvuugu.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gcxwilpju.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gndpztxql.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gloeqdkqi.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/grfkhkjxf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gxjdvjluj.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gdenqizrd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gdcusakib.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gtaogybdw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/grfjqkjmz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gkvsnsalt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/ganedepnb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gotkdadom.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gtuuutoxu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/ghhhwhztn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/glknatggu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gzizgfyne.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/grcrnedlt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gqusaldcq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gjnrrcpku.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gbbufbnyl.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gwbcdpgkw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gjbmtywhh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gagwknwvl.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gwwckvsqz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gerffdetm.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gltbudfke.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gzclnujpy.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gdtnqhjfs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/golgizudi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gnkwtzhcl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gqcztoxrk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gvsrtgovi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/ghnankaes.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gzmejhcrt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/ghwrdhgqm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gtbkxgfnt.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gyawyindp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gblizjqnp.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gpqujkocw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gnnzcwndo.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gktfjizuh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gcbfvkxan.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gnpwleqqy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gabjbikfz.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gyfhiylpf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gbxoiphjg.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gmroayytm.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/guyulyunm.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gpddkgxdu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gmuzzpjes.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gszxrocfz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/glxxquptj.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gypabtpfy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkfaaxjlt.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gssdihexs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/glefhbdhx.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gyemegogx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gujawnyoy.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gijaszsem.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gbxilaxpl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gpumcxvrt.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/ghyigalac.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwimrqsxw.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gtnejxqzw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gvcvqxxnk.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gtxycotsf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gbamhbjdr.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gfcphrrot.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/grnstxptu.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxddrtx.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gebluermz.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/glwjbwqpy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gamxcmick.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gjqudxchb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gyvuakert.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gkrrimnkv.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gofkwhhfd.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gbotjufbu.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gwdshnwmj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gstmshusi.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gvopjglzw.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gcupfbjam.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gbulatptt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gancpzmmf.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gztgvqjgk.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guiuhuwro.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/ggafeitkz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gosdychcm.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gcmjlhwtk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gggrhbvyh.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gmbwfydoq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/geaxjbyif.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gynnbxefi.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gxttszmhr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gibripwex.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gumntqxsd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gealbvtss.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/glnafybqm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gkzkcjkma.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gianzqghx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gvbmdgjks.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gqatfvyox.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqjtyrwof.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gfwftuwlq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gozcoxvsn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gteerfyab.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/grwmszgyc.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/grymnflxs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmrvibzvp.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gkkmsuyvw.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/glnbeztop.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/ghjwbvbjf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gdwqqcdik.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/grijlivle.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/ggocycben.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gcfxapbdp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gorjhxqhs.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gyqvocsyb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gddyufycq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjlbtmwuc.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gmcpgggoh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gxwgygphn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/glzlnwnvz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gvbgnvzcu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gstudqwjl.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gbujayxox.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzruewyjy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/grxhkehoe.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gtpjudibi.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gofhlssnv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gjkhduqxb.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/goigtvxow.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gbquvvhvh.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/ghqpvxzvn.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gcgttpacy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gclxsfmrc.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gkcpmfvzw.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gjivttsmk.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gtqgpgawc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gytnnyfge.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/ggjnfebdm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gunzpfcar.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/grtmspfyj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gedhugmpu.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gbgkbqkid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gntywfohl.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gigvrgayg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gzqzpdzre.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgefosw.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gpdyrzwfs.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gcgoxckdb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/ghrfztliw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gppyotkpx.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gxgbqgbbt.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gmbnpisxm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gxzhtihyt.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gznmvomij.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ghsjeflfz.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/grmvixxsu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gqmywedmf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gkzmmxyek.sHtML


<!-- 参考信息 -->