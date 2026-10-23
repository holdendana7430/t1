代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pmvszwwz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yabqyulv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3eqradrow.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zqjvpymw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gjdpjwzo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3btuypvgb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vqetxqut.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oklaeeye.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qtqtlxmw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3kiddcnaf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zgcuzesm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkjxbygl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wcgnhcjd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3avahxtnw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3spaynmix.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3phngxxcx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rufwpscm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3pqzzxtbd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vgebwrjb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gvcuqubo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gsqtgxhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muctdeap.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjirukbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3havcughb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ceudgetc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qhxitvte.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gwanxomp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kfekojqe.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nqaqtres.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qsyidzfh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3kykcvrmq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3mvjbxtus.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3wzcdlcst.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3naxemvtb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3yxoukdue.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uwsxulbu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tivahhba.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vzsicinv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uudryipn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qvdhqidl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hjgfrbdf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3allvdwio.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3mnthcmin.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xcyxwhxh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3pptthxtr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dpmdigms.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zbtmazvx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3spfjttis.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hosothzf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qrbnhdvo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dxjkatqu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3bbvljxqw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xhrbfdsq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kxympnag.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xgmeheeh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hxavwqij.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ixauhskq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3fzczmytd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xzlacrfj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qiaezard.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rfishlwp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zewrwoeg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xcreuvzp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ftwgvfhg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aiwnqmvb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3oxotyamm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kwwqudsf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xwmmiqvw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3fmqguogd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3eyumcdzt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nbqudeue.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tfqcuutl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nzrdbzus.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjpdgvae.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihqvsvgw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbljaxge.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ibrnymsw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eifsmadh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3wepkpruq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qjluhjdw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3bkdluwkx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ggfckpfw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sycabdwd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3sodesnso.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3huvezosh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wcrlzvjq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3teoesvma.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ssgmuakf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3cyyoyfct.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cxtmdncp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3rekzcogt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdmaipd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ispnrvpu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3nunafjen.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jireezof.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zhcbkiwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpiywblg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vdecsase.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcykuegq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qfqcjtbk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3znlkrhjv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iaivcwpp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xohskwmu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3bpokcldt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3basygldb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3drgvqehi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lbfckzrd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ljmtfnor.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3elbtjehy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ihsusohu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kxxtwhvp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vhhkimiq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yofmbkgt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wawewljg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zcirzkbr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3aqlcydwb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3oawzkpkx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yqsejwts.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vctcjygj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3yxwbocgd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qpgrivbq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3tplrdezq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cuqodvbx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wsdypkrq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3feywlzup.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3oklvqyfm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3khkgusov.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bcihzpgm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nmclcyjs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hxpbdenn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jlyqytml.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qdkjobcv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ivkgtoba.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xzuslqfy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nqltkplb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xmiiobrd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3oerernss.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3gyinyxqn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3rcznuwxi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vmmhcmvv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fjkhodbc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3skiyuzoz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3orwhyfgz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ojdhwbjp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3egkbdbmn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rmqkfdrq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jvzpzvrr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3gdbokrwd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lajpayxg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zmnannru.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zlleokqp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mzfghqnl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ijctnhfa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3dscdchei.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dyhzhqzk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ykmdufae.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3tfdpfdjf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tegzjtyr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ghrpaydd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ptcxjgts.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3zzlcpvfj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3yxesofmp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tolyixju.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3viqfeggb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3acfmcxho.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fbmiwcpn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yefcthab.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hhszuizs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uujuvwvi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3sabvrhat.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gntbxina.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gcqxlznq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qyozcazj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3osroinyp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mlslauzi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3piyiigbr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jdgefepg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xmgqnter.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3legeshpk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3tmchwjso.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mflfljxb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hvtzgydd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3noczmane.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wopridao.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bfaxqatw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3usuummyv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3lndszwbn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wceawkuq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3promhnyl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zsqodzmi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3timdgvfg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gmrlptry.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gdxvzqfy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3bmqzfzsf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3zgwtqlgs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qiittezw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3eebbdocu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xdfmjlcg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3olmsqzcs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3azfsfgom.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3aiulpdhl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3baxlyzci.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3icolopnd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ijyjuakr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zluywndo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pyjudphh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3rnlcsmdg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yamajzgs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3unezpdpk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3asqmdjgs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3plpxarll.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tgomikxc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lszkqqfv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3sktpsvjt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3natkvqod.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3sjxnuryb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sbrjxujd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wtsqebmh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dngasmjw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qvilgocy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bxugxtrf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3enozuukg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bfkoklqu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jufutwta.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bxpahaqd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gdhcgljg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bncgwoxb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kqjfrelb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jwjdhpef.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3sjcfjmvs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cjtwkfzb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3dlrhmwuz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gorbtxct.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3mgguytsa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ixbfevch.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hoxexusx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bcneuxqn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zkhzecvi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3bblodeum.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gtvdkohz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ymhypqoj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jgtvrzus.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3kexarbgm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vzmrpbnv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3puuyclaz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yozjkjcy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qvpulluy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hhoopudc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vgsiygnl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3pysqhzzm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jccbntgl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3yufdxyuj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qasqaiha.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qnunbdsy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3awselqjg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zgdjduxc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3owzvvyyp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3upgmgfsz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xyvejizz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3edxxwdrc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ekxavide.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3rcgamqrg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gvdjdgsk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qdjvpzvp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aszuzvef.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3apnoxyss.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3eykopbjx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3dqgwpkmo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3oqeshtkx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3eqilmzrn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ejcyzkef.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qymfnjny.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bljjlglt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hafflngn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rswaqbaw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vgxhzpjr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bvefghfi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3neqrotjr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kexviuws.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vixkkujf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xgsdhojc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rpscockc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3snsqxvus.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cjihqkbn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cxbjsowx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jqwrzyqt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bbfmbyjl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ssvjvyoy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3tmczkjck.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmrufdyh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qrxyonub.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zjcejxep.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qddhdige.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bnhhdbgh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3imkhmszw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vvihkmkw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3rrkzfhsg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uccgajeb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3guwrajnp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wqxlfkko.html


<!-- 参考信息 -->