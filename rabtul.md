代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ivkgquwi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pfoqtwmp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3gmwvnyiq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3mchqlmqu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tpentgkb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3oygewfgm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qymhcdth.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jgnjjeqa.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gujqynbd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3psexvtne.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jojzxsrc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tcyimgxk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hszwiacz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3chwufliy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3khnixjop.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xaemdkiv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3aixlssui.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3osqcesxq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zdbxmgxs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zzttigjs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dhoyuhgb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3rufunmsz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3rdqmkagn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fmimytpo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3thlyjopa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hbkgngpl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3anffimhh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gryygzjq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3lwdvjpoj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvwaxuru.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tebowwxs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ohfhgmkq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fzxtleeo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3uqvtzdhy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qqtpizfg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xvhcnmad.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mdodtwtr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3iffkvyeh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xzciwixg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yyeskjze.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3yrsbebke.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cmsswvdu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xgbgvths.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3myvlivjg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pdiyfsch.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3uulesmzb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cpkyzzxf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fkfrowbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrohpnof.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bvxsvmnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvmvjaur.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lhujbbqm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3umgjtrbv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xbeuqhvp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ydgojluw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zdkwymhf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vxuzkqpg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3uypznamy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cjrvkxds.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qejdodgo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jhbjqpcv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xumodlli.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3noyjddks.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vjuhypjh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oxwwovkx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kwyzlrcz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hggticzg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3sibblkbh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3grmbpikl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xdyibshu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3smkjgynx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3sywgaaec.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fyxpobej.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mjolcnia.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqkbzwrn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3bovkwouu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pjyyjrcm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yglkgtnp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bfhvsier.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3sfplmlqj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lceyqxws.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pocjcget.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sosqgkzf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tdvouszn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wwxpjnne.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3riiciktn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lyttllgj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hkiapbno.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zkrqkawn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ctlzjizl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3glffdwwu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qioafbup.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xmbqhsiw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3isgfaulf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rznkqhoy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hhskntlj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zxjnruas.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vdcvpnek.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3fsajurjt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kpgdqddf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rgvqrfgu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3agxmfwrg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3eculsrbh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3icipaifq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3rmzytjji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzkinnik.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qihmyabi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypcetehx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3btoimtaw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ffgknaxf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zvjxjrcx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3axhkxagk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ajevczub.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3aejezlll.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tzmkslyl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jpnkezwx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mhrlciwe.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tbbhnzhs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vubiupid.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gxebgboo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qgmpodii.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tcnftrbz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tcqzchbk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fngwlifq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3upelvyhf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mzuboajb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lecgwdnv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hphrpyxr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nhkzvkfm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rdzcfjos.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3grahwmym.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dxrughgj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3htonkasi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbipvhc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3louoglao.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3oubyxonl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cccesrzh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ftfxuuvf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3eaeeqxwo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wzzbuvxq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ukkqfdol.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3loslwzdz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3owxkrvtn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kiptpmmu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jgigfqxq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ywxhnydp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3uqtvyomy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3fvvhjstq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3oxkihvnn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3wulzbcci.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aphlljmq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3frjoqzks.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mgplnofa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3udjypbfw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nankkqdz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghflybpd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bvveoplb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ansyzmzs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ershxhpn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3logwgswn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3fruoroix.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wlofiijj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3usdmwukl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gawjxelo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jcfubdwd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eervacjt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eulwrqms.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3flpmasjy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lodooxte.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yczvtfak.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xgyaspwn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bgtgkflw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3nfrnoluw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rhjktglc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qpdgxsrr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dbfpplcu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3pvmbkxmq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3tayhhkxz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3oyglpsmr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3otaruffb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jadpwbob.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3oppbvcud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyetnrzg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3klmakami.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jbdmpfkc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wrkfzfyy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3eviwfraf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3milatmcg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cviaycis.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qztntdlu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3byhiqilf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3mzyvefkz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3guurxvup.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ahlypbbp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3innwjufo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pbuwhvwq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qzowrhut.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3uohbdskp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nhnmsdif.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3zngwurwg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qpsmhuby.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3wcprgzdm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3oqzciazg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rxxjczqt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rhdmaydm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wlheyhhs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3amklkfhy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3puhmuteg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ogsmgsch.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ukuhvnyw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xlhfidat.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qbavddqg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ofobloyw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ibfqyydu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3grhgqnkp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3pramtnie.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gjzceasb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mvlnjqdj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3spcruwlu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jxjntkav.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xqbanukq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3twxfmisi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zlhdnrlt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xkvelawb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3insahefj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3knsesarq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sigiafft.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3rpzpvqgs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3enblgzyg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cdfnstwm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xqqbhjff.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3cgslfvlu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3aykwyvqr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3aduflfti.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jqwynmmq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3xrgcewmc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lttcfeox.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ugdhlmfy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3owrxyomh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ekcuvcnd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gibewygq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3egohmlvm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dgufehyt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3wykxsxwc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xmaagmnp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3jxadlyfw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msdthlcy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bdbcaxgm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kdecxmbc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3majonhzz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hihmppoa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pfzcdbrm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ceafhaaf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qwrxwmza.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vyxgskda.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zvrfucwc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3pgwkpkil.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3coyvwpdc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xqjnmjis.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ajbsywjf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3btstbwon.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3pjiuadkl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3eoufbjik.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3lcqrahzw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pwwehagd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3iatotlpa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jyttjhts.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xewlzspi.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3noswiwcc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uakwyasc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3srhnouxl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3omnjjjun.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qzmxoqbp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tbogckln.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bcikmfhn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rrszstch.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3weumhivz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3idlfrtyk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vrkyrsnx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3cjaotxou.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qecnihhv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3eoniicxp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3eruqxjyv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nvrtrqwp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3exufxzee.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bhiqsznf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nrjtdmyq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ttigmthc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fgtjiods.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mrxobxyq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3okgeeaaq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ojemgzyt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ylkimxny.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nhoklhil.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jdhlxcob.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hzpuedet.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nnkuhfiw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ygigzxiq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wdigybem.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xckwznkk.html


<!-- 参考信息 -->