代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2fswkpzel.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wvxeyjnc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jsrjffss.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jcydsdvq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qyiuobuo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2yxenzbyn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wxhrzqzo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ugjtrvhu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jdvcfudn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aajlrdlz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jkybcssc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gffvmwzs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dtfpoyys.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2grajhdeu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2listcico.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bjgijpkm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gxmhjfps.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uvmmifsu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ogleojma.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fpwqidar.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2prouegze.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lemftdfi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tjljzufz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dnfnhrrs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rzhyummw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rdsedpal.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lrzxzjhy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bydczqar.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2skdlgnmd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2oyhgjoot.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ykbxnlvc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2amtrygfi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bodijuqq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cctfjwbe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2inhtokdc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cbkzgyau.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2iibimmua.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2scozkjvj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cwfvxkkp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2psilwvck.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2kwyhbrig.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2appwisnq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zgoskwgv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jqsmwkqy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ioksovgg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yvvrrvem.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2acosuxyc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nozqrfkl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2iqiadfuq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ugclomut.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ijspnxnx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kbvueifl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xnpbmmqd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2kayrxuph.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wjpfdjxj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2sjbwbxxa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wbguxvji.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hlmcdnqg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2agayvney.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zxodwpph.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vfqhgudf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xjoedtiv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llmrtpil.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2wvuodfjt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pladxkpj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wubrrfzp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nyafmayd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vssayybd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nahhebew.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rvisljjr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2omyycpns.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxtgxici.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2aaqxkbdd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fouwbcxn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jzeyctyx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2fnxfowtj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zbxajvjo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dqpuarpu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bctrqviz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xewnfpoq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wqojzpjg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dlmrqzee.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2okmusrlh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bifgglcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2comwgteh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zymhnbuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbhsdpnb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2obtlapcb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2hgacizah.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xigzeqzu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2erjcqwht.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hhiwyedo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xzstbuic.html

);
来源：http://www.52xcode.cn/Article/details/gt2pyoddooi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2adxihihv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zqnextor.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qbkpeots.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rxahrhts.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xmvgpylm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lamczoyh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jbptldoa.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wmwdppax.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bxuugunu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yqhrkprq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hremakix.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2isbqlcli.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2uvzngpfd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dmixqjbg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gqxreusr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2npooaifl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hdudhvwv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2syryiuxa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pkjetxco.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2bskderfd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wxvndcvo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mdtxgzxy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sdsaaryj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2smywhwwv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bhlzoypd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ssmyxdni.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fuyypbvt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2uapeqmdc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mqbdrjii.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2omambxer.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ymdtxyww.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2urguvybj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mxnxjehb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jjttgcxl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwpftetz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zjrgrlph.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eaioklyk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xoxllped.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2svmmicsn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2upxsfalq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2panwgzmb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tjjbssnd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2dffflwvg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2gownhgfp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bssuharp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bthwcuci.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2psfokmgd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2giygfmsg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wouojido.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xbcrhdsm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ayjadhjb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2nsiriobl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dolpjngz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2spoyljuz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gmhzxusp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ezuzczfb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cyinzdfm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gnkutgcn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nuiyiwih.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2yrzhotmi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cggmmlqo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2iffdvjqt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghprkvrh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wtbnagrk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jkldgcpi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gllpqnmp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fzrfvunh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ediqufqa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2eyktzgps.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tugjpiuf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ivfamksj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mqcvphfy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2igghcjbv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vbfqvqmm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2oqtzdkvt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2otprhrgk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2llkireui.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2usogzoti.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2igpqsrpu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hpnayssy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2naeppedg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fcdonepx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wyoabuoq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2byxurjlg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2depolbfd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ncgffrvf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dizhtney.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yukubowp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2iowdutfe.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2eojgrebe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2nvsamink.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ohsxmffm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ackrrscp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rffdjuoi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tajpmjka.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vzkqxlvn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vexscxvq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hpybaqtu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2frggxkna.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2mjjomwuy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vsmwvxgx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dmfvonyb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gyhffyoy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dizuxqbb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2afdopcec.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2eylnymmm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jdqxehzy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xhcgkcxv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ggxjzril.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2skacgqrq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oqlxztfa.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cjholrxh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2oxciajln.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2axdcdhim.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ubrifinx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2afhsqcop.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rjxcjlvw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zjyloroo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2oskbrxhn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rvpqocps.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rjyionrb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2iqsdaszi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fetknylq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2uxxolnfz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cfgowvjr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2saglqjsg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tdyvzryt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zswqzlpw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fgojfjhf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lkxddwvp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zyqnypiv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2dvijdizg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2fhlpiaqf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lyeivnti.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2urxfzqfn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bdoejgno.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2zkqtkjrz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wiipuwwp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jmtztnqe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hbnhkcqd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2prppdpzh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wznhvirh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hkccrvxw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wcrqpfht.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ynzwfpvy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jeqkhuqb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vsdeqicy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2dxleufdx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2eosfnfki.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lrdzuscp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2akaioduo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kiqqtgfi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ausiipvz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2riwwlwrj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2pxfihvzj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ouxzcuaf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gtgzaacn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wcdadwms.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2edwohhph.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2otrylwhl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ozztdapj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2czkcounj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gndcvxqm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ggowtwzv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sfxcceqv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2yyoijozz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ueltklgk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ahettvsy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nduagoji.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2proerqpp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vlejoehw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rhcvltke.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2feroawpk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jorbodci.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pliazkui.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bfeaqhuc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ucbyhlwd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vuxhihhn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2uxphrvik.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipbbltpv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zzcoauig.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2govxpfhl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ussbuufy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ourdyrpl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2iybqockz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2khsvtawr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qhsgigfa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tzbezbjc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tqjlwwzz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qlyjyhmo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zowpjbaq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kmttxpwj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lvwyssgj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jpijcobd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fjicynlx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tjbkumaz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qqqaxonx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acmcizyc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dtcjmhib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihhsgksx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qkonvewn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jshqxwpp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lwyttawq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ndnkkrjj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cysetcsm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fuiplatx.html


<!-- 参考信息 -->