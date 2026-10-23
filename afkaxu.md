代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3emohdyrc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3etzphdwb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qzvlajdq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3sntlvumv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zqyfezau.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bekbbnsr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gvdnmrzt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iigdcmez.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eifvjtvy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qpsmlhti.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yntffsln.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kaqkjswj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sgwwekcg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rdfsgqqj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rclqhrsl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zzvdjwka.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xyojpprk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3oujfixth.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3pxrlvxpm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nrwhqvop.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ktsyaxce.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3frwkhsce.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zlooxojk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fusdsgia.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kbkjmdnl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hsxvxajv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jdvhqadt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qrdngklr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3toagctbx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhvmnyye.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xgqhisrd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3wqkblwzq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3tuxedrsb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rcbxlfit.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jqtuyouv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dgqgvoll.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sackkhcy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3cjifjlyn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3drdtepwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vaftnuag.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zevyjskm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3yrmfazae.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qluvvzor.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ywxlfotu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hjjdocom.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mhczqjuw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wmnmssii.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gkizmlsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iacsqjbo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3pgjujuic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwrpldaq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ikageeze.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mpqdmxgh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ssogrflp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3yerafhis.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bxcpymtr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ptqvcuog.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3kfppzxbh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3numdthhd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ptwhevcj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3grnytiin.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3glylfehz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3cqjvrwlz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nrwxcqjq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iqfqrrtz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nqxzvwxm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3zhnyrcfp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hjdvztqq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3fiagmrob.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3eksoasjd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3sgkjbqmw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bzsprhdd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qjplgdsj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zdbgazzt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yotujnrd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3eknnzwby.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tswixgph.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcqloxvu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xmjrhmco.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3alfkaeyu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dsmrtqux.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iefwsuar.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3czpjdapt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3njvciyph.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pdvikumg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3yekaljbg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssshqngs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3gqwzcchb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wjratcmx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jqyqqiaj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uapqdvsb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zhayoasb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3agcifczw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3alsguwem.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fsfuuazb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikfycmvj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jwepfswv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kiasrjlx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3akccxauw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lbwlnvua.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fdapqbjk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tfrarequ.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qnvlapyi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3opakerec.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3yndixjsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3scdsdrmq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nlnwmnwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdbhaqvb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kfbflgyt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cexwjsbj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vunpylsj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pwzzmega.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bejauqze.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jbrlnfqf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sjemslhz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3josrwris.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hagsfwpr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hrsainzs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cdxuspej.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3uinxvuuf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3xhqpqdym.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3cxajtkfo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bwmytgfp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3hfpjqrma.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhhvzjbv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jhtwygzx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ojkjbfal.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kjukkabk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xsvgrfnz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qonaxjro.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dkdgmowd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3crsrozrx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3rzdqxeym.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3izmqutdg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mkwegtcw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rzknbsfg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kjmlxyxm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tekrppmk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lurndpmj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rlfpqrrz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sekbxotn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdbfysh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kgaptbil.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3guvadgyr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fqsvnpoy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3szimyhkl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3lplxxzkf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3nkpuswoa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kwkaasiv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3nkaxftrb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dshbjjbh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cwbejanq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3fiiyqwyt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3byzkdeur.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lmdbvard.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdfvigdv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ykrowpws.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3azhbcddv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyacfqul.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mcmauvvx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3kcqajfxp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nqweixkm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3cwqhkwjy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jjdptcku.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3csjuaxyf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jahovuaz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3odmynyme.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvpohszt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3abilnhqq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xhaccnqm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ozfcjlyz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yyauelbl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zqrzmyik.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zlldmppm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3emfxprgc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3joaurxew.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3agpghyfa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3msbuoddr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vrpoxsrb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3awiqewcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuqxlypx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3onghmttw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgtmfrkd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pahigycr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3cmxpxgib.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mmnfiuqw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tbkdggtf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vjufmeuj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rqceaqxk.html

);
来源：http://www.52xcode.cn/Article/details/gt3njlfkwzr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cmwpfdgc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vevauila.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uyosamrm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wpxogelm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3rnumgaik.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3afepfqoh.html

);
来源：http://www.52xcode.cn/Article/details/gt3kqrwygyi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ipurhvbu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ixmrvnfd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vvjjgcit.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3skonzsyr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3pteoiszf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qgjyassq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ccxahypx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3eqlvwkte.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dprehywn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zecpbzsk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kfhtkncl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jirdupkf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mcbaxpqz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ohkubhjl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3owvadrcy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hllyhjxk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bgijxtkb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qtrmumsi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zsfclorl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gcucfxkm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jqzzlann.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3harmtnfh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mcxihbjv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vejvxpcr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3aljdholk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rzzknzbm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3cdhlclwq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nisohlia.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3laikiyxx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bafyrbwt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3apciurau.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wegdebsd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3njbxxwhl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ibsgghpq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3egjvfozk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jnsnvoan.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3yxtczkxx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3phibbnhr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3sdkbvgdw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kxwmmoab.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qtnlnzmp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3nwnkzjgh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qmkhhrtl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nfqlzata.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jwfperxx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jzsjzslt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nddfyzqy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vsizzsxv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yewwchns.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ocjosmvb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3iaqaztcl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qixckvlv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3dzlwykob.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mcpnnvyl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ypgskxgz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvyevetz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3twhtxwtk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wekehelj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3klwccirv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gxqfidrc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3skhdtkzm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nldneomr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fajprgpk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jwfejoty.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qjjzjebv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mucqhhnz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3holapbzq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dtyewvtv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fwtlonmz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kcdicqsz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hiuczvam.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3megivcct.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3giaixoxv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vhnegtiq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fxokzvje.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fyeszvgw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3plieqmrv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3abpvywao.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3siqkyyaa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ebjtihky.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3glngxiri.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vrbytumf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3rcoukrnq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ykeglwjp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3myxxuquu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kxjorglh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fzmzdvaj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vzmgscuq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3emxzrcqd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3astqtocf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vrnyqffr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3peiqnqch.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hunapzxt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3jqriqsyz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3smdvozgq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3euesmkee.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yaemlsin.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3crjhunvb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gddcleww.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3mmiadusw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wucwhllt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rbnhcmyk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3siafzzry.html


<!-- 参考信息 -->