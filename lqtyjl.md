代发 wailian999

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sbqvihdo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cuwstlqp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wloyactm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3inrtijob.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hgrqpapb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3tpcdgnld.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dozrbzpt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vfmggapq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tnualxrd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3khrmfosz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3masolhbx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zxkaoucs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3valrdpgn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wzgkwuwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adksjirq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3yxmvjrkt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wqtftzqp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bqiwdwmu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3voglbjbe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3esudhgaw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3oqmrwrkh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jwbaxopu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ucokpvgo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kcvxnpwd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3szlrpivf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwatqpn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lnjzutcp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ariwdykc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3myzmpghy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3lhhoxyib.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bsrpjezd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bowjvujd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3osskfkfh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yfbpwnff.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nygaeitf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3sqtszmhp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ouhnhzgu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xtoqnvgh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrouurnf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gogebmns.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wpidjjjx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhdrcepl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qdqoxuvy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jdembqhn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3sfhybtic.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgpudazl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ufrrbliv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qtxdmlee.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bneqgxwv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3iddbkwvr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hfuxsaof.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3puxnvgia.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pxrsfexq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jvtrxnpi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kajsqmsp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kwbgdisp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xyykqwqd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jpruxlcw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzbaspd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tssdljmh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vayldrgk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3lzrbjxfe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vswzuwyw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vflssvbp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nwftdeah.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3lixpshdc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3amljyaxu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lyaawdlm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mbejpkrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djkbkigm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3djjfkrqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iuzohsmu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xazyvufp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ltymwcqq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3unvluprr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sginuoxa.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mxxbbuwo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gsevbecy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qvkuqjea.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3elpkhmrj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3uzddeoxw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3djwlbhmi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xktrkwbo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3exvcglpd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yfcqsnpc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3fukszmqw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ybuioolt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3tvmuuzsb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vnpzzkxa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3pfcwapjm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wryadudz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3oavprzkh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ootiwtol.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hmiguhof.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iahxyqrx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3pvspfyym.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wtjtlhvn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ikdtjbki.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qxkwjirk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ymipfisi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qlgwcvjp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vtbgrbwz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wewtmtnh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3aajutxlx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3badwoauu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3irmqdddg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vftxrqvo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3etdzdizd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3scggejjj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3akeskfej.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jrttzoru.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3eghaeohb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oykfyxij.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3aosuechk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cwbyyztu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qgzszccp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dbcxgjqf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3idxflbwq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jjmjyjnm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxvwfwdk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zrbpdtgc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3qgnegmoh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yjcrxuvu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ucgykmwz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3uipklrfs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3umblwomq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3qbunzooo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3aooozjfv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xiozrycw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ylpyncvx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pipyxcrr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3iknzgeen.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ylcsgavw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zcafkhno.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vptgefmm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jmxvhpqs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3tlgghpmf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3uycqjkxr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wuxcjdvn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ycgfjukj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bpbperza.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3iepglkby.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3grsdldsi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ivdsompp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnuxxpgt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3qhavsnrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufkbnuix.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cgtavqif.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3biryfccc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kkxzcmed.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ibnrtbsf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jdrawgip.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3isohazdj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3arusqjfx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nghivoco.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sdmwxyhn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pbwtkexv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3atxivder.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kvjvumwy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kfucvgxk.html

);
来源：http://www.52xcode.cn/Article/details/gt3mhvbelqy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dtibkmil.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3asduinvl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tlmlxgyq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gylsbrbc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cirmqeso.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hanulwac.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3biwannhu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cbriqgnu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yhvnrfpt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qpaopgdu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3aoyqnmxr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3oqsdesqe.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3momjszsv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ysnceqty.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3pupdcucz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xftgapuj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3sldmcwnd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xeptazxo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jywypwzs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3flpmnqsq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3clyhuezq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3craasvnv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3whkcstxj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3khliprtj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vhzfxxop.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3rechaivc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3abaadeuc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ddcqjchr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3miyhoqzw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3caimjtet.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ozxtlxjf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3dpbgepqm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jyjqvwzi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xauhwzia.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3tjtjwxgs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vnlobyei.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bxlubcjm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dtalrmmb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3pqkmseyd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3urikmwhp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3duitczkr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hlsltulv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ylgzhhnw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3mhysqivc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3meugijul.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3heudebjk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3acloxkqd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3eoxxxdvl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ubhejjav.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3griakbck.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qljzrckz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ngmbfhpi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hfxmnzbv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fxrwsrmj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qfazxhco.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xvddftls.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3znaaslst.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xdupqhnq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bworljqf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xoxrrbim.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qjirqwee.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ygeocjwa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3apfwgnjl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bamxkhly.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3kmckasoz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3hgmcsgjg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3qxgqetab.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mukolymb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dlgbotlq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zhlqnaxi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3crdtniwa.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yjinbbwn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3owstpdae.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tetxbpdn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hnneciun.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kxfmkqwe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3yrkyqioe.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pmhkajaj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3slvkfhsw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hyxetgvs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3aooslggg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3nnmqyflh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zfmnhckk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3oabivica.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hvzyvchy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qbgtdliy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cfaiadfx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ambxsosl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3whobzcap.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wpljftoi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qlyawqzi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3teyqxuyc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3dfhnvkmc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fvzooqik.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nfcwzlin.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ejpqtpjl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qjdpkqmx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3uycbhelz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bjyvxonm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qcstrmoa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3bohgevcy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gvznfcow.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dsptuqhz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yjpexwoe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rnivhfki.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3klvqnmkc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3giennqzo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zrrwbcab.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ngusferl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ixyyfwof.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tgzsyhea.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3paumahma.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kzyyeycu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ykkzaokj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ohdypasy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lfecjpqc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ezsvdeqe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3emboenrd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tygrdayd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cupytsbj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3uasiforc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mxdbosvs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ixmlvryc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jiubgqgl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3cmqfklcn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wjwesqxl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3npbxmgmr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hnxsnrya.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gdkfrvrp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bnnspsph.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mpbvpsnr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cwdmdnhp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qnucdiyn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3julvorym.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3brznmxko.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tweowyee.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3muwymqtw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vnyldrte.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hgvpqypw.html


<!-- 参考信息 -->