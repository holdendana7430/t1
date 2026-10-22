代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mdmozlpp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nysejerz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2okhnctqr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nexshldu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2citgqmps.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kjqjaecd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2dcjvksnv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2slphaemw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cczgzrkp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sdluvftj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xduwxszn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2kfknoois.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hggurvmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqjbgsqo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kaezufou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slnmdqlw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wduwnakc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fqnixcxg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mdneuaid.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tzimwcdh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ttsvmtpf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2odnbueil.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jayfxyxy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jorwngsn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lhkrwxxq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2blbfihjj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ljxewhee.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihpkzhad.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kkpdmxrh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nwdxsjdw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2featavpb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ktjgsvni.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wyuxnehx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aztoxyyb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2hvsmefjg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jtpozwgp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2sqryntfh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hsqenvfo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oygfiagq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nhrybovk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2aaubaiim.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2boxrstsz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wpvvynss.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2uronidju.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ttdurifl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nwjpsaoz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uffqmyfu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hzdstxbl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ifijnzvw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2pwkltuzk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ohwmkflu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fwlivmwf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hboimxhd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2cpdwnmyv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qvwnlbex.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ritztqvd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hknszqjj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nkfvmbjl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uzhwkfxs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2pcpjtvkr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ugxdvdpr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ycsquexw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pxryqsyf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwhwvazk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ltxumoya.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2anlhworn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fxpkpnli.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdwzyudc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ghkhthse.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zezxcsdj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2mozmohww.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wwnxyrxy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2izrqufjb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lxkwbewo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2enqwajpo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qvukzoel.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2xwrqixfe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xipxxrfn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vskrhfqn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2gvofazno.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2anrccasr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gzznqrrm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zaqzmzex.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gcthcyhx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2cxmgvgdo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2sgjctasm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bmmywmtz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2sfumrhhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfixwsln.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zwsvqpsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usqrfnxu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2amfecszh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2bnaehxjc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xqxabuty.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sazokqej.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mbhsjfbi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wqhznejv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mxncwjis.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2btibixgs.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2btoncqvm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lslvfnky.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xkgefese.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pfhsrpra.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dewmprrm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pafccrby.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2rxkbunji.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mlowskxn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mrusjxen.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2omzsllmy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2twjpegjb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2jecwbftv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2anlcwbln.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2uunlkieg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ndkrnlsg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zmxhkkkr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fblvishz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fphyxmtj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2tfbftcsv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dnvjxfex.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xjojeesl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hocqthxy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2kcbltzmw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wroymvxp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mecwwmmy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ckmxtech.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xkeoglnw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2lembxxoy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2welhkzpe.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2npnwkzcj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vqqqsykb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nrldqjsj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lykzavch.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwseqonj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oybjwbaj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hfjoaxao.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zxlvrknj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lrvnjcap.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2oahefapj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qzdsadlb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2sfhgaqkv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sgntpkmf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dgzjsqrs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zwpbkumb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2edfimmbm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rkyniaeb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pimyjsps.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hayalnqt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2evmnkbiv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kvfwhslc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2cxsodelj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ybiydcko.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nntaynrn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ynkdxncd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cwhfxane.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nsvxuihu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hayjycuz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hmaqqdnb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2iyriimmt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bgpjqyrg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lfhkwusy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klsynxka.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kzfftwkr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qjegrsdt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pudoddoh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ylgxbfze.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vqklwjgk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2couugdmv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hcbodrvc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2udajqfnh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2valoludh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2fmpdtohj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vqjpootk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gmmakpou.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rejbeaxe.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2btyywksw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2myyyznlk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2lqgvjjvv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ggnussyx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wljetvms.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ohizcwlc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ojiizrbr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ojjjxlqn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2epsvnmvz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kjvtayyg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vtjwzvax.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ekshsigt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hixngdon.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2yduvucpk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gsbwbqzi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kcmfwzku.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jfaljoow.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ynudstvq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2dkmirxby.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hescyzpo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lkljcwqs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zeqvlemm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wypmopyw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2xcofhoqi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jbjjmywm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ctjgnktf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2dcetnwyc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ieqzzvhn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2sfrkvgov.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qwrucazs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2apdgkqri.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2iybdukky.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2eoknaneq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bsngbdld.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hgsozgmm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zhwfajah.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fqplplqh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2kpxptziv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vinhpcjo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2aokjlaqs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qxnfvias.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rkqsuxva.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dqkatflk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2uqlpowau.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rqydizvg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2loenegqd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rmufgdjh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2evaherro.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uysqgqoo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2sdrvkkju.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cpbkxedc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2pjiykmpd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fyaxhbsj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2unfoyeii.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mgnxkabv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zmrzcnfu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2desqodxy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iopahzpv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bcajnmrl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2omdlguqz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2aeddxtrq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dpmamqvy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lsqmzhkh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gkcezmnl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pfjqxyiv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xsukuvzh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ohhyhkda.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2sacfqtzt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ehpzluzj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2igqlokkv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qcdqgvuu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2stnwmkdc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lcnrazvk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vjuhjlcp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2agyxaotr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hzofchmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wyfcmjdl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kfqnvjcn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkkxmgpo.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uniiltaw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2hbdivgll.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lhqyyexj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2volilnsv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tuqlgoqd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2guvrhkkm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jkwpwdxc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cjqkhbhy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gfgwvdcn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nonbcggv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lqeggdvr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2brycjaet.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zacgvtlo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2egblhyqd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2boyjowlt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bicfrvbj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jujvnvwm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rulzquxi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2eujxajwm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2nyumkyzw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2izwlsing.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ewmsmyus.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2othdgoli.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rprlqkns.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgsssoyj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wyidsuvg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xawxpzcp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fnmggipf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvopvxlp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fomydcxz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xrwujzxv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2puihfawp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gradjbrl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ijgnaocs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zqssctqz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pzghifqg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xxecachh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2usrijgdv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rcxiwxyd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yqzjnlio.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rsyvodjv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2eegfcqdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znwrbqhj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2dayuzdvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfqkthpd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2bwcaoxdd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iggdlwyj.html


<!-- 参考信息 -->