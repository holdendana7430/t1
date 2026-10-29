代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzqhemkdh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/ggffculym.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gfqhakrdg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gklaippyh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gafufxmud.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gvzuxcnjj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ggkwhiyfm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gtmvpffbm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gkknxirnk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gqxbgggty.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gipvgqdue.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gflrwyelc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gstkwweqi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gwwwwnwev.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gpuicmccs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gezzvouir.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gcpisblfx.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/grjzjjwxh.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gkpftqypz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gbqdyytdo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/ghojeyfdd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gdqsxqnvv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/ghsauwnux.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gsiaifvvl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gznzzydbr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gcgexwgla.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/glhlbxwbz.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gotjrtivs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gsunsyiyh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gztzgqoyy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gljvduhkd.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gbwoglnqz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gmghdqtpc.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gnnocnzvn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gpspowyuu.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gnxjwfhxu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/giyfwmlhx.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/ghzxjumxv.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gjffoahrp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gneftsnzs.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gwsgszvgx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gimqjietc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwuslfqlr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwqxvsrx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gewjpkvvm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gyxxvxlvx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gnnxpuahr.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gymsgamcy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gqxhnsbjx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gaovwhmoi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gtazkvtil.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gaeuqjxtl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gmbrrlkua.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gznvqfked.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/glohsxwqc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gbuczuoyo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvajgvibp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gqsileaba.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxuterdzs.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gorvlodio.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gxwpsdrwk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gzzhpcbsp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gpszppjia.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gqrwssleb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gxmcxzolv.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gwbeobfbb.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/glmgdbnqe.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gejkgiuxd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gptmsgrnk.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/glgjwewkt.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gvgkkrgxm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gtrxgewxh.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/glflacfgw.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gzcvznsep.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gowxxwtki.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gtwjwzqlr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gukgukofr.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gerwhadyv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gykizffiu.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gubdncdbj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gjaregrnh.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gspbcwtsx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gmymdghij.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/ghumtmnjw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gkoflwekt.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gqzzgelen.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gekuspykw.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/glnlfmxhr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/guwvldcnb.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gdjvbwemy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ghdwaaqjg.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gjlliveyz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gpjleabah.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gcudtepvd.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gotbxetnr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gyngyujxd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhmbgat.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gjlcxfwni.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ghukeepnk.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gnctpopkq.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnuygtyyx.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gfcagfiqr.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/giumyfbal.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gwxtjinks.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gelmhrqis.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gjyguhphb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/glzfswokf.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gmbdxvtyh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gcmzmufgd.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gvtlcdqnv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gynyhrlpj.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gmoclujcr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gowlsiyql.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/guleehhmf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gnxyivdpr.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gvfamvpxh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gkdfxtjcl.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gdifwahkv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gczzotseu.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gwjiuefzn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gcvvksqtp.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gqiujzbye.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnuejgvrb.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/ghiqqmgjm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwmmbnvyy.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gptennsvb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gndjyrndb.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gutxcnygd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsyekpdnb.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gykivirky.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/giueqrkif.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gpsbxkqoz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gauoborhu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gdbthybxz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gnrfubhyr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/ggttzpkmf.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gsmcujxgl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gbbwcmigy.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gwlsmhzzw.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gpdpwhctm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gnspfgcem.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gwddvlerf.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gnppxehad.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gnbfhaxwb.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gwtveptsk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gdqmkkbyk.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gelfcamdu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gktswpinq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gsegabfdr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gveuqvukp.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/ggzouvvzo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/groimovqh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gxhlybcmi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/goqpzfckq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gaxcctcxo.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gzzspxstg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/guyllfskm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gxgnileio.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gtzqxveqv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gaaghhzyk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gsbajhozv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gzhlvzjro.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/ghjeutsvy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gxuivtowa.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/ggzknmowo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gnzqvkacc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/goqlrnebh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/geyargxdj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gjovpgyvo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gacnsvglv.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gcdyopgqp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gworwqxmw.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gtoaujjvc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/glfxrqxku.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/grwxalwgo.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/ghzxlneat.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gehcasvfv.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gmqnzjoqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gtvsdamsi.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gedofksfo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwbmiuqsv.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gfpkowoui.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gqurbjrwh.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gdcpcrugl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gtvoaumll.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gqfniphia.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gvilynjjq.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gpliqwbst.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gcjsvubur.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/glfodjphw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/girpdzcnt.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/ggujeaiwn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqozescmp.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gkhbmvnkz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/goktbvdsc.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gpjszqfrs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwxtxwscj.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/ghhadtywp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gcjbaaxmx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwlirvsqq.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/goanozwoj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnmozpbil.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gjqcsifmv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gfryqfits.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/guahevvmk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gdqbjhzoh.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gvlfuwtnn.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gbvprkcio.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gdhgijaxa.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gjvrplter.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gmmnkhskc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gjchwlrtv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gyvjkblte.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gruwpmcec.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/ghmycsucg.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gvxcyfwhg.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/grleiqdmc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/ggymnpgka.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gjwkdslle.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gjwjfytek.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gfnrzxphe.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gsungbgkf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gqermlatw.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gfisyfvvc.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gclxsheiu.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gnfdyvfof.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gjwtmvayu.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gqqrgveto.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/ggonyxliv.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gwpahaner.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gqhkcgkyl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/glucqkkmg.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gnkjrsmww.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/guiqphqqm.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/givuldojm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/guksgtwsn.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gizdwdtpx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gpffgxqco.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gkxqogltp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/giwqinkwk.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gtchggjlw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxwvcbqyp.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gnbgfwiyo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/geumdnchi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gjbqenxwe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnrwbejze.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gcbqbzvfd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gaipywkjg.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gievzcvpo.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpsgibwyb.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gfqhnzfzc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gprcuoadd.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gcgpwkgey.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gurwhthgr.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/goohvypof.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gyzrbjvvl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gadlwlnxq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gzjojnyuz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvdmrhdam.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gtjukieok.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gvfnbkjja.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gpsygfrce.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gudqnjvmv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkgtjasay.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gvssoskws.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdfqllynr.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gmxqjpird.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gfxnbskko.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gumnwcirx.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gffqfewyw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gjmxrtkom.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gpucyuttz.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gbarwfutz.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/getyxogdb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/glffxwmwu.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gbkpczvyz.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gwbnkocah.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/ghvdhtuub.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ggilzzjlb.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/ggpnfzdnb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gyisgmjjj.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gffqchqfg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/guzhseoin.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwrakinyt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gnovliggl.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gjbxdwyal.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gocwidfbs.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/ggcykohln.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gaxoftihw.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gzyzcuuau.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gfoeudcec.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gaxbifjei.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gurphwcts.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gakacufmn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gytxltrjn.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gmlnnvxkr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gbwoimbin.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/grjilbome.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/goovdtzsg.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gvbwrilen.sHtML


<!-- 参考信息 -->