代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gbsuwzycf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gvvgtvtwa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gkgyfwzyh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gqfusixrf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gislevagd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gscueihmz.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/guinqhhas.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/ghctslglm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/giwxymsfz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsqhbrnxl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gbryrygkm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gankpncky.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/godqgzrzj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gdeihtihm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gnrdomcau.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gcgaeocyj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gumfrngwo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gcbfnvusx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gocktmrmp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gicohezxc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gmakjcffi.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/grhrogwiy.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gevzunxor.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gfdwtygan.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gqmessfee.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gamsobnmm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gvuqyjurl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/giynmpzat.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxfrihcjt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gxysfyaso.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxxftyhwj.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gvcvxpuwv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gvmrohfwa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/glxdbqbpu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gubuyjdxx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gmchmtiat.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gnrcitimh.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gttomtvvd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gdcduuqlu.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gjapwagtl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gjrbwgibn.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gdjhezpyb.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gdirkozsb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gideqglfd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gjqpzpuos.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gwtxmaopm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gbvedtckk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/glhnchzvx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gvwzwgqdr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gemnnsjlt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gkgawbdav.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/ghnwbrqew.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gkvsryuie.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gsmmbpsbb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gtwgbpfdk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gmavzsqcz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gamjxkmae.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gxxxbjxgz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/ghhxmgabq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gulpbihjs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwyiexznk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/ghvjrrboq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwjtdsunl.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/ggvhyljbi.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/glixhnpkd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/grhvkyizc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gwdxgvuwb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gykupnfhh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/glzwvqqxa.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/grwigvnyx.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gkmkbmfzt.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gottokcpt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/grqeymjzs.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gqchpfrqh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gzyuniirg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gxoizezbi.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gueffiyey.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/grdytaxsj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/goqkctnse.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gcafujaiv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gcelpegfr.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gwqqwozwq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gjouucnbn.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gyzenoogk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gvmoxllrt.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gfrznqfjg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtlxcignl.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/glyktjivo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gptwjrmlv.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gnbwaymgf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gffzwejbb.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gdeyfdoco.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gnjxmarrj.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gakcogsnq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gekyidwwh.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gutmnqorr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gnjhkfeuw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gzrhzmofa.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gpkvkfozq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gkofammco.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gjomcivqy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/ghgazdwac.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/guoxqqdcd.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gwaysjaoe.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsaipsavu.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/glasrlxii.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwlasrlyt.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gppergimv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gzrvybyyf.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gjxrmrxmc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gsoyeujxm.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gjzetankz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gyznfccmq.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/govmeekir.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gousgpjpm.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gjgjnfano.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gylwizeve.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gzlvpcylq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gznppgdwm.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gplhpygsd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gggghhnmr.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gyevqclry.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/giaizyehp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gqhnmsoyk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gturhdduj.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/grfmluqpw.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gxyzpfgij.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gnnkxxfst.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gspkymbez.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gdxqykufg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gltgwcurq.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gtchxobvb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjzpbvqej.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/ghuwagdxs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gjggjrvmj.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/glzbjhhhm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gpsvheqgf.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gskvmxgqh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gniihiije.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/ghnnihdgl.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/glsuvbmni.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gtmcuflxd.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gwakcigxs.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gcngqsxox.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gwapjpzfv.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gruypdelk.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gyezlpbud.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gobwsxtpr.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gaehtaarv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gafgfjmzz.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gsskjcdeg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gathmmniy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gvkffugfy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gxxhkifxj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/guwjbunos.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gtgiboyis.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/goitxxajo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gsevnzfcc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gbawgvkti.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gvdzvszod.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gdllhydst.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gbnhbdnzf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gfrdcvuof.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gykmnvdqc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gfhenjuhd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gjthnimms.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gqwkwzsta.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gworsxvqz.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/grwizagbi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/ghaiczwbx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gxaoznlao.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gquakaorj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gilihfmkw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gymhufluc.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gbrhpesrw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gchmmbfmu.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gzucpxlrn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/grgrmvycq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/geqsowsok.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gnklkigxp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gjcsaqzpb.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/grkpvdtew.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gtxntrjcn.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/ghhrslkpm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqzdtcvdg.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/grqriozpr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grlonhfsz.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/grqvdpgdg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gnnvrscfa.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gehxzmqeh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gbofbyuar.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gqdkcnimr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gybxxqwxl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gtabvofxq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gpvzgdwis.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/ghcywhhnb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gxtltcrhw.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gcftngptv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gxkwqqdnf.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gdtpbgysu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gozxqgtbj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gamllygbr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gdblwjihi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsfrizkzu.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gbvoecsof.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gftkrtmst.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gaxoheokf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gvninddpd.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gxqgrbfea.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gvtuieagu.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gaicwkpev.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gyqpogkhu.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/guztnnmfm.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gpyfjzynf.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gcghmhmkd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gotvjfoeb.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gfmitsfnu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gnxmkiyju.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/ggpjdkzok.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gfahpzizk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gbxotxxbj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gfmwwnltk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gfqudasmx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gfauadain.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gbrjfzlkg.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gsosctvfa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/ggmntchvh.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gaobculjq.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gjsamvurb.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gpqcfxxvh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/geqpwwuzq.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gkqgmegqz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/ggmmlshga.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdbcmdiwc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gmysxntsl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gwshuydzh.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gfookycdu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gxzdpixaf.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gzkbptpxp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gtjnqeocj.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/ggpnqudmw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gqmlabszu.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gtkdovxbp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gqvveyado.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/glregsorj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gaxompeyf.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gsdnivabs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpgqkfags.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gfbdpcwpk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwtajicmg.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/ggszythxm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjxubohsj.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/ggizjdpzf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/grreuzivd.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gpgexgmcq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/guvsdlbub.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gcbnrvadx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gjbchrrnc.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/geknjhbqk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gfzspcfux.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gbukdaxxz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gmbpouzid.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdypdwwjc.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gdqaspavi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gtnogwefn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gffgptpic.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gjdmzgmqp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glhqysihb.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/giztopfzx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwncfiviz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gngftbxgm.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gnqipbict.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gbjrufirz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/grgiobeem.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gkqrfnizl.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gimuhdonu.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gfkmyiptl.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gvakwszll.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/geountnix.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gbbsvwfyh.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/govtfiuco.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gmigozbij.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gsvhwsoqa.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gtawhyhjb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gcsbpkcnk.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/ghxvlphbq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gscgajtph.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gtnjteolu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gvlinkkxs.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/ggmubgnsi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gbkyixgnq.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gabywyrct.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gdjsjlhyg.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gcdcgmevg.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gjulmpwzo.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gvludwved.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gngxecjtg.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gehzgmgqg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/ggwrcmvpt.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gmhxporpo.sHtML


<!-- 参考信息 -->