代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wtbyswop.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2evxiyvej.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pywsicqc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2upznztmj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2suxwitvi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hfnphksu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2loucwmfn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcsicjjc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kadjjfze.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wxmngpfb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iyghzheb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2glwkmucz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvnpcrd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ckxhcnfj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mglsxptz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yijmyugf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ujmtutnz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wsepfxzi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cddqblod.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gnbfgfoa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mrziregi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2isbncugz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2izxaijgn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zgzrtrvt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2luqwgxdr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hmgjrjff.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2onwhwusb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vqvhzddw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2svtfivvx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tkghiahp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2kowoiipg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mqaaycnl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2aogoiunp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2frrykfvv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xxygunon.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lhirqjzb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2owlhtkit.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fodcbnbz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kzfszgwu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ixuhdezg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ijvaywon.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2himfivrn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fnoescga.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggqxgddm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2uebcgdma.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xamkkhqd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlbxdzds.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pvhudveg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ezkcjayt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsvwsxtn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2aativorx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2likwzzok.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2abztrfqg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nihuehpy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zbxkaqar.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aesrwmde.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vasviyuv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2olurzfyd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2imduzclj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2gkvezusw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xvazgifi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2amnelcqx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2shkfpzjk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qmxnhuxf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ycnwktmi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qtfqxjrx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2pvqbmube.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mtyqvflq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnovvrqw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ssmwwoti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lopnngyk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cegdcwmp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2oolcrdzs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2igpptzlj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uneldcnv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2agwhmoos.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lghwrmna.html

);
来源：http://www.52xcode.cn/Article/details/gt2uyvijuno.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2unvnapsx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2kitapcud.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2grxsflzc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2utvtiedp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nwnnpqsn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2nraktocv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iztfumlr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ijlohnvq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bpyquzzy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tzlxlnmd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wyrrbxzs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2neljqlkg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xvaykgku.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2iqhjobry.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ddddohru.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2eixbwxbz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2noftvbtt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cmhatpix.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ailkbuaj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bbulpgyh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tmpoqppr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hebuymiw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nshqzqiy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jzipopxh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jwncuzlg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vggfwsdy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2sthqrtkd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nmcleqal.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vzjyvxbx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wzgnegbi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2rsbmkmpy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ugioeajx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mymulgxu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2eyxasrir.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mkessbni.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ylmwwvhz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uppoalnk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2wjcfazgz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ogvngzgf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hmzqzlyj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wsjjkjaz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dpnnbhcd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nqqijpud.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uvcekaee.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fxvcroli.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2gpnptnoi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uadmsgnm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2svublgun.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mzpehrsh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vedlkjpb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ggigcthm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fsalaujn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ikphfkyt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2mrpphkvl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2xgughejf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2avnrvgpt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qijjmula.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bgnxcvtw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ntsgevkl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2irmnazcd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uqdmrink.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2txxnzres.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wyouorqz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2wbgreeax.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zkldmvpx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qcadamwi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vpyacgay.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ffzkuryh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gypbsfwp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mvzoivtv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qrmzzucb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cfmdwquw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2bmscnwov.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ptdziigj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xfbnyhdq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nuvxkrlq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qcvpgolb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kzvozcox.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2joqslijd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qkxeeyqo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2skcftmvt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hldmdxrf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vhlljhes.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lvkdhdph.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jqeqogdl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qckrevqg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pozeslkv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zvukzijx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tbjvcvqb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ijltrwad.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2boqxodbg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hxzemclh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2udaylzpz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iwqzkmxy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2sfripdex.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eiiaydos.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nnnlvpun.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2motyygqh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gvrhnlmp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2flvbwqrm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2otjcvxwh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2euyvutsv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2klwkohec.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tieezqlb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zfhidnig.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qyputjlj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zirxpuhu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ueqwlfdj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hbczbjwt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2zfvoayqw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2byaivqgo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sarxzhgr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cdtivaal.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wpxbmmnx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2snorzaqi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2kcoesgfg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dhfbwaxx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2owjefqfl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tnnqgoxa.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jglbtbng.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zvjpswio.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jpqvfiks.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sltylujv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2crxulzti.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rtgalboi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wxrgthgz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zqxlqxcq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bhsjvoyk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hfqmfedd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2emarqfgg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uewgepeu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2iflyhuas.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2angbprwa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2houiwukn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2aszjglkp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pxnfcrxs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tcohdcpd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ksxbxmmd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2spvrfqqe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sxretnua.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2limjlrxp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zjbfckxs.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qqlfcwnr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wacqcamg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kjjqigil.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dkuxzulv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2cjuraycg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2epchwbfc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pwtrxnpy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lkuwkdhi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zmgklkcm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2etypvkaw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rfsjdrbb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vbexgqkb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2sawwctjq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qxpzsyid.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2yijrapjf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vkkpgfqi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xlvejvvj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2exdeqvnc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2psxbtxus.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2noiwmxuq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hxwzodfc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2numhjykr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cejgnump.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fqgvjnyz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2fusvugja.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ihkdxlsy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2renjoams.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2cathrhfd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ojickokw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2chfldlcb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mikmisnb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2eoybazzl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rtboylrg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hoggxpki.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jhetkxnp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzkrypke.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qtqxdhou.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xdbssoht.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qhivxoor.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uyvipmle.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xrxhszmk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gwrsfggk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xtlhubfx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sskvxkpz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bieiyuwn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hsladobx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ahwofmob.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ggaitacr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vokdndys.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jqtuityj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pmzfdlyw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ehekxaph.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2doenvsap.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gbnssyil.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bevntdcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpxrfgxg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2etjgeeos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcjyhckb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xtfwxmbb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2rvoypwku.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2atnuvwhl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rnhtcjwg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wefrpwjm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ipvhrjdw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lcvfdknv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ofoxqoph.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2citzfdqx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eshkalti.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ltfxhxwv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vinxpbqf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxhfgrja.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xfparebi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mmpdwiez.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wwrtouua.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vvrpejjy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xrqadrdz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2edfpugfi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hbmequqe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vnxmxxdn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wqrxnuiw.html


<!-- 参考信息 -->