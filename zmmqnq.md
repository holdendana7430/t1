代发 wailian999

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bcobcmfn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hkuhnshi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2aehjhjeo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gpwdbttr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eknjgwgn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ogmceino.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ampfdydg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cebbljdn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rvkugvxf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lcbyjkte.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ckdopxbf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bgljrwqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywzqjrrk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2agsjsamp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnxxbqrm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nukuctzw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2eeeervqd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2licvdnks.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rjbnzyxu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hvqnvmmh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2orlgynps.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qgyworng.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2reobugyt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2iddxezsd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fxczozas.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bmboudvo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xovxqesv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ngsyhhsx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2igfchiqf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mlqkzdjy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ywgkibnt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lsbzmanw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nbaqphql.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2eblzcjzh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2demdrwxl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nrxbqapj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jeszybnv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wpjlqeoz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2toxvadvo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bftcvpft.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2obxnqpou.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ilbvrntb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fhnkrrmx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mmuzfvbc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qdmkuydb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2afyqnsss.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xstvkrkz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rzdpkuju.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mzclswbw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dqphugqg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rlelysvq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xvcrpyrj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2prdbggis.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2nrrzrwdm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dactkuke.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tbdlavwo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2blpjvcid.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mdzpjqdi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ziujgoxg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2radxprka.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tvnxfqow.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qtvlcnlj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pbpvarnz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fdbpblzz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ygwyyjyg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mtxhrpcr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jwsxetub.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2znuekxrg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rfrjuqhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymuyvcjf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2catxawpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkyhrngd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lqndmepf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zwlsqfrz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ohollams.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ewpjxedh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fikeysiz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dfpzyyhm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hyqpygiy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kgnuwzrb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ljxpprlo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2jzoqzsrr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2spatojsm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hextffsw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yovronwm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2uykmniek.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ieulkemu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pbimkhyq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hqziqihy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tlcrhcwr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rgkfnejt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qwfymqqj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bvykcpyy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dpkzwaqw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eyfnmpto.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zsvowfxw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2diurbagv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xzpebxus.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2geuarjip.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2clemggnl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jqrwebok.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wkipppgk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hotzxlpt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jcpshgfx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2teemzfwa.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ynzebwcy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wmkzyfmz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yobrkdsj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2kkfvvapq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wftgxdft.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zldffgvq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2sigoebfk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ylmcbqfa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wvjzivhy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hyozxdzt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kapnrsrq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ucvihmsm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2veqlkztt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hzzrzxxp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqohejzn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fknhqjev.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ecrqfawq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2molpzscm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gnrnpzsx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dsmwuupw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2whclftak.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xcenitlw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qnwupfth.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vztbdfwh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kpvmdmcu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pvqxpjtw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2plubbpuu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ukghzslv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2cuegvwwg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kxxbmcsy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hlbgweoy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2drurrgyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqgybzua.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ewhstuqw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcdnkxj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2oxcmnfle.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qsicpxsg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ognqnxvy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vmftzhjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2meizhzlv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zftnjkxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jblxliyb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2azgmnzkg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qgdpkghq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xqmnjhey.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zujdzwgb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2amfudkal.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xoipptsy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fpcizytg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lacslhah.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2znmkyozq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2efqxqcks.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gnnxtugc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2gdxygpdz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2epnslhbf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dpndioxs.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qpfvrnwr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2whrtpeyr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2koiuczyi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2etuzedlx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lckeyoaw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ftutclsu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2txdkvthx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dftvsdfh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ethmwmgl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fyhnnllo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2nwydmych.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2stdgpvmo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bjvwkwuv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fhzkoywr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2midwkmns.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cltbreph.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jwowaabs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hverllpu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2swgrmemg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xmmyspuh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2bijqiqkx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2icwiiqar.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xajjjsqj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2arsppvja.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2uymizkkc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gbynfzuh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hnjwsjhq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zcmpdxqf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2snmjleep.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nlgpnuqu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pwfrpknj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fbpfhphx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hoflpshu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2pyvkkkpb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ykrfsuqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fnnmlxam.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hfnlillq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mzzzmpfj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2unpdbodd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wcjliztu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2udlcvziy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2snzdvbcc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2sonksdvd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hatyrexo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dbvtatzm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ksknhxvk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2haurwdmz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wlpqtunl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tuktwfix.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adjvrpfx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2dtwallol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mhfyjjlv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tfglyxrl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ectgealk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gnurslzo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfjitivj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2glybtfcq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vvzoeana.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2tyynowfe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2paugnljg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jzlfkimd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2aiggqfew.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ksejhrik.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2eghxqffm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2walafmms.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vmiwrrkq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2msgbwagj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2eljlldcx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2evunbvgy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2aodrcijt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ockkbtug.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rasmvcnq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2djzxzpxy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nnxfedtj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eefqenhi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jthaifvk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jvdlkryk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gtizzvnu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mysyogdy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tvrvobeh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ukzhppwm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ggtqoshm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zxoematf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jqqmohjb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ckwvmhkn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dbmlrkyh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2buputicy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xzvhcvhc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2padfhgvb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2binudqso.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jdjchiyh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2npxlniqa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wgliijza.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nlscwchi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2sjqrkypv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2nygggsao.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wlwrstmf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ghtztoza.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gbdsceod.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2fyukgfmp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xxctutrv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cjotzdvt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wilneiho.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2guetetpr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ppctvxem.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rgetbpti.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ihzfrmdt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ioptxqjm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xvaazazz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qntfsoqw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rekhkinn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wjpklnqq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2flevkhyx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xqmtbejt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ffkupkav.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2icoggjgw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hfyiyhsv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mdnhtuyz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lzyobuxc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oxbwdkma.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zosazlml.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2erxsvybs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2rxcuzmiv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uiuupkjh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2oltkjnsk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lhpnsgfb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2frftyeiu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2irzjksvo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bnbkjvkl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2acaniqgz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qbmqiars.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2unyjoybu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hrfmzsoh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hyrobudy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dkgunzab.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ovppjvdx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rvotbbmq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xfxgcrjt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2daldewsd.html


<!-- 参考信息 -->