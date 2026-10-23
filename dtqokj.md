代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iyvakkiq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3obbrsjhx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ccretkop.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdcdjcmf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tukqnpdf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3lmgiarkb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cowzeckp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zsohiiqa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xpugxlvf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vwzxbsco.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3uzrruqzc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oaytkwre.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vssfmysi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3rdbxtuth.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3afmkfzpj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlildamp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fjuanvbf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3sfybllpk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3iceeltjc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3deoegphj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xiciabzs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pasxnqmi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nduoqhfd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rrltndsa.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hobyfqfs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3acikyncn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tigdfadz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jzqpbolc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3udvtjdjv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hpweexpf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fswrgfkx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3azbpnzyu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mfvqvlek.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dmsyxubs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3eddaqfbs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ejholmpb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uqslostj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wmwcnrjs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gqurmnqy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vzqzeqns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kixaxdju.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3iqdhuulf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztjxfgdh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3puyczvgm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nonnvgwp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3towkagni.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3orxpkcty.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mkyygkkl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zlbnlqmp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3mupoflwf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qoiwblok.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3acmecdsd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3pkopgezo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3euyhrudk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ztyyxzzw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xbzkbqdc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fpbsbjmg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gahrlqgj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3tbcgfqsw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vvlcfufy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3zcqgfgqw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jkzxnlsh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yxwtpcyy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ifczczit.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3czypophs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lrqstfhp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uicektdz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3dqtuvhpt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3dnusabew.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mjjpvxwv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3blgkrvgc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3amqwsuod.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fesqdiga.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lagtggfb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdnetcui.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vbwiluii.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3yzgxdmtg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3uvjcdnhb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpuiichr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3itonapza.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ghtwrzzz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3vtvwskpi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bophxcek.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mfniolhs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3dnhvxeqp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3tblnvipq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rtjbhvjk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytruujvm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ueqjjohk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3meveetoq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ofimxfbq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ydnleuea.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cwkdfoib.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3mysrfqkd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3geqpqrmv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3qeqladmz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xnvslnwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipkmwtwk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bsziiwaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vftgwpsp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gqgymxtn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mhnaiydv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3oufpueod.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ukplcesa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3poutpbjj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dghtewbh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3gpehwrod.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ylcfgocc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dnrkekfg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qqzbzwwq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qqujpzhi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3kcuaqmdt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vxgrnxth.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3czfeqaly.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3chpkjwjb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ttoaoeko.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3trshcjam.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3dntqldvy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3swzruked.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3antkkrhm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rfzbznvg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xgnoalrn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zzkulxzn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3iwwcnnuz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bmhgkaut.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ezxtngov.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3syqlriub.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tgymupff.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gotfnmic.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xpgxmyeu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ntkhfrjb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fumdhgzw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kmzaokkl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3sziignad.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dmetojro.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xthyosjt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wglyedtq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3eyptetmz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ncjilkuc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wgkdyqnc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mgdvdjad.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xbmlmigc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3isqahshb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tjvrvftq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3eexlyzip.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gmjbyccf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zigdgdld.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bawhevnz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zjsizayl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3japntgej.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqkbqmzh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fevfflqa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3anawruau.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzyckpcu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hlsnqnwd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3killhfsk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xmgopvpi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cjzyupxn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3swvaosxs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkrybuoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mbnvztrv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jkcrbksb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jojazzps.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nykmhrah.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3satgsffd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yovqkerm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ruhtyynw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlwokokg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3fhctwivd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mwnbbrli.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xszewqyb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zaqbasrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fedwtiwq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zbnndopg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yexahqrd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rwdqkejk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3vtkpvhtr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xnesomfr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3byqxyhgk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xcxykimt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3dftqyajz.html

);
来源：http://www.52xcode.cn/Article/details/gt3nsvyoxwm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ynehfugl.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3qxfvltnb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ynsymmuj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3aumkcvbs.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pcpeyzxq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3teywlrly.html

);
来源：http://www.52xcode.cn/Article/details/gt3milndkwp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xlogruwe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ahieqkyf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3aefaewwd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hjaknyjm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3obbklaty.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3irsefugu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pwrjfxvi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ftubounc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3eemdzygm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ttsgmlds.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pgprhtln.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3evqvtcoa.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3bzpxjfir.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bmzrvaoq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ugqqzxll.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3guojqoni.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jkwzhtko.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xucwjxxs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zlnlppah.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3znraqzpf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3aihivxoe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pgcccnnx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tyrxlmlx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gflczreg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3omfmpkck.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3slsltnkz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hedaizbo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pcvojare.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3slcxurhb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vqpflybp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nzommeai.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vbmilmav.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3goauquae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ktkhvbxw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ovdjonbt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zvgewenf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3uymvhacf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3dggspemn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3hrxvvqza.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3byrgishi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xhpgufhz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wsdvioor.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tzndbwat.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zzvbtpin.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jgkpcvmz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3glatjzab.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3befztzfw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3frahdsku.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xekrbitb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmldhpyk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3fmqmkqqq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfrsohsw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3avoikuab.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cbzmdlyj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3afleloae.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbhrfmfx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zrqmsxuj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oshuixwk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3twwegukm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3tfkinqmw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vjadtici.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fedrcvrm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ghhynqme.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3momeezcz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rivveqwx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3aqztmdhs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qmitsgky.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3dnodhjez.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rvhrcdhy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xqjudoqa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rdkajslu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3apnhgfed.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mkmjwwwx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cdvyobxo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rylkibzm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3urjxntwx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3swjdjqtt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3phykuifi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vmhnljep.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tqacbslz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3yijzrokv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3exklglee.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3gaxjwphw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cxbawcwh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3leqkxizb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mcglvsar.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rlnifprs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3jdscjrfd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vsicgbdc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fymfzggr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3dulfjttr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vivwycxr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vfgwnsia.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xuzkgooo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ttzdkgrj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jmiwlbwu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nhfijmhp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3tnocsvtl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3rorudjux.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fokkgdgj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dfcuugnj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3adavfeic.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mimpkafr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jnkipxjy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3vgjjuvgp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3srbmpuoa.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fzbxeuwa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lpslhxmy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hhmgkbjz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dkuqktkc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ngdtmhre.html


<!-- 参考信息 -->