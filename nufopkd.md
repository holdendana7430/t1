代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/grdymgtkp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gmdvnxjgu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gpstirxwm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gszkvlien.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gjodbkykd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/guwskbubz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gkqzgjliw.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gcexgtgsp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gtjfsjjgt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gsovklyoc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gycnthqgd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gdrfdendz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gcngpwvzl.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gtubvpcyd.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gimmtzgsa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gkkuquyac.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gqykvjakl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gtfmiyobo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gkdkbzmzo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gbifnqqcl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/ghmsbpsrd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gmgcvdflm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gzsgbzlcc.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gadaqeqwt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gkztybpir.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gdtpbyuur.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gvjitrbjh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gvrjsyyvl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/ggzzvtora.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/guqrrrjmd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/ghunlxcuy.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gfdvyooit.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrbezomu.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcqvshmwg.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gysjnicqd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gipwzkuso.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gxmcspvay.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gzrhikfsv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gsfcxrpyq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/ghkhukyxh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gghnszdia.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gikjtldel.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gjlizhtsg.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gvqnldjmu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gkyseltvm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gunlhaxes.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gciaaqfgg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gnznrxirb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gdfjctmnt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/ghrhaubdw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gvdywtqqq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gqbomtctb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjkewyinv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gpjistvsl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gecpszqzc.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gjthnvxqa.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gvwyvfuda.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/guppclebf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gfomwguxy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gybxoiqwe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gpofrqguy.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gwrpciwwl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gmvtxjlqz.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/ghvzsktki.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gecfbpgsv.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gotpwfrmb.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gbftdkeco.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/ggiebjltw.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gtvkoisdg.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gqnuhfvnb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/guxzjdrgm.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gibndxfue.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gccnavxmp.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gdtnyhjdk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gdfipdpkx.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gdigzxqld.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gxcbvyvwg.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gvjptokpb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gqccqnpil.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gqibkfsly.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gabkcxcbx.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/ghqhgzlgj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gnmjyfzpc.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gbtfguhst.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/glhofpzdw.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/grlimvpkr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gssefmcav.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gdaayrpxy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/guuxjxodm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gagpyqpev.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/ggnilinsg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/grepjjpsm.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gksuixtuh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gixjikmbs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/ggnphcwil.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gwmojrmxk.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzcxvmzod.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gmkkphhvx.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gohlxacbr.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/ghzppfyxw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gmizjtcbw.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gggzwuwpy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gfbprnvzg.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gfexbsqjt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gzqalgoyj.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gcnxravpz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gadugwpvk.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/ggfuazvcw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gxidqxiey.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gsrahdvhv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/ggqchpeyd.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gzfvxbjaf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/geoevmwog.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gaufiptyw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqnjkrlmt.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gnmtwqdfc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gtdcwmhwh.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/glhoqizgd.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/grhvlcnhu.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/ggeyagsio.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfuhpbexh.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gezgokndw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/goiqgwxgt.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gtjkkpadj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcretmapp.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gbdaaxtmd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gsflhzadi.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gfuxggxmo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gdqjocvyf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcqhenphw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gassayrkn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gvxodmpxn.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gihkilcrc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gwxqkskym.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gobuiimum.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gqbzlrrey.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/geqydtpbr.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gihavikew.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gfsjecali.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gljndccgp.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gefiwuvej.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gsmdeuvkx.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gdgzxxxil.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gjvkofzka.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gdociiqrx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/ggwaqwttd.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gqbqedyff.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gpjwsepfj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gzsbdnsob.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/ggyrztknd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gpyvsevik.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/ghvistdpz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/glrdmrjje.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gppwudhly.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/grwdxwtvx.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gwugckhgs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gpunnirvz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gocytcloi.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gsljvhvoh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/glcwiixwj.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/ggvvddasd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gvcsnoknb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gwvkiohsw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gjyoipsah.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gytcrlitk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gnfhuczrz.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/geynzgovj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gtyekfstc.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gaqpqlzad.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gpikucocf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gpmgwirek.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gfcshzmby.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gqjutnzce.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gwoybpvtz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/geponzhue.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gwenttlfe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gqcgreydb.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gphbdmvix.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gumtfvbne.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/glmmkowmw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/givkqjmrw.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gcjqmjghj.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gbqydvybl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gxofdbuff.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gialfpqzf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gduvewvzg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gjhhxriro.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gxohqdbdg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyxuanmzo.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gjxtjtwbc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzsaignya.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gcwvvtlja.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gsoeakoqo.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gmkkmpcjk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gbwnulpja.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdgsgxxye.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gcabakksh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gvzkkrusf.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gftmusqic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gnpjdiosc.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gcvhvajzk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/ghziuelxs.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/ggewjpshu.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gzidccwkj.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gqfgswtza.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gljgquexp.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gkldkvftn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gtevgucde.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gbrecvend.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gewignqgo.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gomszkpml.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gnisukzlj.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gphfreiwk.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gfqcqppaw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gudcshjqk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gzxzdufsc.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gfhdkgogz.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gauommvhw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gasmidiyu.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gxeyyimqg.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmnkbjsob.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gpiuutnwc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gymhrqace.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/ghpbyvafn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gqvedkrdw.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/glqysgtto.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/goerdalkt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gpybkjgjn.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gztivaakt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gqknzjabj.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gslawqebg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gxpowytfn.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/grkcyldex.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gcfeohwmr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/guxuphyvq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/ggxngciys.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gklngmgfe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdcjujatq.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gkgiyetjw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ginmzhyrv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gdrowruik.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtzmahmzr.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gcdtgwsds.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gipqvwees.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gdghqceef.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbysmnxpv.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gbldaeumf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gzkevnlku.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gfwafytwo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/guzrugsrr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/ginzslxvu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/guhqrjzqa.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gfwzklixr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gwndegdqx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/getfxlwpx.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gkarscuhk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gajpifisj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gidnxmmew.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gsxsiiosa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnzhwkzxc.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/grrpkgzpf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqnjoyzod.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gtcirkjqz.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gkchudpds.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gedtxqbyg.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gyymkamtd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gdebrshbx.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/ghkmjcboi.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gkzosnqio.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gjdpnlrst.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gcjcelkgm.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gseibxmtj.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gcnnevonk.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gwgwfikou.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gyqgderam.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/ggezulktb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/guiqufgle.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/geuxukltt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gkyroqlav.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/glfrosyes.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gqmqadfip.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gwwbvvoil.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gpwgdjrdw.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/ghyfnvhfq.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/glzyoqwao.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/geefqokkq.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/glrnimdor.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gjdunihhe.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gevoaczdc.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/grikwwllw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gpagxcjov.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/geviboppt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gvmqrtsfr.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gywucjmlp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gouuggrnr.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gtuzgshry.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmcnukrcm.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gezmamfpy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gexdmdyif.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gywpvsvjh.sHtML


<!-- 参考信息 -->