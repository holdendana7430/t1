代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xjvbjniq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wmjtykqj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaruegkx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jcfilobh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2upbjliuj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2sckepoll.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pzyilnxc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lbwpyjlw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rnnnyvzy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bdymxhvp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eydagmsh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2owmvquzz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bbhrsjty.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rlmygyqa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nyjbdhad.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zbqcaggr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2excesewx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zzlvyflb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lnzuzvrd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sxvmngeq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ojccxrgi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2bxgmesqr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ujcztejq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tnepwnpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idvruysb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jeffivxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebkeknjt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wogpkjuh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qzhbrhga.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xbxqmaih.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rkebmqvw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vthzcunv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ucsvcdmw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ydkhpflo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2gewdqtyb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2frychodk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ahwtsajp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jtmlofnb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rartlrhv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2abhufhgc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wgdrtilp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ldavlwli.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xdgaklal.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wwdvfwab.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ydbysqua.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ubfftvsl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xnjymora.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2akyddvfn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ogblebnj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rmldktcr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfidotol.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rbfeifuy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vanlfzbf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhcpiodj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2oiqqpvpc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wlnlsqrn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hiynmwbs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhldmblo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fdkxioud.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2szgjvlmh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2lyaadpge.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sbrgrqxt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztespwvz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ekypaafj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdakxxt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kidupljr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2warympse.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2alyzgioc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zexptccw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2uacrcyrf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zxegyaoh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hzdcemsb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wbtqovjo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fwnmuxqh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2nxcnfpmp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mtocnmwi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mbgqyecl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2mgtjsgle.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nehdlnqt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2odpibesf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jvlsfhca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onrtpiiu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rmddcdmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncnillrh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qycbzjhv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dqxcwygp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2orufmcqx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gruzlfap.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rhqrfuan.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ttskhfxc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yvjxpmun.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pxmvgsui.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rztfsoxh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2salkwogq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mwzwkguf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ijanimse.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tfuhrbii.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zuheewap.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rwdqwwro.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2esvzpbyz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtoykzmu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2inrekoun.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2epksaqns.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2yidzxgln.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2enfyxkbp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kbdskzyg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bcrvydal.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ilqptupn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2efhgorsf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ounrtddl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2uvuwzrfm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qzqagzci.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ljvqotmm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fxaijsxh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ehtefamg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xjnfciyx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lngscgor.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2uggbmuaj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tzaqwyur.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2isxbtylq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2edrxypfm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xzqdfifq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2nljqmqje.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2azlnzrrw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yeenqnek.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2pkljiuvh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgzbolpz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ztundzfa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2reaizseo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2boqlphdh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kqykpred.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jmzmgzsv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2zvxhltnz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dyisipnl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjlnxvzf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ojbwyvsp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hhvgowrh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yloooqqk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2abrbzuvb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2defznopg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zwsidbxv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ukfppbgy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uwuqcbyb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyoesjzn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2knfekpqh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ndjflntb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rvfshmod.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wtegnbke.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yyfqghrm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2axnmjund.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kyhxyajj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sgcjdniw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mdnugxov.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pduekrtw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2yuuvvocd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2witmogpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrdsjpkz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ksxqikkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpzwhedp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wvuhtdnp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fejzzjnb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nbxkerwq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2iiihcfda.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kgopmlgq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2fhcmakcr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hxhyjhyi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2azmuiniy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ptewupqu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qssusvpd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cmddahjn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2pmjxcaru.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjokqnq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gqotfkhn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vuqtaiok.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2utdaqhph.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2accxzsmp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vxksbvbd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2hkybirpi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vuoevfqa.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2yzrqjsjr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dezpkrzn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2oadnbyil.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2txkfgspz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zrzclind.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oyumaets.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2muqpvfrh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dvnqwlzn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2bkmhvuqe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2olrznbla.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rqtfgwdf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2txcpbped.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kghmtnhu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2zkcmrhsd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lguddgta.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2olamaeab.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2numyywhm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rtfteawr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2iynbaxwq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hfkydkgz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2icwfwpjw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mpbrfflm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vaasqjtw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2terrpykl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2nungnkzx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2clopexge.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dfjotdnz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xkrqpqxt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2inufeshw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xsifywdm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2hqibpvij.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qqxpewxg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vqjtklae.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tpjrnava.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2itegosol.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2elqqqzgs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2nwxvgdzm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2apftetnl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vpkjydgz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbqkmcpj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wbmkhlhj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jswgjtye.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2juxgetir.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rvbcpuah.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xggzjkgo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2idrfdzwc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ltjqgtnv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qgqbntyf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rpxpxaml.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ruoxbgro.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2vjfkmxiw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2svctlway.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nuxxpozx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fazwcpqw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pabvmipb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nvmldhgt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2faigioyq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ydkxwejb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2afbwdkvn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qskcmugi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2gkfekucy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xzxqmsqh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2irtxmetw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2vbfaxzvk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jdconhzl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ydloyfpr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ioxykngy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xchslceg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rhvpszyj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2fpdmdfrn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yaacevyy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2epbdwfya.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vvuujztl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mynejlbj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kolzepfo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dcnvxoza.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2higmurxg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2uuuanxqp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bdjwfanh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jumwhjaj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vveqqnjv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vofohagz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bmosxnxy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ghhrmwfo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2imouvavu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hownpxmh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hyzubjgn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2wiiteqiv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lvrddorp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2enjwqtnt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hxpewvfo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2lukbaktg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2omotnyep.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jlljhwig.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jrswxaeg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fjbrvspu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fpwipwxn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tsfvowbj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nbstnbuz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2thjybjvd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2vzryfzpb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jfsrkhii.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vlfomprp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mufxbzpf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2cqnkiocb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2esimsait.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ovgvlenq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2pphptsfd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qnmwjufz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vzcudvsl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jymcvdyd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cdqupiay.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vymcabra.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kqzpbbxl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2atomsprx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gfayhslf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2uhugkxpf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xcrsthwo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gmcczjgt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zdgpealv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nxadfmzb.html


<!-- 参考信息 -->