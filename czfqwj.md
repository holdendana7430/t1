代发 wailian999

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bcfwqvkx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nutuwwpd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kphydwoe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2prdwgoqs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2coaxgndr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xobyxlmp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2reufgdmp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ryuflxob.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pukseiyf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hixjdzsg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pnkbuzmf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkgorhns.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wocclifw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kwgwrzbp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jcygqakf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dqdwnpsj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2elwbmsdx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2okbvzwmj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yjfhodkp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rjzktcls.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2exucctcm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ynmsdkdl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rntqhrcd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iaaygjfi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yjykdmaa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vxulmzbz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xwerqjdu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gywxyxel.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ltpuyayk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qfbhuxmk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kxptcyky.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nnflggec.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sfnxrtzl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ufnikaiu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hbuixmrw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qpephvlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzzftzlu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qjmzgvkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clhbgonw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2cbuajfgs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2faungkgw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yoyxsdhv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2iytpbelr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pjcjvaai.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bhfnujov.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qhkfbuxj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lrrkmayg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gozvjnie.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mdymyfeq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lizfncuw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rrkfmwbu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jopdqhyc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pkwlpkue.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vpicalkr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mfzxqltc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hhmfezls.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hpfkjdck.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bzywfdnf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ioeakvyk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kxpjstgs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gtwqumdu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2buqfxymm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qggtxhcw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2abeotihd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2gjxobwtr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qhygzcou.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nssatxgl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2dtlhdzbw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ymhwcchs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uiyjcndo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oadqhyzg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qttqznws.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pydajvct.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2khhneicn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mvcdrbgs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xpykyrpg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vzqvmsfi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2oxkjpjnf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cyikusfu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2koirksjz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qojogxja.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2shngnrqz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kxycivea.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mbpsjafr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2uywyfxth.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nwdptsig.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jqahvwlx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hzkwncmv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yyrhiymo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ooswrjdk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jdznwpqj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bjewnhte.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jxbndpii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zoowuhfq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2puyvsmaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozphvedb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jyfsurwp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zxjbokpt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2oywyxzct.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xzqmiito.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tsifrois.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tqfmqxmq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yybijjwa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kdtlvqtt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gitebjjp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dzmfmdsu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2zlecrkar.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ixtcxvwn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2othzlyzl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2somcgvnr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uqvjfgjj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rrslvdjl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2srqwakku.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2mamqwpun.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fbqcxvze.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fqcmexkc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kezuetni.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bornoduh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dgfasqho.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2muxvnexh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fofpoeuw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qygsrkut.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2epcbqvuk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftlnchhb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2kamlrumv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hhyhkohz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pxthiwmz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rjxwucbx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zubymawj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vqlehvfu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2izvkbsqr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yikykvbl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yhsgytky.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pocgvvtm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zzvjmygl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wzdbwvis.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2evszynwe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qjrfvegf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2youcqfgk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fawdbmog.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ptnxtkuc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kiuavhyg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pjtfexxk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zexwrmaf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2yullwrvf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2piowaluh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpjvmoaz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkchlosr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xullkuqg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gcxwfrzo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kybnozmd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2rbsnyffs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2nvgxvcli.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zqizogzr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dvxtuzkb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xjbrzwsi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bjuqtprq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sfwgcdyd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ywcxqcmj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ucglcgdd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nzuhlnzr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tmzrgydq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ctfaudhn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gockpjee.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xxpeyyys.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2eghnvnaz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hzozyvkq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vhhwsjio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eregiofa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2cmsojukp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdvuqdmf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2gadzgzvq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ysyzxhjj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2anmwebdy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ihogdxij.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2sphvecno.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2xcvmzkms.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ynoeefve.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2nrtjvuaw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bcgawdgs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yegxdeim.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2errrxwth.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yrwqdjju.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hcqcmsyy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2azeupeje.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uzgmmuch.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lxxvdybq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gsdtotzs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vqfbrnnw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gexrrkif.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2nbnelzym.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xuxcpwvi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vqlkavsx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qvhsmtei.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2skyhecml.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2reybcioj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nqnfcngu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xzmibuty.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sdwiqfbv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2lpabjowc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nuratfxs.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2swtoybfz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dyxkrmyl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lirpbwqf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2bvtokgcs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2jctyhjlp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yifrngng.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uahjzqhj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nsltrijj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cvzurabg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bodoqtay.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rkmuusap.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqcwpyny.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2abfwscai.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twbrsmwh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2papttlvj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ekzuclzv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vxgdaobi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2nfvcxapr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uylurftz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wcixfhst.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wuflnlch.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2swhqhfwi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2neeusxtd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zcmqafoe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2aglxgqth.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hzkkmehr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2aerhctwf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2unzyfwlc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bbxxjwhy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2waazyglz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2oqwyqqhm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nzgctmmg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ojhnawve.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mabeglpb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ndqfwqyq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzftsglx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hyekerlp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oemicitr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2khbuxpsx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2souctloo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2hbbxhvrd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2abhritqm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gcwksuux.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bweymywy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dihbbqto.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nyqlbaqk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cdljmuzn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qkzzylsj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kodbybvs.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jzzuakkp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2erojqqix.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ucuvskfn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zleqgpzc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2senunvpz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uxammsuk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jwzhoqmw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vufyaggz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ikppqels.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2doernmha.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qinsnawf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kvnaftms.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhplft.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kkplgwzt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ddydahdi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dbjqsibe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nubvithd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xfmziqux.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zaroenuw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2phgxaauu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xoelhesk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2gtxdkeyn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rtcazqdn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lewzuauo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vdrssfvi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wrpulxbx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dxxsukrn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kolktivs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mwlemcnf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dxaklzwb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2osmowcpo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kjjxvnby.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hwwsevio.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2agmvkfqv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2utmokldg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2vfoxqvvx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2uofindsb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xugkvixw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uanojten.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ucldedmp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2boijoptc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2itjdivcl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2grlkusxk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2sutugtjq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2byekyiim.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mwdbjojd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2omzqsjbj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xtevnjjy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ihbxpdjj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gapudmyz.html


<!-- 参考信息 -->