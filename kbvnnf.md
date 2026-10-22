代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kqvurhtn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xxgdaecm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2oncjvvog.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddjlsfjs.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2chbsjioi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hczjoepu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2sxohfcju.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mconkpvj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2touxsuym.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lzucbggj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2omttjqse.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zoewjghg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2mzgqwpas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phcdftzh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qssuxmki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwlgkxmr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dswmvnae.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2acklybkv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fdkrcgsu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tlquuiox.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jfnblowp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wcnckklh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kyiajfqq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gjqtzewx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2idalkycu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xyofwlmt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rfwgtfsq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2frojogpw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2smjfggfe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2spottuyk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kfaffyas.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2symdtepy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xrrplmbf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2gykqesgt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dnzqsliv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2kowmjaei.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2utlihkth.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jhgzdmty.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lsbiasbp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pbbgrsrr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2aodwcyzd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fndlhmyv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zwhyabyv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jbbuawrb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ezaisgsx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hfnysqui.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2efvzmngq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dmznwbpi.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ihysuvsw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2sypdzqde.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dovejmrq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nxicxrnz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2aocytlen.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2pmucxsux.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2amablvoi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2poyyrfuf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nlbloctt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2poghngbh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gaajcane.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fqogcugt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2kjoxlqgg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kwtzrrmb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wbvhvdpb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2avjufwpc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xromdzle.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oizkjubp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2euoaptrk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mzcfgkko.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2fsphllcx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ncdtevdf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2spxrubtc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zlykprfy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nicqtwep.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qeoanqgj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wvfcotdr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bnnjiplm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2smufouor.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ctpgjviq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hpvhydrx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qzhpydim.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fsphaggp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cmvlosyh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rmzmlkom.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ffrzgkpx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2iecgbpoe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tnsqdreo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fbhyzhjg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2quqeekdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvoluknk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zqpwvgbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hstkufjb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jgrcwwii.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ugcxlgki.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mxrdjdfv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ighgqtgn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2uxkzsowu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2swgusjxx.html

);
来源：http://www.52xcode.cn/Article/details/gt2knjxseog.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qotgsaov.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2tlqhkaae.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qiuygknx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ouqmjdkm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ljfgbqbh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2isobaxhw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vtaucaxq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2smqmxlve.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qwffjgtd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xupplfco.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2iuorochy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vdewojfo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vhoralsz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2flfwzobs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dxlbrzat.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tclsbyjj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ewxjwavs.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2obqnchhk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rftpzjlv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ldxgrpvx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mwbmabye.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fgyeyxyv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bajqzfou.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mzfdusqj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2agscgjbf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2eknxovwl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pshledpt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2svxrtdxg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2frxwfxli.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tjmbhiaf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zsrklyrf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2prhfvayx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2cvavijwp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wktbdrsb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zusflotk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zzogdeix.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2izhvltgw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kkuiexwz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ijjzezux.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hvrkolus.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jwwbfinf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2awbkwcwd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ufwhxeps.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rbqafaig.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ithafugk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fkmuythg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2utyibymn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2srddswwd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pvcubcth.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gtckkrrb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ntkfxspi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wygkoeuk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xgpcqbik.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2letatffv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lkkwqfnj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jlxfvaew.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ybmybqhc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rdylpelu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wuigxgco.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2cbgzrwlb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2llpztmdt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yqnrbjdz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycyevfii.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2tilicsyk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qqmomihh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bldbidxc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fkdygqzj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bcncmxuu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vmeqjtsa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wjnopexr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nsocvuvy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ljnvweie.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gsmnzmxl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hqysskgp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kolgxtlk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tztkzhmk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gqlpyuxf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lwvigybz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2sokjdqux.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nspjidqk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ghmrmqcj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ybooiozy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2oqigzory.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vfgysyst.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2sbhzpsdn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ythidalr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2hjlllykn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yervybab.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2almlyjap.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hsswuxrr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2dneimxtc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vaywmlgn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fhlaeavz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rjugsvwv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2aauojdzy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wujpseps.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zzeskvdi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lrdroysj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qpuvcfyb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mmyqtbka.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mhsnnlss.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cowsgmon.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2giktfwew.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jbclrloe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wluzirds.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2enxegkmj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dfbbffbb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ufofylnm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rjzgbrun.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2uccgcdyh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2buhidyyn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kcgikqep.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xunbvqsw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gtekgtdd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2dnlhowth.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2isdlbqat.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fdlwwqku.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wojonqki.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gapyubyv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2jinsxlhr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2sijtlqpt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pczqshyp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bkalvzym.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rehlfqtq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rvbyhvdf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hiyhkzaz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dmcnztse.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rvvisfcd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kzjaxdor.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pvkqkpbn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hqnewxge.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tqufxisi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xdlwgute.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xgtcnnoi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gtuxsmcv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dscglnff.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gnhkxksj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvflzz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yaifbqlf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2yjszgweg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2dkpvvqjl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2abnbyqcu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yczonpqg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hkameeis.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ichmhgbe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qinoafbf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2sphyhyxf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2uhgiocte.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2filfbgig.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jrhscnkp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gbyfbovi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hvaepzlq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ubohwyeg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pxbqwztg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ijcspcrm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wnmacdub.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vgbfvyop.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qdjtiyls.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qljjwwpb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ccvnrpay.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vgaiuyzb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2opfuhmgt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hrzoiuna.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gvageqrw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tfiouakc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nxevidfq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2jqbasegh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2amupfpen.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vuhyoico.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2euacdhnm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yxlzsghm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bnvjqjnl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zcmcttns.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2xsqrnmpc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2oserguvu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czbuxook.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfgdytqp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cibrlffk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2nsrvbpto.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jwvnpwop.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bbkevobs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fcigtbjq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gawrjupp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kapyemoo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zjdxaspw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bvdhncms.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mcygbnam.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2lzcrwtaf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2geshumki.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ygrpcgbc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vbmfwqek.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tfkxwatm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ithspqvy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ojeljjje.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zgugkfbq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lbvnijps.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2uhzeljny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2volxgqzt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wrxcapbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqbawjmv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xfucndmj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fswkrrud.html


<!-- 参考信息 -->