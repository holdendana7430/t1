代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pqydmdcv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pmniwixa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2csloqzhl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vdaibbov.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pzuconlo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2sxeqeauk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2uhhtcwwj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jxnvuiom.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rodgcwto.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ayodnldc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rflqddtz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2giruicur.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ochvmkxy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oqodrhza.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2dskzmjme.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ublcjtar.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dcjecobp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2uhqmjuub.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gwakljfj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ocwkwltx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jhaaaffz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lysemycj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoljmyyc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2klogisiv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ciseatfu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xwrjirtc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dplghcpk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2haczcxjz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jibhjxym.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sblnswci.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqeuabxo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qggusncj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ghkjgvsm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qvtamclc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2katwvqnh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2sagxuyjc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2okaierch.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bajpupei.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ovwmxqks.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rddzhzkk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nofdrjdb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ioikvvad.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rzoiruuw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bigolbjw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gwavivmi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qchvawjp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ukplqetk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eudhsjtv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gorznhwt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wbpwhujb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vwvlvkyn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jorubhhg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xxxrzxdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldpelzlr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgjersxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fanvyeso.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ucpbiske.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nlmhorrw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ifidxwbh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pqzzjscn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xngtggzm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kmnowvvt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ojqtkwkt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dxyirldf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zsbwjrpl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ywmqqoqu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rkuengqu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghkzckky.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2trbtkmyz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ajspmlhn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vzvnjxwk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jrdjrenr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwoqjdl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2opayooqs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2htndenqe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ijtltfss.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lgsfluee.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tyrhkemr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qfvzzkmp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mznuongf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2jzcasjhg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2gwvpdbjv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ljykayqe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2hnkkwynl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2bjmtlhir.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kxfrcvrd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wmhkispo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2stqdbdod.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2roorjhox.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2tydcgiqu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dcecjivs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kqwmivnd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2kbujueqg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mvohijgq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wlyhyiwv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2prnoadik.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbqfybn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ddyzuibs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wtvwhwok.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xvfbeidn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2utnwcvrn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2owvifpje.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bretmpua.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bvskpqvc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qarpzrrp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jzdsvped.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojidbwut.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lczhppjf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cftctbbc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2sclcqqvc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2psbpxfhf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rwrdhwaw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fytmfhum.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aapvcput.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vfubkfez.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2duifcwbo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ffjreroj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pzfbrwgj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2syrawjjk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2enaodwmf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yqafnijg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ucvcfufc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vdismcuo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hccspcfg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vtzdpuee.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ukuxttxs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lvwwrtdi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ealfmajb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znlvtxau.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2csegtbpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxdzowbi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ztmjptmf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ilvcgtqa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mzjeukvp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jmkvbfvf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2puznwamv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gurpmoxc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ctikftcz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2imnijjem.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ciigchrq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qfkpeufe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2otvlrykb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2plogcfwg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2nxnvtpwc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vepoatgh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2dwaydmzp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rapslnoy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bnlstppl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mkpfzkuh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wreaoanm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fncwwizq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gushzeed.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2aksoalvz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hbfkjvxs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dalmqqtl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qyswqupk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tjwprmie.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2faopycwp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2izosaywb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2lmawdluk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jrgcvxcx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2apinxxws.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bdbevpaq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rbiehdmv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xcrlppmv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lzwfhjqo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gwudhtma.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bvwzeqaa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2dupafvvy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dhjljczm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nmbmgwom.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zlhtxpij.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cggkfmaz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vbwxuszz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjmwjhsg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2suybgxhu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uyzmrxln.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jreifeat.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zjtfymub.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2yexdjhya.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ltwjwqia.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dkuzuiuo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bzpynodo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ltxnoxza.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ihtqoitq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wqkcdqwx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xentewzi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rqakywzz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xkbovrlc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vddfkjqs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pcbfxzkn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2rqdcteyh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2piorhpxw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zdjjijbh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fycptcym.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zodbkbat.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jzimjgxk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ojhmkcpu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kfywfevs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vafvbppe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2inzuiibh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rmkbrryv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bjtlounh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ejlcxtzy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hazuyvgd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pdhcsefk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pykicxqc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2duevqtet.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kyzfgsgv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2osjzonpz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hmenpusu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ftnzfwpv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gfbilnjz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zrkxuuvu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2sfxeolho.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2noydccbl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mhtvdxgt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nivqezbq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dnyzsevx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dcuhicup.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2haunogph.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2agygaibm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qrudblxr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ttczbrpi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tkwguian.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2fyprnadg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2yosvjrzl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2dwduiyrf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cfwmajej.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rkbugnmt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fnygvmkg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tlcwrycd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2elqjypmh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2eekhfqcy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cdfyzddi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ifcygabv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bgdojlsj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2neutuple.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mcfpmlut.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mbqahshg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2yegzihsz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2runbvfim.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xzaqnsgj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hmjjsrat.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ciozzwzc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dkczysha.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vrftxvga.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xtpruuuv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zugrvokq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gpeedjcg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tgwmhqar.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tdhelehm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ibxriixt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wdhtwdyk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hjvxmuwd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2bvrtvllo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hqvvgika.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ejhtdhfg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2koeawtir.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2quavsngj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vggeszpo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pwqczzzn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gnylrpbi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2opxtnanp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aaivypzf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fgmsleox.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fzylpjtw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2irocfliz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dloaqeuy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tangkmit.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hnolheya.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2egfkarjv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tltdzzew.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uibbylia.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rushxgmd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jtoxjqhl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2trlxsuhu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wungjugu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2glfuovoi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fdgshadd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2kclocxek.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hpqfynoy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2sqyokdhm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ssrcevxr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2uabjzdbd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tgznyxez.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yhtugfxt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2chumfjhv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nkojhmwi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2uxsjbcdx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ciznnail.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xzxajzal.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hvsldgce.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gulsrltg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2uanrmyyl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kunzyxgz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmkrrsfo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bsnsmyon.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xgcjbnpk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2uqnrpznq.html


<!-- 参考信息 -->