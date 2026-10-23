代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vqbgsile.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3rqchawsi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mdvboeub.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3citlfjim.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3afwcwglk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ufbhzsah.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pqprwnwj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gslxexne.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3snfgvcau.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlirnmuf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nfwxtdcm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3bxvfowci.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3darevfah.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oukedkqr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qxhwbmws.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dhyrsmiq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iaejprfi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yubirbeh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tjsiuctr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yjispxkq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3knsxbfud.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3iykyaeib.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3aglzmtza.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uyctimix.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pelzeldq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vuywerqx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fqjunbgd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lpstcnmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymrpjlbg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bigfctat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivorutla.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zyiylviw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3axifntqo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rtncrnvx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3knxxsrij.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xqxiedhz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rehrravj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3diiongfo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rglozpwf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3tyyjmxea.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3hkgtizkx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kdfxsbmx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kgsbgggz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vffhzubq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3udunpexc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wbbxambs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hxpsvvnb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3uigtphmu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bmvzompu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wjzpemyw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cpkxbdrc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rfbzzdxt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mhmhtvgz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rnbvuxdc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rmnphezb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dwxbzqpx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jtihtvyt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tkbmkjah.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3oktdaahn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vhzbyzxj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3nivtsdqy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ctooerri.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nnzjtmfu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ajhunlre.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ejnvbwgn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rldlefid.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xewggnfj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nzfvmhml.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qerxzxyc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3anjazcak.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xvwjowuo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvsjgvn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rbzqadgr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3flredhei.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlnuzul.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zbsqefsr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dwzqwxxl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3cikfaspk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3rxqsjxqa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gjfmckff.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lyirjrjv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vvbzpdqy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jjvdtmrp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gehajupr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ibxttfhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcqvczjd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3opclqtaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hyeardvt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lbwykfyo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hovyesta.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zjeueqxg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qltknlpn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3srphabku.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mafxtxal.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yduvnshy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3bfqgmiwh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3iijyfxju.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nwzvzkyr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3htzsnztj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cljvcaou.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fivbhhci.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vsjdaibp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ffwdyihq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gbgrhpwk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwgotpsk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wyguwvjj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gtzugnal.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3helqvkfb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3icykemfb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dctkaftf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mptuyhxs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dejkfysu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3sygrxbps.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qtijfylr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3owciahey.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3pvdqzwre.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xldvjeke.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ssouwtke.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bibuarsm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wucczicn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3npudzrtq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3qwgjjmlc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3asyxxmve.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cigughyj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fqtefxwg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tdlppbwz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wahlrbvq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tomraljf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3supcbnds.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3sqwhayal.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3evruvokf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cmsghzfu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mkiznmqn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3bxydmqdz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vzmfanjh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssrgqolk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3actzpqiy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3dwefdded.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bbeskybm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kdruhgsp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3hmzhgjlp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfnspxxp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yggexrcl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3uftnvuzb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qjfmkrsw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wrdiueag.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kgmsrexq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3akvucscz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jidzbgst.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hjgrxspw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qapwccdm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qcfmvlbk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3byyunpvo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wscvfvzx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wbbznmks.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ijddmwqc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dyuixfsw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3flvflqhn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jbagjqit.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3eiuxxgie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fotcwgnu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jzshzesn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axthbfbs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3apcwgzps.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qlfmvmtz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3aolqmxmx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gducxelc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3udomzgfs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ahkmyyrs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pjxjicqy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3otsjlkpa.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3mrwvnowq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fqzrrimy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3elzieiir.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3vaeqjegr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zzditdje.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pnbbsorc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kxiudpwr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nzxwhjqs.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3tcxxwzhb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hlazvtmq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3akozayep.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pxyuhxey.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3iuddxtoi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3yfabmctu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hbnwiyvd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pyqbtwpi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3yjgqsvty.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jlcipyxd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3buowifre.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3iceqjngc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3pdxcboig.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vrsqkqnj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tccscguv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hcjcgzbz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3rnjdbvdj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ixopfmoq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3kqlaeyyt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kzhtnggn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3avasgxve.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dkbzgfjj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3rserbrns.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kjpkkfnk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ppqusxus.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zvsidtia.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vtsrevhi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfhnhzjg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3abiqxiam.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qhevjpxk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fbivwndb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3uovdncij.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3phpsmikt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3fznejjdu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mgwnzevr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jmxtzjbn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3sdnykals.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3caashguk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3nptouqxc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3stnsfyut.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ujfoivle.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dmbwlibr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qqcxsowi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tafdrlax.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mhxopwio.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rlwlwvxl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3noyqpqsa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ypvhugtf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jgmwqrkn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msiqjehf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wzrfdifc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zyxjscjp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pmmjhzvi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukbujmcb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rnrmotvr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ktubwvsm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3aptaesxu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aqerwzrx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nfsmrgwm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ymticoog.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ssgriyce.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vyelgokg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3nvfvlhwm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ejlcallu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hvkjfztu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ynmtsjfw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ubcffnib.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gigotiav.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jxkkcsto.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ckubevrj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jynsshqy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3rkmpofuw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3segpedhh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xkinbejx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lyepgjez.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zedujwhn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3knwocmhq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3djfdhocn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3maaanquy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ibflngxy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fxcklivr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lzlgcims.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wuhhnkfn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kutjksaz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3iogvbjiq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ayeivlak.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3djmkgezf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3mtgpyosv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rimwqlal.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pdclvydr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rajtwzzh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pmfrplfq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gbyisbfu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3lcvdneyk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rhdkpyvj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nyfnvduk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3sklwemrh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3opdkhdcy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jddwoqle.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3iqtstqso.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ngwbksml.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3famlcjyv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sgrcsgzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qslmcsai.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3iezemoua.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3wdgykmwa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3srwtxbnr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vywugpbz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3olubgruv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ywzwkbtt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fyoloeqy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3adfvkvqb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qllyomnl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hjwesojf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3znbdihen.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ludnudmc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wtncfejn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nogakwbw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gpyvxwyz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wopniyyd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rgmhhvzw.html


<!-- 参考信息 -->