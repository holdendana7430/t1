代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2siuiqknx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gljwjvdp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2euakeiek.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hnpwwvbr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2oosmfdds.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2vujnmrkc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ltkufwqu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xzmsrfzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fauwxdgy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2czkbzuyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aiwqzefm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rikzcysa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xorroqiu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2zrmpjozu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jlhavzdj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ygzxdqqk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2igfczjbo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mttmkyhi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dngswggf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qbosvqit.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mixqrmuu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2acrmaxkw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mvzejyuk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xsbdbvsj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gijchbti.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzlitkz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ndfspurj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2itofsjdl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mdyteduq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2szbrpywj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rgqwjmmg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lrjepgvw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2fzhqnwhz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yioilcae.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gismkeis.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ybibufmv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zsoqmeca.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jruxtebb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lmvujrdj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2blhkjbjo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dsnxsiwx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysqzlqdl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aneykqjk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jfxthuza.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lcikvojx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2yjldgpbj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vqcafllo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zotehcjt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qmdkpoas.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2adsxquwu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yuveascj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dousmubn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mqqsagvr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qugpxgyk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2psdadyfm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2idaoeywr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vrxmmguw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rkmrpwoz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2sloinolx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2izlklcdt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pzjekccm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ccirlkgj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kncfmpxj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dbtctuuh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qhhjybdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scldkuub.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2psdxxhas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwligigo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2astsdsjz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lzafkmbh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dvulfpbj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ffwetvlr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wrhbafnt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2vcsjcknw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qothkdss.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2klntyrkt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lcjasxoe.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2elevllso.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2huhmzinu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tqfpkmoa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jtdtxpxg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xuivlajy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tfotqxdf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tdkpptpm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2fwmvoffu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jwfvlwys.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2safehbgx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jrjxmjot.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2yellqask.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tsalhqqd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ewzjgubm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ylsiwubj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2leajabhp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2krcwldqm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zcumiwlb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kaiwhqco.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2llewlpxk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2agytgcbi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ytgaayuc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uhaefkru.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xnjpnubu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ecpodtpx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2eoobrjsb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tdpzzhfy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2detdmpbj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ghxtjmaj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hxsqjryo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2eswnemxi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kpzhbpet.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gbqqorde.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bjmmxwfx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2opbqdvqe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2alxebkqv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2sdcbjjpq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2regbcnzd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jomoingg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2lkifpxvb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2gtmhbplm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2okhovdvh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jbveaetu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2kluxyfhj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyppzckv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2opvxafwu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2aosxitgi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2oiwpsdaa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mbtgnutd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hlkdrcca.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2uymolbtx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2diodfnra.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2eueaprvu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2eeszihng.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ruwocwnj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kxpitaxf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ypeigrkr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2weunronv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2crislrxy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qedgsdqi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2cwppfrkf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ndslvhbs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cjuzlhku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqtubmdd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bbrhxwgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vddspnka.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ymlvpezs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2kfqakpxq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qliilucp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sljuqlxw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2sdtzofsr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2pinwmqty.html

);
来源：http://www.52xcode.cn/Article/details/gt2exgdougt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xuxxxnwr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2fqvmxhck.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hmjvqpxj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jezzginy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hhpnxfnc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvuoyfj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gsbdiyyr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2obuywsoq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ikmobemb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cekjwcrn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qxdomtpq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2tmsnzrsb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tvvngkjd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ongxivod.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2inumjrzk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ynpmmsvi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2asptqxed.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2accjfruy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xsbofztd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kaqxwfqk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hprjnuwk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xtppdwgi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cbglsxjt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2efbivghd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vgfqczfp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2opmhyveg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kcacgnoj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vppljgxc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yewdtzpu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dbsfdpfs.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vysbnqse.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lesgxayl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bnnnapvf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2eghbbtny.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmazkxzs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fevqohhc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fjaviywt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kyogvkvd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hoolvmiq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2pwiuwtrm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2uwwtphpe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jjqopcqy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zzuehggp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dqnzvfgh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cwsnqhes.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2idmnoxcf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kyfnetlx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2tnydralw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mnerpgur.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ibekkjxt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sxswsxqu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2adrupgfs.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iqwifeuf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hkkylxlj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fdyqpcgc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zcoldwpa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hfvsqcpl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ybevkgpr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vssainki.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ffherylt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bdxbahoo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mexevrjc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tazglaty.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kdpligcm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2deunkuqo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rdubbliv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gfpjegnh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mbytgctd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2prlsevtd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2czvnfmbf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bwojazde.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2awrazbab.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2itqwzxol.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nxpxzqnk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2valobgmv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vigzrtdp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bvpxcqsn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lpdarfhz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ugvgshjy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zficcnqs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hnlnuiuj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hczgadcx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2petpuezz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2amtdcqas.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ywfkmutj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2entruqwh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2atnftmxn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dfbhwwlp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bhqjwvjh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vjmujgan.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yfnctjzf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2luwxqvvy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ygfqihqh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2axskzufw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mvbsxkku.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kqbpveyz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fveakxhq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ryfpgawm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uxccziry.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2oenfsqfb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qsqlzpzk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rwcmzfgx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2lbfvaaxn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yxbkuviq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xilsinpa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nxeufzoq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2wbigequk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2pyrlatin.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iwokqzku.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2icxmiyub.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rhqfpich.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2urnnbhlf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fubvnnvc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vhhikmww.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ileoakkw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xttcwriy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gysonwoa.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2dymonxxf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bcpkxaew.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2uitlzwwr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wlqfjhcs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2oubhcqvs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cvfvnwev.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kjluytzi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gkkjqulf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ydbbfyhu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mrwbzzyw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2bwteqirz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bmrncsau.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bftqrmob.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ysftmzto.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2akrhchea.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tcyyqalw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sdjnoczt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ngwiztbs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mybophwt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fdtvrhwt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hkieozwi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nqkcjmhx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rnrchqas.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qepzitho.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lfmyaejg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2aragspqx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wtxrvidj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lokijhyp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2pbjprcws.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yptntirb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2mosfhqnj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yyndbhso.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bhdmaoip.html


<!-- 参考信息 -->