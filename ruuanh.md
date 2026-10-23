代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qoggzwqx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bopfzaxg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jxwdewmt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pfarbneu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vscacktg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3aqklauee.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sxuhioii.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dpyyjitz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bynvxqfr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ybaubvfq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vrupfvpb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lfhjsuod.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3psrxxmrq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tyapgmpm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lunrhdvr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3cwfflghz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mcavaisa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3itjhbbpu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3pxfmgequ.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yixwhiwy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3czdzjzjy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wrgholaf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qzvwciqh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ylhroqng.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3pskoytux.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ropsoqcv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lrpjyyzk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3plvazgby.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3yeyachvo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ukrcxlld.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cjbbqlex.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hdjpqlrj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ggpsrktn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3wwukypey.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kpdbfwyj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mnjglllz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wcgchyqd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3gnqzpyqb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bpzzklot.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3sqveixvr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mrzwqtrr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3onujpitu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gytebiun.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jlgxmpcm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bjvmsavl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3knopkhgw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3egbwodvz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hlkjpdgb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ijdxshan.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nqnkiwkh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dpphttjh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wrnspwwr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdpawep.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3uvztpsku.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vhqbgjia.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kxktsgep.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3yuwfdxww.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jyapigsn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3egthlqyn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdkzrpav.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3flkjjrga.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yfbzvejq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xfcbikbe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3idalednq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3lfbedfou.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3auugxgba.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3tflhaefx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mhinvmxm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vtkltvwx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kgjtcczn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vehpduyu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gbhxxyan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctxbovtu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jmbkgyls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcjelmjh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cbdsbtyu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fjidmtom.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cesreyhq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qgjzkyqa.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3kpsimgas.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3saolombs.html

);
来源：http://www.52xcode.cn/Article/details/gt3khxndrmn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fpyesuzc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zhbvzabt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hfwnzuyb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rbvbrovw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3obaemmvj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3sfmuzjvo.html

);
来源：http://www.52xcode.cn/Article/details/gt3umjdhpxi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ziaknqll.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3swjbxliz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eelommic.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3virvrivn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yicjfyfh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3sjnctvhb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hgvfmbaj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3equalfno.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ickqzlra.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mizvusma.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mqtxutdb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aezxabaw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3nmhguiaf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yfzenemz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hptvfetu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wtjfatxj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rehynrvb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zijfiylv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3srmyzuuv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xjbiixya.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3saitibph.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ummrzhwm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sihmricf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3notcqbhm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ufkpaoyz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3lkpxwxzn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3suyvmfzh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dvkrjhyd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lhfvczvf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpozgacq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ozmqzhns.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ipxibjcj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3brmfgbza.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3byaomfnz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vswakvuy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hakqndnt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kvtjjjbs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mtflmjqc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hijlsacf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wydmprfp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3johnobqy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wulvptsk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3lavmmzgm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rlvhqiqb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vhnyrevq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezejbgba.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hwoinbst.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ohpondur.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cbavvnmx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ttrpvvih.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3yfmltzyb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dvtdyvft.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3azxldrbx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfkoiati.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jusjuswj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfrggfqf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vihuepqo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kgxtrsvn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hslxjqzn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iulhtagx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uxfzobcd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fcbagjvo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vcuibikl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jvirflgk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3llitxwmh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xjaiqqgh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ptcgzamq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3eerrktwt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oewbmkau.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3edxrbuzr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ekdcqgmo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3isvgtgvm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pbyuxxyx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ysrggaor.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pojypskc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3tjfeqmkd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zntzncls.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3vjiabwgb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mosicyvn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kkbuiabg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wrfvynuy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3bscdarwn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ccddedkf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mwfmpeul.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3krrzcmxa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3izvzkhyn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lbroudpl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wquziflc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zqromosf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wtzflbrr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3lrgoauqb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ftyecjlg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kjfqnaxa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pzhkjkms.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3txmrlaip.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3iviwuyda.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wjbihbqw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sroaivly.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zesedubs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3lcvcbfba.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3uhxzzbru.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sgahourt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wbnguaxl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3drakekln.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3sixgmxfa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bkageeyb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fxqfpdey.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yuqdippp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hpgwqmwn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3azkjvrfe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qfxxiell.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fdlxpdss.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3svekdjne.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3trbivxzr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3bifcuvkp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tuweobpx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3pohlouux.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hmqbqeqe.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3cbzkspwj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vseeqani.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3djmximab.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ugmbsdnr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3erkkeoyb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pvleyiru.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3nufmosru.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lahaauea.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wighgztk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3pqpwuckj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3czyfoayo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3sasmzpqr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3onybnmyw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vivshoqn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cshudian.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3txijwxge.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3iflkcosj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3kskdrpus.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3guocmypz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3uhvjwkwu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3iftmaxwe.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jvrktsdt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mwnvliho.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3brtbzxmr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uuaurnyh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mpijtclb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cpeyaaei.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jwggxqsv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3lqfoynfy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kkebbkjq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hubmxiek.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3kgqublpn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tupsqwxk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lominxah.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lolghsbw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xpasayfp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ijbljfpe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ieskfcrm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3afmbnecj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hbxzxqkj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zcpakjfg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lhairezb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3puwyxuqj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3doanstsl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ydgwuuvs.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3unoctips.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kujthuny.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fqviffbm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hgakilnc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yrdwbcol.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mielhheb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3opsfxniz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qehrktar.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dtnruqda.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zdnqfhgw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ovjtsubf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eeewggxf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ywchtugh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dlwgbbzg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lphwnppx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3epksxakr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3bysajacb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3uchlhlxl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hgdwnugh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bvethsql.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jjcmzdya.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hvbazdzk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fodwkjbz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sdlhqwjh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zzheaglf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qyfyarny.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pbvbmhqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knsfllzj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kkhjegqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lajethsf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ukqscijl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rngtaltk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3lxjylbmp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zeeoyusm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vsmjvukp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dycutkoa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3sjyaldef.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lwxsedze.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3cdvdwncj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3inivmhmk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rjmtzljy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kuuvzvqd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ejzwwxfj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3aiajgvfe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lcaufnlf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lwrejfmn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3hyvkixym.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3riemwlrj.html


<!-- 参考信息 -->