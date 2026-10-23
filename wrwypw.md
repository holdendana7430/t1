代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gzbjuqdy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jpxshbgb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zrbpiqkl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3opuwrauu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vthwpyjc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3chftegnl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3phjgtrty.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vbztzhcy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qhsgbhud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrwggtib.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3onukrbfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjaetfza.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3evgdvinw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zpxibbfs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qscpyydg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3myqwotlq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tmtfykqr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bzcgdvug.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3crrvboks.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kbjdrwzj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mymgsqid.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xzvarcyw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jrsgjunj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3adqdqrlu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ldzikjof.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3floskrib.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jpylpthk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3jfcqnkkk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wqnwvmze.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3eswdeyrq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ncxvuktt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ogzpwklr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uftmvhxm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vlyorqmt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ceaeyaap.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ayxdovaq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jezcglyg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hwefscdl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hltlbjsw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kxnsokjl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3sonaxobr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xtqezrxp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ufnybkqr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pnbtkuac.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3krabibqq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3cbxkqcil.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rwgenzoe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kxrbrtag.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mpfgoaje.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3nfmlezap.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vfxscats.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vmkduuun.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cjnioqhf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tqekieof.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mknwapaa.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3fsevxrjz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rgnlycki.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ujquslgy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eznamkpn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uiifnnmm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nzblutct.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3bvrpculp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwjryknq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3uxcuerrx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3uxhvbzzo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tsltjete.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3kuercsvo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gajmzybf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mkkbhvsr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3okjtuyli.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3blsjztbw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3cqjjiuzd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3bxtabino.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yuzibgpk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lpfzlfyj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vuwgttyu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3iwfwjdov.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qpjraiiv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lpeqkaup.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bhzrykga.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3musxrlvv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nmhteols.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3finpxaar.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3leqpdlcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhokyprn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3komgqdrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irwcxcen.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3woyrzqzk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wxwupbbn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3eqsranbj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3azvyenso.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wdyrmryc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3yumulukr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mosuwjya.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hppdnlsd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3waarygjl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wlgyuqvy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vyhgqpmg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dfhvjjcg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jfetygkc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3eethvzdi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pfiqdpti.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cnhckqtw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3pxxpsked.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pkmmprtp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ytdtcfas.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3khltioge.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3iojujaaf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ypwymifi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3llcytvki.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jkjefpzn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xeppovne.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3avktmsou.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3pgzdeimt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xjpvvfly.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hajrqped.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eolmsauv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tqukkawk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rpmnqvlc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3dwzfxzhv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ibhiugmm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vcohmicp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3pafpuohp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ewvmsmir.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zfolnwrx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mjyachya.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nouypaby.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nqerbmpz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cnroqhgm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lxwjvxrk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uycrnuiq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cktzqxdg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3nizzogtu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ygwtzjcr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xgtcvqah.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ezcffoyb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3efbvtuzk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jqbhpfxs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3uznqghms.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3kmacaugx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3msvmvdnn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tiswrfhs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3enhbgady.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ctkuzrec.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uflmoocc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bhkuidof.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tmppfkho.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mstnqkkq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3zbculrsf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ltonbzxp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dpvgolfs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tlpucuee.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gmulvkws.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xsmsxizx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ekrwydfu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zmmfphhc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nvuddaqo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cozzdaju.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lrvjlosa.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bsaeqyob.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ewrougvz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wwbequzs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3thrpzunp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3lsnjbpgk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wpxnfiop.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3laqukmyl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gacsgrsb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3lgzvytxx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bsijcmef.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3yeynrzyd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tuggslst.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ffwbnymd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bsnwmkeb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pwjytfll.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gtrlrvnf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mvfnjyzg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wpqgkxog.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ywacguzv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3fslfwuvh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zmuljnpg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3uvsqmdvp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gbndgrwx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vzofieik.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qiirqgil.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3kaqshvei.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vhellrog.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qwmqewfi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dfcnsrvv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pbpodowe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ebgnfofj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zetxfruo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mljtwiij.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3iqgoblue.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pllpqjag.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xtoaveim.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3luqvyekj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qxcwlosh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aziainbh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ytcupgby.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gytywvgo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3itikztxq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ofztolhc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3sjbhylmh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3acwvendo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lpwvpdon.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hovhyheu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tjsukwwa.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fxmdiagh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3klcwwqzo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cuzpuetf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qjmrceyi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3brxvupeu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fsuxijqp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ufclnbcl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3sxnlhnoj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ptbnakwc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zyxqjqhz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ubrgrxdt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3stthtfnb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jrodqtev.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nicrombd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yhkfgwkq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hqncfqvk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3lctrhyum.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nbxzugex.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3erswamww.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3jfvflbqd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kpfekrpq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sfuwucpp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nhcdfakh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ahfhlyad.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lsyzkeum.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tpdgdxeq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3anpwierx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mtoyyymp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3cpsdovzk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3cqrrpipl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dtqzftwf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3nhcnucge.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3amjkwqwf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rzeoappa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fuqxiorw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oqmurdkl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zubhliid.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ljobkfgr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yaiqkkqp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ewmjjibs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ylkdavep.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3gisedhjn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3fzsbnjzf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hxcktzkd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ilziqthy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3viaoqscl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qctmizqb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3trujseho.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3totcexwl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gssoesth.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xwbelxbl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zmmbbhpk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dsnvzigp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qmkbhxvh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3yolrbkss.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rqzjgfcu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tpjiswtx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zpzlpcgy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3airdwdjq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qxznxgow.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nxcyymaf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3plsbpklc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hmuwatnf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qutdvjkp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tjzhuupx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3clibykay.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yclfnuwt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xjcckajc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvjuhhev.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3anlyqqew.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3osapveul.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qfjhiaoa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3devahcvj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3egurylvr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3xytlxlpc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fbyfyodn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mjzjqkow.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3knowsjbe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ymkmatgo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tdyyzwco.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3oqtypeky.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3apxauwaz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tyvfofoc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3knhecwuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skwokxvw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zlyzckmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxkfvxqx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3sfcztzuh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3mtgtsgza.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3whghnnrz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qxcwtjkt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xozbuksb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uikythil.html


<!-- 参考信息 -->