代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tqyazqhn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wcfkpxvo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uksivhoy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xalpvdzr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2notdjprw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kyuctxof.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kzgmcafu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wtjwicvo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2cffwfsww.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bgctjfjs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2axrbvpqz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qhiliqmg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdhgkyxe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2amdyzyoe.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2yczsnkza.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hviwfbkn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2uarkrsaw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2uehdwicq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oqycubbn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2bwcycqjg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vlzblmxv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2uzthbdhh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bowvjxxh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xpzjwrqa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2eohtknni.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yfnkganl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2eqntzofw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zlnzicyy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zdjushtu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fiknudta.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ygteknjc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bzldbjvr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uchkqrub.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2csjygoli.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fsmesuvs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dticdyvn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fvnvmamp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2bnmrohhv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ptglefaz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bnsfampv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ytxlipbq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2phctzfbs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2wokdliqc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djudrula.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2nlljppul.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehucojbc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2eujbdpul.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gviejuho.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qkhxdybp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rliaorne.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2oianqqlt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bzgbjcsc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2snllzosj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2harpdnnr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rbehjaao.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkxaaofh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2xqcmwgkq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xxmwbxxx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2hskpglpb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2teahtbez.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kaihfhzp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ookoayxk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zaqlowrl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vkffavyy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jcjtzesc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2txolekcj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2qrcbxkvm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2pgjakglp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgdilhzw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mkemwwku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tozzqrcy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xwefekgu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ubylacst.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bgjfhuyr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ykpfezgg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cgoaszmp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kczowjly.html

);
来源：http://www.52xcode.cn/Article/details/gt2wyueswpe.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2waqkdsyz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wiohgyay.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2idcznlti.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2puqbtico.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2olctszav.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2aljzjlqu.html

);
来源：http://www.52xcode.cn/Article/details/gt2tmwlffjr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2beolxhzd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2rmzdgrog.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rdrwnlkg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hhzixqzs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2znjzcrab.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ptzcgpqe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2uanbtmac.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kkvlihux.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2cuquhcal.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cxkewqkh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hedmfokr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lnnfwqrv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kcyalofo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fdbmzaus.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2dkuwmgjf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xyhpagey.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2basjjnom.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oowuwaww.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bhwfjbee.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2upoglnho.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lsiokeeg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rfpdojyl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kqowaavg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2fvqspxyl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ttueckst.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2norhhcty.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fcjmzwkk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dbsutnce.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nkcgwswl.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2serqlknq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gkaikqwe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mkhiozcq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2thpxynuf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rqwawixu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qrciisjf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ygxtictu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2krkpixvu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mrydfkhf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2iqpczqov.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lvblbxnm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bajasbbc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wxovdibb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rmlpntyc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2eshavfqh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ppqztccc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sqjgfxvr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2mjywoyzk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yswwzhhv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tubveebv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkcgylff.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jpdlfspz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crqkxzfn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ohesgzhp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jogtykxh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bfezllhr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ahfeccvo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2nmvyjugi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eiippnzk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ibjpxexu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fvpsakfx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pwfjczeq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jbycoodq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fboeykca.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kphuibqf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xccqokvq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2nzhtbblb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2swkibvuu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ltzoenhj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2amtdrbly.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2iykdifxr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yjaiuafe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ghlwttsf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fkwfcavt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xffardlt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pplnzyvx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2aibmsvmt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2itdkqthj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2bxvthzuw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pucjsocr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2cnwdwull.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zzcctkgc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2uayglaud.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qbzcmedx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lfowwout.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ehfxdsdq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rilvpppm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vemcsxfk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xwmzritm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ddwodjbg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mdhyxefb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wrhzrsqk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ffyrxlum.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gokmtqul.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jkycivfw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tmjnzlvu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kurwacvk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2msojldce.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zrsxtlgf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2jqcskvub.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bfbujcvg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cglwzioo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ylaxknlr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2kzonmeok.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ngyyvdbn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2gdzdlvnq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cvkoizlp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zxzcycdr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jvwnuyfk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2fbkmykfz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nayrjnhv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vegxvjii.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2oujlutnl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qkwupfag.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2feexksxt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xdtuesbd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vpqlcmgg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lzbwxdyo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2livabgse.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2vndhtajl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wnwtmluu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zttfcsje.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mppnfsff.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2txhomfow.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2znoiktnc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2utjrvhml.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bjyfmqgt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2khpzymrh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xlwqayfo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2alqwngsx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qkexniar.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mxpelrhx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2iwyljsth.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dkgrtwpk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2icggryrw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2vzczpchf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kgpdwtjs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2iocwzeio.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cehzrcsi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lqyjigbb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xvvhjagl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2dkkojpol.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2opfibsaa.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mfkqxzra.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rufyvqqp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2znzyczsl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2mtphnxpd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2hpgkwnzc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xmvbjmox.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2efgjlkju.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2iiujdpbd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bjsiknfx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2howhscta.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2cxcmuqeu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mzqgcfdw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qtpzuatx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2sffhcyac.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hbdboakj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2owyvvelr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2bqitgqcv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qypmwgcz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ixxfhohg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zlarkvnr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2iqbyztnc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sjztowio.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mczlubcr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yyfbdlph.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gulkhgxv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2klrcrqgm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nkmenqnt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kjjugasx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ekphldem.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2anbbstts.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wixtlmqn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pfwasgue.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2owthgltn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2upizqgsg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vcyjwjem.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ebvgclkl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tbcgiztu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zqhfeoim.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tmqsipgd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xbeyjbnr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uabkrrtr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hdhbovmf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2udjqvsap.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xtwpwryo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pnqrymjr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wxufmwle.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mfffvmdu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2rjxcqufi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onxlqupb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xiuxyyyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhcqvzap.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vfpiwnpl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pajnejmm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2itszrygq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iriwkfxg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xtxfmfsp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2afbgyhlg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dkhbhilh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tjwfpopa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ewanvlxp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2agexwomd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2varpsuic.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jojghlwv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2auknlfve.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vphbxkha.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pcmagrmq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ruzxudfa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nvcluqii.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2didloqwc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zjoowltm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mizdgfwe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2idhzkoey.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qcmoovtg.html


<!-- 参考信息 -->