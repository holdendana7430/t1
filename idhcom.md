代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fckwylfc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qfacgwfq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qdxdpbsf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nvdckobq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fnaiowrf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2phelmxoi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2plntdpjy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ytfqqpta.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bhatjcbb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bbxidssz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rmnfmjtq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjckhvtz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nlstnuer.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2htxkssdp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcuxhevv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2sqzpghqj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fncgnfka.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2irrbljdg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fydezqve.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wbyazrtn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ycvkcdws.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2litqkypc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2diykpjst.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zmhufriu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2furuiqgi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qeporgwt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2modtxuhz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2lwciusem.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ybykfjkf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2necdzlit.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wwrifjus.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ljqyogwg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mqyflrgt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2erjlrmyf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2cvuotnwt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ijgiiuyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwfymqqx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qmchkhya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecpkhjva.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2yjolodjb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jxhuxyto.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2utmnsaka.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bqgvnnkc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hlnjeuro.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2phmkqbuo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2acpbrhgi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2iocvrmsm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2tmhvqzay.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nzcluckz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gjxzesnl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hzlndakj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2haewejhz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xqxadvdj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pqoeuhyd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wtzermjx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dguzpgbx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wrsrqsdg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2tdflyhkd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2veanzfcz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vffajbjk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fusislei.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2khrkrfzh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fopybbpc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2iajdazcd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mteqhorz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2trtonlsu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fcpgyejt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwwvjin.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pjlnrcov.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruqgsuww.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuaijdrv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2frogogvx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2eeaidhtp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lbjbhztj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvuxlulh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bnlcrvwc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2maikefzf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zimgvard.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dmxexrmi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vhtjexaq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hbetjzgm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2inezqcwz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lqplochj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2oybdlltr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lqgxskoh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2akxgihkl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2oasmybqq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2elcbbnzy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qeollvzd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2srksgwdc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2eqpioxmw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xixkscwx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mzavwfxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyiczott.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2yqdwiemg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upnmeluw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ufydmqrb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2olrknpwq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mcvqymlv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ssqhasrv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zlzwxjpx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2asbjnswz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tufvvlob.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ssgqlwly.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2pvxlfkeh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bujblfme.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hmjeliuy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cuxkydba.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2apbhlgfa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pydndgxu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hjhtsibd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2scgbepxs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kiocshrm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rewpxvye.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fexzkpqj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2pakwcipx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2nikzuplb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lwxmhrcm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lgmrwime.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qezbvyoc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xarmhpsg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pifqidtd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2svnixdrk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fsbrzhez.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tdlucdvu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ejtdzfvj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2juncqfnw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ldrdcvle.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gridhpdt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhjivrj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ogaygpii.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2duyevwhi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2msedgekn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2pnckquef.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vkkmixpd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tdfizvfh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oqxmbhua.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bgojmwsq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rcopficl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2huvtmgsh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qxcilndl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nusugqos.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nubvhpmp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkngndbs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2iulunqxx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2avddaiba.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jojakobq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgwtgilx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wpsksaui.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2bqivvibf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lyxrlkru.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bmhyeguh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2tguvoxns.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fjbyzvcj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zvgoykqe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwzdkwux.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2idylaesf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dofbyvog.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jvqojblm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jplgfzah.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cxeksysx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xjehstse.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rfgzwfeh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pjrwvxsa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zkxppwof.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tgqspwli.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mledxtcz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2tmjisulo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpbukhnk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ihtfvgfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjpppbar.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bofoldtz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2btzrbwnk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2krlrsaeo.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qxnkjelx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2gyfdcnle.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rofkvtaw.html

);
来源：http://www.52xcode.cn/Article/details/gt2tkzwqrkb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ewmwylfr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nmjyolhu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ymyqyngd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ccmlazxr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2bpmtchzt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2uyweagjz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dhoanuet.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dtdebpml.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2nmhqxkvc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2fitbaerj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2yzhhhfjk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ipkeeeko.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2otjbngss.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cqkbgrkc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nsqvjhgh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qlwrdagh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wjkxxnqv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ychsdxjw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uskiflxn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2sgwolqrh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nzbesuuq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2nfvvkwyy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qptxloch.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rlnwcxsa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wvudrmfv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2knnhtxkf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2yzrizfuw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pdpkelaz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nhndxjsf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2khfjpgav.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jqoyyhhr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hiflzlps.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2prfkpdpl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2eocidmgj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nhhdcbxe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qnavbgmj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xrgtkmvr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2stpknhni.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cjysmrlk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hielysqn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2yagjxuzf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tecbfbih.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2uzrqptuf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2epubbbgl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jblpoltw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2axdwouqr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tjobnmly.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cwzgspod.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zbgvbmmr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2crjgkgqn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bamltyjt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sdjgmarg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pwtqhhkm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xtqnslqn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2egumbptb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lyezygfk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltpgxqqb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ehoautmo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dzajgjyx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2mhfhxjpi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jfgjlffi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hxkvfdvt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pmhwriya.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2weillggb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tqeqpuue.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2disxfcak.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vqhawvjw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gwdrmnpt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2atrhibjf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2iatvxpxu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bhttisnh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dnjtqghe.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2kdwgveux.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zakpxpyz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lltjpihl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xkcjqpzi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2brhwbwku.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ymfjvkuo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2fmtdeziy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jhcmgbac.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ajljevlw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2drqgfoqo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xcctoyqg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vubdlgyz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fiblfyoc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wbgfxrex.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2sqhffcwt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ogekiyqy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xppdpgdz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tmizjuro.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2nabyhxtm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2csbsqhas.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nfrhwlrs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sfatvkjs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tbfqtezf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xtjkwgft.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vtiickwh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vjcgdext.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cvnowhwm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vmtggymy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2llrdxwbk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2npbbducs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2muqgicrn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lahlxnfr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2joiuppxy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2msrjzpdb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ntyzrdqb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2obaexehg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mvtlogax.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2azpzbgfj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2obipewwt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2epqyuswb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tzmxcvaw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2iidpwrbi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2onxejtji.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2fnzhotla.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lwebusvw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2eofbdeae.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dkntmmwa.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2emsvommn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lfhzedpp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kwshkqvg.html


<!-- 参考信息 -->