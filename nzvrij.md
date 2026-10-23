代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tspaowfn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtzmrppg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3tchpsuba.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3pjtoszhl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxvfafnh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ycbwmxxe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iuztlmka.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zlpdkwhe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mrlodlbz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3eejoasoj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uypowugk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fciqqqfp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gzycaoio.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wldotooo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ojmtpqct.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qsrxhudn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ibupfuev.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3pjeeudbv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dkfkzrjn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rhykyxwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dslpjqrh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3saucrriz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfhuddjz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fmibvbwx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cewgrovh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bslydrvk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3gfqqqnwh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pgavxnyq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cwfcgmci.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xsyqjgap.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3joqwbzkn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kejqzyoa.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3evthdukx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3wpnpjpij.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gxrujasv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3daeqoquc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3currjttk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xoycowmb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3qsbkxcmz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3llbnhhwc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gidqjycv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wfxwqjho.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykszamgn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3dpfjwoex.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3tipngdlx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3menjavgb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufbxbwyn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xrbtgprb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lzfkjdnj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmoqhgri.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vgsrmxhm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3njdlcjbc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nrmewbrz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cirldwmp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzqdjgqk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3upnsslwd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hhnhyyus.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jmgetlix.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqsfefyh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gekjlkxa.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zgrpvgkf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zpyastci.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kymkgoiu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wpmekdar.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gczthkfi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rvfuhncd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sbqgkvug.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxhineli.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3mowqpnzo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jgkulfqe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3guqrwxfa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lfatzxwf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3inbyooxk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tqdmpbnf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ypkcfykh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jrtdpjli.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kfmmfhec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sodehwsc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3fvhaowiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpljubac.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pmreoxdr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xbnuxngd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ruzwvruh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eionfjlv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3agsymebx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lhljzgct.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3omaeckbd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wbocclft.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gblkhgzs.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3puoggwya.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zsobgrnf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mzhpfwwz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3euxhbfcs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rzuctsfg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yqqirdwi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qcaxwifw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3aqebmkao.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ojuyilgg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3soxmmdzf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kopbwcbh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3utuemxvn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kenbyeuc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3alxixcmx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iiyejkob.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vvcafguv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3awlghkim.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ozetcoff.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vkipkkgv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3duogxfwg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wdikqwoz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bacwhwis.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ngyifhhv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ctogbvdk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3yloljdno.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3druwxpkz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kixakejj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lihvgyvj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kvpsoeri.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3tvvjhdnl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zbwmrtpe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nemqozhr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jmulwjzz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3esyefzfh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ytayvejq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rkztkzud.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3axyxvkwx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ypjcxhiw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byejojke.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3hbsdpuwh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3uvmkisnj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocqdarrs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3avmdoprd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tbhoirzs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wtasimck.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3tdzbuxib.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dofydcvy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ystkgboi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dvahvlyt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3brcqarpy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvnkdhhs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qiiihhmq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ijjlvzup.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3clstwysj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bnaajmfg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ltkvyouk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ohzwbrvw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3gxldhrey.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3eojlqgek.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3emmnxyri.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rfzgrbyn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ttlnllhq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3defliwdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aockvojv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3pylslizb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxplojan.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ahpjsroh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3piobuhpl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kcszpegr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lznxkcrg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mmszgrwf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3zqfkxelr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3owpihpjh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nabzhfwg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3edefzedj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fjlfrdvl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uzqywpod.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3brpbjzkx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fwmsvytf.html

);
来源：http://www.52xcode.cn/Article/details/gt3nepajdiu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ynkmglzv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3eaxeikdy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ibuyutwn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dqsnfovd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xudntvgr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cjksnuie.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3svewdccn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hhapozon.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ptuynhki.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tlkuxxvr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xmuvuerk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3brbyzrin.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mjbyaftg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kudrxmef.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xoefwgnk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3effrjqje.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3eblbhucx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hgwxshds.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jkklpvqv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3msanbxgy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ywfazjgn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wryhgzlj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tndbcene.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ertfgicw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ujtcjhmi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bvswhqfm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rgkfcvrf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xthbjmdg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ruroxzgp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oikxqqvw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ahqnjxtw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fewqiueu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gbnahyul.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3jhatysqy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3iocoxyrj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xlrcwjwo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3liyzmgac.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3iveoasqv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aikexoxh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ojainqru.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3uhytjpjn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ybmzhvog.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lbocssmz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3mtgiwxik.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nkcnowqm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezkjqwwa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3xejvmmbd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3yrnrratl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3aydvbmqh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wbedgouu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tpmvqjth.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmfvmsdf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dioydyls.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vauylumg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3efbmicwh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fxpnzubu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3acfdnegp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3idwzzxcy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hseklkuh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ilxkxsts.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3niezgxen.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mhgtxrym.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pemcfmzt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mqyvvlnj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qwdjwdsx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wlurkvyj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3eovyekhp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gtpqshgi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3czjzcprq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kicqixnp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zhxxoobe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3msgvvzhr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3blhjlryr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mrhbgbgn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dtrocksp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ecviqpkd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rdezwqwb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3huqtyqse.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lfpheuvk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xjgxkpiv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3whhicepb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kcdhnirf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kmdzlmjw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mohteaof.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ffipmulg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3urqriqmw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lvymqetv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3yquhpbfc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3synyrnxl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3remwjdgc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3duyctepl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xjjsiiii.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3niucwnzz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3tjqznaah.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fwszoktj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jyltmoxy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zynkvbgi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jtimlbqf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tiawkoqq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jnducvfc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3zfawszgb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3btifuspm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fmlhpqkq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3unxxvgia.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3esnjahlg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fgjvjzly.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kidcwymr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fegmkyge.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cyiafhyx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vubwxala.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3osohnajv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wqzrkwsm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3lwosngdo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ibhyetla.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uauelglz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3clbmibfe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3phggpiaa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3iuyibaut.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mhxtwqcu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3olbhlvpo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3axneryxb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jehvaaxg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3weazeabh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3awchksyl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gvwsfocz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3obfasnib.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3thixjhgx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kjmlqzod.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yatrtpmc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3flwttfzl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gynrnews.html


<!-- 参考信息 -->