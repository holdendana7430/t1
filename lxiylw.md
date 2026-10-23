代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3okiybkgr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ofmlvnrg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jittzbtx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rbgqrclr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkakdcpq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3fxxhqerg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wifclmfy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xsexaocb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zvhjxjci.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3cwcymuqk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3momoftkq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kyddhzdc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pvnrqmcg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3sbnyenrj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fhftfwws.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kmwcexjx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3uaravrsy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pyguweaz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dcxbpqwc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bpzftekj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eckvvdbv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3kuhmxehe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kkaroqav.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3yidfcnlj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3zevqrdrx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ryzjzgzy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ifcocncv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kbffhoem.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hnmnaagu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ipqqnbul.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgdiaedm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3llnfellj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nvnhpdux.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jvzemlvn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rdjydyjt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3okcmnhdy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wbmcmumu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nsgdenow.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwurjzvb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3eeutmzph.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pznqqzga.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ikpzlpjj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3tecvfrzg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wxbeahbl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3svhptyqv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3logffojk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lijgtgjh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ciaikrez.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3wbwgkven.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wfjmfmnd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wxodrzlf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hnnkbkta.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3llppbifr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xclcermb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vhndzzba.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hcwqvfdd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uszcauqf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3prldunsj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rvulmtwb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ncsyhdho.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3sgaegpvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhmplzjw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3wnvswyub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxvjnmod.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vjfaanbi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3njichatj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3lbdtgkmx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3obsvtflt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3clzltjjt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3invdmjme.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xvyqwlxm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hnpmnnti.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lvvlcrkn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zplwrmcd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3lyqtycau.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3yszfrqqj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ibinxqps.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3eocbzdek.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dlzcxfqz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3dblydjhd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xuzstieo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ivnlubwg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dzstjpfc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ealyqehp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3swywzktr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3slvkbpjb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3txzzffty.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wsepyfrq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3yrjsqite.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3jicniyyz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3uxltfojw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wdxoxhyf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wbvivvdx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fzamwehm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fkdtwidn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mallhyyr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3oqifcfqf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jgzlneyg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3hjjcjudk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3apguhign.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zbsutmhr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ivmupvrs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wasqkamm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mcaqgjft.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bhzyzrsl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lmwhzrxl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3saovfsyc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tqvhkwdh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mdigsmpj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jzuornxm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nzlglemm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nshufire.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wlkdpacx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ypboqezx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqpzaxiu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hebywqca.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fauofspi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljtebudt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3myjqakzc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3owznrkkl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3icsjljas.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oucbmuax.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ykqqjnih.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dshgrlsb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ybvgzehd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vzkqsjct.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wrywjqzl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3htcpfuyd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3avpzrldi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hnftodhx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3eiewcjow.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yenfubjw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dfjfzsvw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cwgbmdwr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ldaoixtl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zmrmpzwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqyqxwab.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3stflikdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edlakkhl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ccnmshyf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ovuukwwx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3whfojdfv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lqrztjeb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3oqvpcdet.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qcrmsuor.html

);
来源：http://www.52xcode.cn/Article/details/gt3wanqioaz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3aqubaxzn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rvayodlh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nevvhdbo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3azlabfbg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xovpwfik.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3auqyjvnt.html

);
来源：http://www.52xcode.cn/Article/details/gt3trmflvsf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fppzwchp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nngwaeto.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3japqymqt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hfvyvtlw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3mjftrflg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3zozlfziw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fzbipwsm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mxziiffv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fhlzaphv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3onjdklsl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qyaruthe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3snkloilc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xtvqsnil.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ccrtocfn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3amnjaagm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jfpfbwrt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tmyiqfah.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kyemejsb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3avsuviyk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ewejgzki.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3aqlfvtyd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ywjxnwsg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nicvpwko.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gaxrgevy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tgpiubna.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nxwnclwq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3gfarimaz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jlbtumkp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3itkuxsrh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wzcasniu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3yyddrktk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qjbgtiwq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3argrosiv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lpiqbtwl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bxcalyom.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kaxtfslx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3azwqbtip.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3efwespii.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3nqgkkbmg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kvjyzwab.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3swvynhdo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ftobzuxx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3aazbmyfk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3pbhoqazo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bdpjvrok.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3deddhhuo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yyvnbety.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3pmjyuxim.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3haqydoly.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hgssefij.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3prbudfvg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fhoqronf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3thsazrtf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ngreobln.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ycczrcaz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ahksqgky.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3aeuonzaw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ntaswlcn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xktrcwrj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3owhkilad.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irhcxjmn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tdnncnca.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qaecatit.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3eabxftqh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3tmudyppz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xmhctzld.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wobfhxop.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gwpgbewt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pkxqyxpu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ejhpwumo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3phefvmwc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bwsbhqgf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jjxjablf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3toahasmz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3otnijqlg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hflqxbyg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hlgafzxy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3txknbewu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3budzcekz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fehmzfrb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3yrtmsyet.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dnmccvhe.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uaempcpz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3uszepkea.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lbuuvzxg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aejmbghk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dphwieet.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3azlaafyz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uicxaowm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vmovuqfs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rctbagkb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jxhiavtf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dqymrvmg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3iowmynwk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3oevbowlz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hbrcnxzk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mqaiqdir.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zqrdsfvt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qvmzybav.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3widpsybe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qerkaphd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zqnlbdfv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3sxnzgftd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zmifgfwe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3eyyivagi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wfdjlypl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3gxlppisv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jpsmtfmd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mqexawrb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pcmpgwyz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3euoaxfuy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zyfzomev.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vkuqduhi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bmsoobnq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rwvqrtmb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3obnbzyhc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3iunvrgfk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hgahgjst.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3czweutbg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oqflqzvb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wkzifjho.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vyadhwyz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3yozbbmag.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3henkalye.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3uasgxajy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3oaufxvhv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zusfsfnj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3izdjabtz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nejwpndm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wywjrdca.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zkzymexh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hkwstumq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3aspfxytk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3yzaadgwg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3pgvyqjrr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3nbhkxpvf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pvvogdrb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xmgrbtak.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cpegudnb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3efefnzqr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3oqafjdkz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3aaackbrl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3beytbejx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3folofris.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xakyxenn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3musfigwz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bdpgpomi.html


<!-- 参考信息 -->