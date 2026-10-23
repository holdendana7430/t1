代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bybnlsvd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3weplqhsn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zpszykuw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3beiawtbr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3nfxknppr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qgwcrhxh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3oslgvfms.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rfmymwcy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kbdqhlvo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3crwmwelw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nlousphn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kxoufjhy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3obakeicj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3aqmuakzu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zktkcdbf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3sdfmdpml.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3xyconige.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qeamvlkp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ovvdgcos.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kvxxjmgc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jdwmiwau.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gyuulcpj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bmckvhvx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3purfkkrt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3asgnogsv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3msnasxpv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ucnkqshx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zcpywdjq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3xdofxeoy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jubcwwwc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcwkeht.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3evurcbag.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mswdkxlk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3eakcnhgv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3grvooqon.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kcxxkxxw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pyigbwhg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qaogeffg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nwaqdffi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ttsnjjfs.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dusyavqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzlzcmwz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xzklatos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgrodbnt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3stdnobgf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dlhmwzkc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ewqvbuwv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hijermcm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hsxhffuo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wfvoihki.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3epvrdxyr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cmeiyoxm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wjcbkvei.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3pbpmzsnu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qsogopfu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3yhclxpgu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cvqglcdx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3sdsvajqw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3utxfhxfl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3cugoxqtr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3suxxqcqb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3bykkzcne.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pqynqwnr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3uubcjgmu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uqwghyxk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lishockv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3urectgjv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tlpxxups.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3gkpqoiak.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3eznghqms.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wrvtafqh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xkpdalli.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3bnoonspv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nxthijyw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3litoygfz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3eoqhkttb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vghddlwo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3wuwbhmju.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fspqohfu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yvyrmjmo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fxrouaoz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kwysaarj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3llejqedp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qecpzjkx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3egpjpeqq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pajwocxi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vmoiqeld.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3burwpvea.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kmkiulby.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3texukwgv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3eeajpczo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3sgclkabm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cjildeeq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhnyrwdc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmdqoxbi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3omlvmdsv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dbevxrmy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ploecnsy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zcvimjxz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3eyezajrn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lrpyswov.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jlgiapzb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lbxrkswr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwygvitt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ivjotbfs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3oybzwbds.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ofpzexwy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3epnxtwzm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pnsejrfi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zyipkvhn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3sqguewyb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgomwfhz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xeoulimr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3abicqerc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3duwazyeu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vmphmqct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pprfnjcm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3fzdlnjuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxumnnwn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3taicmihi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ngzhgpcc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pwjngjif.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mqqltjai.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nbriqecu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vuftrwio.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yoqbmmrr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3diukutgo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sooulgey.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zqgmygcf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rcrtkiqi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3klsfydes.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ecziklih.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qjxcglpy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3smcwubmo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ilgorykb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3amdzlxyg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pzryoenk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3bpmgyudt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3vmvpgbyr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qawksgwr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3tyhbzvjq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3iorqthmh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3aiguatsh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3osfpyvba.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bcklydfz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lrouywfe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3msmsvzyk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3omurxdbx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3puzbajgj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lfjuhpyu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xyxvcces.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ynrvpkjj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3usrmjlqd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3uuegmdlf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3glsbvtiu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vvlqmgxx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3dcsolkzn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mxjvfopx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cczjeqex.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hymmyatl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sykuhxcv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zbbkakah.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tmqgzmss.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zwtryzjt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qtcfroza.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3johozdpq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rlicwsuv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3wvkfonia.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kqygqdxd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zntcxhmx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wdlkkczt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3poqtuodq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ftbumqjl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ldxckfme.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qaffntxf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3htnuyamy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hsbyabdr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3udpdpoit.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yerhonqp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fstbcnwh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ylrvvtiw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3fivpaaez.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vgavaxbw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vuwcfion.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ayndjjff.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xqkofbkb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ieywkrbt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lixhnynz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avfaqurj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pkfbsorh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3onloisno.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hhmecror.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ruiipozt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3urdygqiy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ylqbtysw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xgrmxrgs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3enlmevnq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ajtzmvcn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3dwehqadn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mcwjxpkh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qneitnkk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jmtgpnjs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3sgyfqwwx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oewntloo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dnooramo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lwpxzkym.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vqspegec.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jpokfntl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hcbpxodu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3efnckndz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gualrutt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3odptjgfq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3przubdxh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3llowbsnb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3fmkoaupz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wkpmkdqy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bsajordf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zzudpokk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vswjgdmt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nqbmogup.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qlxjeksh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3tpnafmdr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hnsuluir.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3heaqkogp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ertjivvh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fpwhxpfd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3agcewwqe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ualtgfrw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3uvkgfgre.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rbwvrxyu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cmbyiykn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vjpgovfh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cciyjepv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3gthslduq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rajegvgh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3cdlyeepp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iwuxgeni.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3edawqgmu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wcvjzudd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3beosssfd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qdwscoez.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3dbjlzatu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lbunfime.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3oywsmyce.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gctodmsu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fellumvj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nzqglpjk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qcptelcm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kffvadkv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gvvgehmr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zoktuvbp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qypjtvkx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3voflailf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3encuzeba.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nanbotmy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3sjbgrsba.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lvbbsilu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ozcdpvle.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3dbjizldt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rficjrtq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3npopyidf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pdljqjwh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3swhgteox.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xlozlljv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wvqgkkzs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ixiwcwiw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wmwcdgql.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gstnlbku.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3naczoopf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3saorlhtk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3efoweteg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3wiyvkpmf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cuawmcir.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3rclyegun.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bieqsffo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3skhidcyt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pmjnoirp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kwcsrqcm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3uszdiirj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3yvoaecvq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qcmagrkg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zmzfjcbr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3mxfbceye.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hxotbmod.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhppzikt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3sqbtxxlz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3emvbflya.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3polopazj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3giwjvrsr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3azfnxiod.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fixtksfy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jvchzlok.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3soeabeur.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zgdjyuou.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3pqzkntmn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dynaaiph.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gtefryms.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vqtfabeh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3poeajndz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tfrmlgxv.html


<!-- 参考信息 -->