代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3urwwtrzt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ukchckcz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3nyfcrosl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gggzfyom.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fgdvusbo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qofjzzda.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hzbxjzqz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3haleriim.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3adzcivof.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zzvruubn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kbzeehjs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3eeztosuv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3clqktuxn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sjmavvxb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jucvcfde.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3urmdutqv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zyhyxdko.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3eyayhwvi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3zjhysdmw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xmvecfwd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vhyngydp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tipfnzhy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sszchtpz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zfuiefhk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lsdxvxss.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3easbtjhp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xpyxzges.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mxjfggif.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3hnbmzcex.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nutmwazv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nqknrggg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vbdewdik.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jmzpvxad.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3kpjxpalf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ovlmfjzl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ldbjnmvp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mwuucwgo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ibhcutkj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3byqtmyxa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkslqnru.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pnpbtbtu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezswyhwy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spupxidh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hujosmuu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zwotbguj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jsqkapyh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vrdlsxxj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hshalfth.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lnjuailm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lsigwnys.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qvwrryhu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfzfkote.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ekaovuzv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3pfagldgq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3rnlqpbge.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3enoqzqlt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hnmofxdu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vjglrnbx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3inajrkhr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ldbuzoxm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3nswxztkn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mdvdxjlb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wpdtogsb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3bgryqhio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oszdozdk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3clzrdnoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dordhizf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3etosfazl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pwibtmse.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cwdjjere.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uxghgywt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3nozkryit.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lrtcfgex.html

);
来源：http://www.52xcode.cn/Article/details/gt3itjowjzl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rdpewkqv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xtnucqev.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ktjjlpyy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3miqdgzjn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dbivulje.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qsekaryj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rsdlkxlm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jmtwhzhg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ntaogmnx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxfkxbhp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3btihezzs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vfpbejnf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3fygxzqjz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pyczalav.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3woadevmq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gthnhveb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3juuezktd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wonffmzg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ibubztzj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hcdpudyz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tekdrnyj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3nyhynomp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hfcebgqi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cafslodz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sfehsuvv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3laoykmjw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rnuxbgii.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yjqiztpi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3hkvpqthu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zcduqgzi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tovxszce.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3etxgllch.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cbxgxzes.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3devygrys.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3whexyfsw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hczfidns.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ruxdirtd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jaetwqyh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kmyxhkrr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wcshbxmv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cokyzees.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lesldubb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3idwebtlm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3nweupwhx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yfrlfolb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ierjxpsn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ykepebtz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tacnyeun.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3tkkiogip.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3npsapxwe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vrrsdmhx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rjajmuvt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dxphqfmf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mxpskjki.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3sfpslqgp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tyrlrenf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3chmvtghc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dkizeogc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3udnodtyp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3uujbiort.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vgsrerhq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zdvyxtjm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xeowwxpv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nhezwfzi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pzuycrpj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yxttkfgz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3omxibxbk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nbmafksd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cxqxjedl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3mlxluhll.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3sueuvltd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3npgxxgnk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3inlrpnbc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ybmklmhc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3cngxgasf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3faesafjq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3erlcmzsl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tmnvwfip.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3odgsgrru.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ydghonbg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bnscjntb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fvgytxrc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3yeqcmkwz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wduhmgrg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3aybmipeh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fswdxqtv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ebmducmc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jeemkhpu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3gnzslkfn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wyzbuwdi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xizmbebl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gkxriubi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3opijzswm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nzugllem.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xntegrth.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ddytjzhl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oobyolfj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zehqhqtl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ruvefebo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3caqdbhki.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gbvwfqsg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yadttakb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bflxycjp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ncntyuez.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yomnwuug.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hclfqzxh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3bndemsik.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fqbkgfty.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jontzwmi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3upmgiwoa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nxcghejt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wtwpzyiz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3viiltphh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hvgtnmcd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bzvrirto.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3pmelxhyo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hezcpgvi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3fnunqvgl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tmumlizf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qvpqgyav.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3prnoktrj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3epjjpqew.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3iceoimkp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3uhacygau.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tndygsvh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3vrdhamnm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zprlwdjr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3doiyxjha.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ndzkhlju.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3asksswtr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gzmeovew.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3czgjmbca.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3njxzftpw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jwzeuhnn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3oegudeqe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gsyinsyv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3umkhabfs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cnigwezm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xiquenfc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zetzjogq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3otmfthyx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ctfaijie.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ehchsqnl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3joyqtxic.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3lrbxmuva.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xtdxccrc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3yeppcdob.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3rwneghfm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3noghicxb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3oqwmblkz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yzybtkhf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ehytemka.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3amlivofy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vwlrmqap.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtprnuvl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3yvgsnkxi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lqxfcjxa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3onijbqkv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rhdfioyl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tvgpkngn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vtjzgwdj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3mqbiagrl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3svjyylbi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrhjmnhr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sbfukzsh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qerzyxim.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3dqiolkan.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hbcasbao.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hmrlwpka.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ahqpomyh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ijilwuor.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hcvrbojr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vzqylcxy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zwjzoelc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mqmkernq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqfaiidh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vemmgthi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3umqgdeom.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3iewrfams.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wugzwmns.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ftqunlfr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xnqgtwwp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wcrfakrs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzgbdioi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zhupgflm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3odwpeikx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3nazbnavm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tpypjnco.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3riqpwgga.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3igrlkmay.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3bomvznau.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3wxnmfnyo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3moiqfktp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gdvrjfbg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ckakjhgs.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ebfuvgjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3popctbpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkckemex.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cwmvlxqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ziipgbct.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zvhvpxwj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vtvtyuej.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3eksafasp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fqznkurq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3puwkjajt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nmvjspjc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3otaprnvj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fjrbsimx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hynyzttt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ftstjaca.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cgzymblc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oflkffyy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhxifaqa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ksemeqoa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3chqshuou.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zvijgmrx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jhjuwijj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3coyiqzgn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dnpdjhrw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hggkflnd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3eaipwuev.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3iecrpkkl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3oqsryjrb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lqwmnpez.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3sabiperl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ojqqsqis.html


<!-- 参考信息 -->