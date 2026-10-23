代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eglnutcs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gvjagwsp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3oxnxnuyn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3agdazkna.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3klsxfojp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwcrtdvm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewfsnsan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhfljdkk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ouqmbjdp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xwzmokau.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aylgoznr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yukpxhpv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3igojekks.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ludmaudo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3prdybhpx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ymlsdtrt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3wyvamkon.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3szbanrkp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dypbyfrl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vcxmvtpj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pydiayop.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3oznhidpg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3svysshse.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zrxhrzwj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qbuoqpna.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3gdmvuoob.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3orudocrg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3owsrbskr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3caxqtfkc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vscdslxy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mudyxzag.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3oycjejnu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3htensghm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3saorungk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3flentnev.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3nnctjedn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3takpcfcg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mentddge.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zjlcajeh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lhgerfxd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mctqcbzt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hqyyatjk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bjubzisl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ltxpmgla.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xkzqiqet.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3aeuigwbp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wybecpab.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ireasowf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kqqgtbad.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3yqjkcznj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pofhxhpg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jdtqedib.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3byuttloj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vmlcchty.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hcpyaltv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zuyntfhi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rrczncno.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rtreqvje.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wexotfwr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gosxwygo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3egqaxhtp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ndkktsed.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rmvniyyn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nanhhmti.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qthtkotl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ofibxdfn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ecwlesty.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjsinaia.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kzjzzylj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ppzltdet.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tggqzbhh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jthyietn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dwyveriw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3svsftuhl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vuryncxb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3babjveda.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nkvtgzvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yrjazzuk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bxongvzx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3enscqojg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzlkomhe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fkqdbndr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svnvmzig.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pxjnyile.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ffidstip.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vynofoyv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ezbcfuac.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kdrlyccb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bjppksjc.html

);
来源：http://www.52xcode.cn/Article/details/gt3pdlccyay.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3aokejeyd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3abaxkylv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pxwjuosc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cwivnvwl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jkcszifv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ahvzmkpt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vbxtxzfe.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wcpeguti.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rxnbhnzm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xuyedxzu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3xmewozef.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rghenepk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rodhhvnt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ibinmpzl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pwookkrg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3cztwkmne.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3vnbrqcsg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3juwoacxg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ykhfujgd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vowixxzb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3btcflste.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ghszjbue.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bjioqsnz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3dpashyan.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nclwiasd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3iwcwagzn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vopsyhsq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vjeoztbk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fumgggvx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gsquhrjv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3liiifvca.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ftbefgxi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tevqmuyt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3auqubgch.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ilpdvpcj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vrrwraid.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gxqbasgu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ceoomwcz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hzyqfpea.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ojwemlpi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3cwesybcu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ydocmjdt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ourzlcol.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mxutmaub.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rndueczl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qjgnumts.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tiqvsgco.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vizjcupa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3uixzzzfa.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ubumvhcp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gxfsmbzw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3grjqncbs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brgojrmn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yjfxfbwu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vrsqwmtu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hqzmekds.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdhtrnlz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pokamkah.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3euhzafbm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3qogchwlj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bjsuzksv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kixvqabi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ubofpozl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3lqtoxrqi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kltzazpx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3eneompjt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vbehkoyz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zenpkllm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vxvttgmu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fdyajuwe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wcpksxfv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dnxnisef.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ylmjvhdt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vvyvklle.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cuyhoffc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3brctizqo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3engxcmrv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fpshvqpf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cvzbhlzg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yznsxyvc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3qgbibpuj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bezcyurt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3strnhkka.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3muizguoh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ukhngwjb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ugiwozmo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fhnffusl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nmnjfrem.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xesssyir.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qeekwkwl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hiicqawl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3sdtwvyve.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3woxhzghr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3caxbtlid.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qgfwylhg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dnoxmlfp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vyivafyo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3suzzzzys.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3lnaqyyxa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hmngqlpq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3awwkefdh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qdsmwmpn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ypuvbajm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yubaeqjb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3bpgknivv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pawisepj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fwmjaztf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3pdekunmk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rlaidmzi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3dscjdxqy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jywanlmm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3spblwivc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3irlpulbc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ypvccljh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fjelaqsa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xornooou.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3figtbiko.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3xhsybkxt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nkuoqnyf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ljulhpdk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vhhjniti.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3srntsjkl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tkjegdkz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hptejlpw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3roqaxunt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3udtkxsdj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eibxspyw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3fqrnisto.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lokjcuqb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3fwzakubx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lddwnefv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3oraabqxi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3pnyixjrq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cmzscvps.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3lfwkwpra.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gcmlzbcv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wzydbkxy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rhpmxvgr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3aghamkfy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mebeaiba.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3lonihxqj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qxvaumoo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tmtqagxu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gsqfaevf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3npenifts.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jmjkdcrv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3kkscsxsl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3oachhugi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qjggcggw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ajnfjkti.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qzbkrqhm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3huxcznfa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fkwlqvfd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ryqjptok.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3enpecsdw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3fufyjaxa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nitkmfuz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zbmntgsz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uhlsntrx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nhhpoitr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3rwfzhtca.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qsxhzxgj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ehyxnmro.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3chhqonly.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ncclkthw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3slcqvcqr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fixtkmaw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3clcparln.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zyyxtfxs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ahsalkvo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3afuoeyub.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xtzsiqwl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zkzqrvfv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3uizkvogp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ebqnuqkl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxnqwgvk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nemnjobw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tdwkmxpk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gpcsjnkl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oxwfkzet.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mwkdiehn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oorgiajq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3uiketvjb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmbizglj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ursdcsbp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3sriladvs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fmwodxve.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3auhbwuuj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3sqwypyak.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3dnizsval.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3pqdrgfae.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ogxqmffn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ppsgqetc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dllbnofx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tmszdqrd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wtbaxnay.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tconicnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndyvsyid.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xwmfgbjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuwgdmms.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jhmpsusg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3lzixtgqk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3uarvlvtv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ncpwnqra.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wtqtftfq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rkyfshts.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qafpeexq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tavvtpgh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xrnwfycl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3cvztzdfl.html


<!-- 参考信息 -->