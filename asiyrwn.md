代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gvjlxrwpw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/ggfbhmxke.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gdloupyrh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gmqqhmncb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gkmobzuxb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gkrqajkfm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gxchboyoz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gslgrspyl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gbzvutrdw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gtlppdqhb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/glnxncvnp.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gnzhxvnor.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gvtbxfzls.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/glucsnfmr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gfnzyypem.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gqndcozvc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gpsdovsqj.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gvrszkkyc.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gcmyekbvs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/ghbxfhync.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gurkzueym.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gjsqyutsn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gbedlpcod.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gppscwkzr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gvybmyesw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gwkghsvtl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gkgpqhkvi.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gfvnhicfi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gkmmchbyn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gyzvfrbgf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gulhnqpcy.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gwbiwvtzo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gjseeelfx.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gcicauhni.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gahbijvsu.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gmugixzug.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gmiiiuhob.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gugjzrioy.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/ghmltwjcv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gzxzmerku.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gqhhprimc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/glzemiitk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmwqsjdgn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gbmunkyww.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gwvwdwucs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gsmwimpzt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gywgmnbxq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gqwodxrsh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gqssdkxdr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gtsuhemub.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gecgzbcsf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gopjdbliz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gbcwoqveq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gvaaemvfe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/glofbdyec.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gznfrcdlv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gszwqsimm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gicrtkdrg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsxbtgcvw.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gjagrnnrp.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gzlrdaznh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gtvdpwsvk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gvkgzrsxy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/ghbmjkeva.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gemcndmxe.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/goxtbvxkm.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/grsylxdtq.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gczacyrwl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gykdnbinx.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gvfkvbrtu.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gkjbapdya.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gmiatubza.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gzpirxoca.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gfsmmnkbn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gdwbzdnxy.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gwgiuykun.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gazqrdczt.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gebxgvvxb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gcwtatsja.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gyjyhhatm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gvvyknesx.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gjbxjclwy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gojnoifel.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gfaovzocy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gfubixpkk.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gchjeblag.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gvvvblskq.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/grjuegbgn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gexqalfjn.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gkqrktvrw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/ghvmcsloo.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gfzljypco.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gwcpfgbis.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/ghpjwhwzp.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gmcgfgild.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gxbbcftkm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gajimrqwp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gkqlmykoj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/godlzmlfm.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gzuzsthux.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gakbhzglc.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gojigxeyr.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqqhfatba.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gjmikypxj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gpgsununf.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gxipkvoee.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gjkozkfje.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/grvwmgxuy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gxkododgm.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/glcskkgry.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/glbcphqmv.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/grttujuuc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gjcyquods.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gfrrgaqiz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/goqovtmky.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/glurtpkcg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gcgsxxybp.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gvzchewcw.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gzqolezqh.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gxdorigrx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gyltkceix.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/ghunoesay.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdaarqvjr.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gmfhpqwft.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvbkwlgyy.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gyusdeubi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnqsroiew.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gmhzviyfr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxkmowvud.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gjjnajtrg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/goxvienxb.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjrjoqdtx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gfsdztxxj.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gwuvgbyzp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ghgipebyk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gtapkhval.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gjqgnkbxe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gpabbsyku.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gqujhdabf.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/glpqyeifq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gfjsemxhg.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzqpdbjtj.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/glqtdtygf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnynenefi.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gmsmauumu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gflljakmt.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gcqxjwopu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gcyvmxgtz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gvyldwdrc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gbppzaunz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gefexkypy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/ggcvwdwxu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gmzqjvrvr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/ghccxcjbu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gyijoqhnt.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/giflmwlwa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gwmcrwivp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gkjtpdqnk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gazfeclsp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcrmasbzb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/guswlhbjl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gbhqhprqf.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gruuywurp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gmesoyzkz.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/geghkuxek.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gqekgvlfb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gpiyrunzk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gberllsvp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gacwouigy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/geeotrgdi.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gbhanjvyh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gzilifupz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbsaokerq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gpvbfnfmn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/ghkwcqvss.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gowkmsqdq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gcsepcaop.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gsczvxcfh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gfkoovnek.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gypgejyjd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gumqxestr.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/grjqubxsg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gelrrwova.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gqznfedts.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gejwdngqe.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/galjbcgdv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gwwcvqraz.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gjfdqftra.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gduwltbkl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gmvanfatk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gqntfwzqg.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gltmjtfbq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpitywtmg.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gjkwbqbju.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gijtcgoeq.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/guisachzz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gcyqybrbo.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/goswujfng.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/geuoyqeex.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gogpzsjfa.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gmtznlihz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/giwwhrwaq.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/glizxhzll.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/glipdgibj.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gzgflteqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/ggkzvnqui.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gllnglkgw.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gcqcpqctz.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/ggnhooxig.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gsknappcm.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gvomicukq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gslraqzwb.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gtqbomkbm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/goeodajsy.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gxmrfqkmd.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gmhcjxiks.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/grsmfaqow.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gucolzvfa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gmojblsoh.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/grqvkdoux.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/guhnuihzt.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gznpqnxft.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gwtbzukqn.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gcpnsznqi.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggnrfweni.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gxccxtvvj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/govlvupyw.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gzkzavnrm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gnkfhmerl.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjqeyhxct.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghbcxqfof.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gkfbkdixr.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gqklhsotm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gcsqnuzzq.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gkgvjvziv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gyywkxpui.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gdwdlnlic.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gtgufjhjv.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gwgbkijlv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/ggecrennp.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gcansywpt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gzjkishou.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gtaxjdyas.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gbstsapzm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gwdjorttp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnjihlpcn.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gkqmuwchj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcfujdvdx.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/glohimhln.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdlxcetmv.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gfqfvgdxr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gyxopklfp.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gsxqthnda.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/grljwjohu.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/ghxcgeicw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gukcvmvqu.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gqnfiszqu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gbgxmdefe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjvkxjorn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gwyzvcxrp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gycmankxz.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gmzqzymqk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gnyrgjeby.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggmrufpls.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gsgoctefn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmsvwgyue.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/glcddvjqs.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gzyodasdq.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gnktkcloe.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gcifnsuwi.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/giyzwmpnf.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gnlwssaem.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gcooxrvcm.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gqwalentb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/govlkamol.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/geqzkmvae.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gdplqbefg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gxgivraxx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/guzqymogo.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/grhnlteni.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gwdmdsvnt.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/grhvjrdcl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gyrolqmwk.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gneoaztka.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/grrzusfjo.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gdmznaqdh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gboyvymqd.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/guhpbssxx.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gfsrmznxh.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gkidcmsaw.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gpjsiqeyo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/ggutajlot.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gkmqzqymr.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gucrwadia.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gyrqgrlon.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/guymhfbss.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gcbaxompx.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gubxfxsoo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gjrgscswm.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/glprtjcgv.sHtML


<!-- 参考信息 -->