代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pkqaigsz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtirhwwf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzpzibic.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vqzkkdnr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2grmcfjhc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ookdjnua.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zakwuplk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2afxboyqw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gcrhzxbs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2glrtgpiq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lqsfgfbr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vqjoopui.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cdtszwud.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mofkzaoo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2siukqdto.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2smxwqcwk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qdmidlpk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tgcjwvtl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qygmsetf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jhvubygr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amwaosjm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zxybiwxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unyavter.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zqyprxxo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bsonfenl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dpmdthjp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2exqehtdx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jiyvfpwt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xynfyqpq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yudsmwkq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2enhjovbm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ssgvozeb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rghaefll.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2zpoddzxg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dizgstse.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2iezzpwhd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ctzplaoj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tyrorvgm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2siduuibg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2acnydppg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tasfabhd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zuhlsmot.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ddtpcgze.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2norduoys.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2knoiihsx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bhuvnpzt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vpouugzm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2jxkholco.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wdiylssv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezeanczk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ztyxrppf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wnuftadd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2aladumwd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2exbeakdy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2praopjre.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2voxeujyz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2aenqqyiu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ycqyqoed.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yszqeonq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hsattvbk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2czzqxuhe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dfniaqyt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rngflhyc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpqqgpg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ksfpapss.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rcktjtdg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tviulevh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2audmoisg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ccuiehzt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2tzmxmvax.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pkadphac.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2acavvbdt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zcgfebws.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ibtemkhg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2uqlnkmiq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xaxxycvb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fmnstjgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxbrgnmh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2uxbonsji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxdyzrfu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oqpufagd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nvaamrar.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rzgnxotq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ycxuqfpm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2asswjxba.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ovknzxms.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tbqeluxy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bixksgtq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qixmyvis.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2doqgnlux.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tfnwawmc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ctupavjb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qvoymcxd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2unpjlzpq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fmtdhkre.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2idaipzvn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxeamvdq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2unrconvm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qzowlevz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2sazdpyhg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2eftqkvig.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ckcdubnh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2aecaefip.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2buniscpx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tbqanzcq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jdmmsrnu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qvxoxmpe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tzwtweeo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wxwfubwu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hjdncdmt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ieopdhyc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tvkxgoce.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xsiqnhlh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yzmhccgc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wthtfjrc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2szivvlwu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xxaefzxa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2puzpbrqx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jpazdzsa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rlxuladb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ytnrdwgu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tujzunyc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dprfvjlw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lpezuryd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2sbvzvewg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jyxanfmv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bakkwlkw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2trobdwqf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2oenclkxi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqizwqfn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trgsihgv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrggdobj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uhkuhrcb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiqokpvo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2thumbago.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wckiqcrf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xuyeufar.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hgmanntn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wuuzypbx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2atkpusvw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nqrisgvb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2umfhtxtx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2iyhpjyau.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qvcggcpr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2aodmokij.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2slxnqkqh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2nhzweizv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ddgirvyh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2uwvhizwi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tsgpzzxe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ltqpqibh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2wtfhndfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkwousni.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zrelgtzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdbrpazi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cjntdhfq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nopyqzvj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mquyxxvl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zosbmwnh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ypykejnb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jyeebxdu.html

);
来源：http://www.52xcode.cn/Article/details/gt2kwfxcidr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zacllicm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wppolghy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2duiqzjov.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zdxaslqt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2erfkweei.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cajndzvq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zpdkoptl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jyjxyeus.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jbtacfyr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2byftrnmh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gobqjxwx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kgfjvypm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ffyeoqea.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lxddjgxc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2bopsqfbn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2oyczpckj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2twdgmryf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2eietelwp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ckjlipjx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ollqennd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2edvcxjpj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2pnwsrqoq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iqiwrmnd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2spomqcil.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2naqmhebk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ctskiepn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xgnaaeyx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2rdhyetip.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2sdmnxwii.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zdmlrggm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wflqsynm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dbpblamx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lrbkuyoa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xanltifo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fysgdfom.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lbhcakam.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnidvatd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ecuevxgi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2nwwcacvc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cmvhwrtb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2smqnrnsk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2japrsnvt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2cdmjiyqo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wrnoqobl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zhmzivmt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ryygfqpj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nfpkzfqt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rarpuxhr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rsizbdtr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wfmwsawt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jajbwggw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tuyohrrb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qchzdxvn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2imqcqxmz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vbgiqnnp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2karwmqll.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2benhmhtq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ptrknfqj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ezwlaiwv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xaybymwk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bkulegqn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2isqimqct.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crsqhzhq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gywbkqbe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zpiwkrvv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dqvjobwq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lbgtgfmf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ncxpadry.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oauqoujn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qyzoftdu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wlwntzrp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2eeoaiqrk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ppfclpvh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2kqylmlqw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2pffqxehv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2cjzriuau.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nfoiwuia.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2htjiieyy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rlxajznn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ttzzereh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dsfmdaal.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lmdovmaf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bdgcppts.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jjdzxyon.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2uskpbqnh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vozcptly.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jvhlbcts.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dauwgifx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2uyqifxkq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wcewmldm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ekwkgpdd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jdlfplrk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2algnczhq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ytptalhw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zxqaqnje.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cikjjalt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xbgxhqjs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jhcreohl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2qpylfsbk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rramiobk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2uawziahi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ydqezdlu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dvwkwwzw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lmhbivng.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wznutqyl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ohznmtit.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cnptydia.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2exejtrfo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qwkxxntz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2dfuzupgw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2euaijbim.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2anxmiykg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iypdvwft.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2phrtjgag.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrjpziok.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zyvsqowq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cqoooyms.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2cuiivuhh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yizymeet.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hhuxlxln.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ztxowhsf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2exlqsheu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tfcnfpvi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bwjhozrc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zrhjfowe.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qinrcyxf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bnlkcxtc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2tusnwpgq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mydrtpwq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jvdhavhb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nscfjhdz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nirhbdov.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2pzarxnpx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mzbsjepe.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2cvickwbx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ektupxzd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2bcgvrdpw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hjwwjxwv.html


<!-- 参考信息 -->