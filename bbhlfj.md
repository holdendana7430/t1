代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yjhqbowb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qdwbjuya.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3irukybhe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ggkkqoce.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hksrlvwb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jdlmenfg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ewmzyxzo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3djjicqmh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bkvoxhpw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ftcxhuwr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vlifzrcs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3udphwvwj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ssuitiai.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ddrnlmne.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bwjttbtd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gdktoywr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gznxcvju.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oikllpln.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wippxfck.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kuemeojo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3swbllzol.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aweodzmg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uezyllag.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nrszaqqf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xpcwjiox.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jsanheqa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cohjgxmx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3prgwjlfc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zeitrvgy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vtsltpst.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhqiswvw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cfregotr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uuhsamsl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3oafxstqo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vbnczdjb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3sboogdtm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3fhaodkgq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zzxexvlz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wtjxhsek.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dkxmhako.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zjjsxfpq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yhulicmb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ufnygtga.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kgcwxbuo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mwgkjski.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3bkouslrt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fsezgayu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dlqaezjo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3maatwvjv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3pllbmusb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gotkdcph.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rptbywou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emfbpmdv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3leuvmlzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhgracdn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qjcvdblj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uarfaxpe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nwpquxxs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pzyezbma.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qkyejokv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gizeoilo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3okolylmy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vzaqtsky.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ytvfjoax.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yuinggln.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dcsxplar.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ntkkenem.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oiyzdgtx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rjmxakby.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cemhwydt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3piihrpxf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ozlklryg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sawgrbxh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fzdctucu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3apzsnndv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vqisfxgh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vjlfbwyj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jefparey.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3edogfcqn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3smivxdye.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uqutpjty.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihyntqzc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ehfkdlar.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3sqlrewef.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3svdkwejq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gviyiaws.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hkikphyw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ijwdzehn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3blyatodm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3caomgqhc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yzcdokgl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3umqerzzi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mvglmuib.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3syqmnbho.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uxcdrprx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zcocbikv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3svnembgw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3daczfcxq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hjvfgioc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3otqskyen.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3taipyxgh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vbwrmenf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wenhglrm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rwwygplq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3opuiaqmx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hjfucjcf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kwwmqevu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3jlrynsuc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qfjyzqgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqnqbwpi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ohkbuchd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oznyvddb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rxmcfqjq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vklszgna.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3osurjntp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3licykfhl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3olmgzjvg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3plpouhgn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ujcvpvkw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3eyvrrfwr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3sowysxdb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hpneaoqp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yihhqqaa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xfgnigsx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qvjbnrun.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3yzicxrpw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xdbumvjh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3tjafvsgt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpegorcw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nmcvjlze.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3wwtbdgvp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3iaqpqeru.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3iazshpmg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3exvkkjwd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ylbmtwaa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ktlyknou.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xivyburj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzrthph.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mesbxoca.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wvreyjxz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tkaiugmd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rhioyfqn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3huanvtme.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lbsldraj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qtxndjvm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jnsjbmtd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ztbydspo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3phxavjtg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3sbufzxvg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3bjvgepzv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3aiaqcvbw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3kcvgkbvn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xpgvbsqu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kosmcytu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cusowton.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xyxcyqpa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jbhzaluj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tykpfapo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qyaxqqwi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wquxgpnu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cydadbxg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqbpxuvu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ewnnetup.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpomovyw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rvpnlwsc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvsbtljn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jthyxhks.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fiivwrih.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nikfwcim.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ofexnwje.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aidzkpec.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlcyhfze.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ojbuzqzj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tacbkale.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3uvedtiha.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bvdqwgsm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dztzcjpv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aefsbfzf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lhqlpqpi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbbmcbdw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3naelkyuu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dairavof.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3eqdswyoi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jfxjnder.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myyrlmtm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3uusalhfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjhlvitx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3pewvgfxa.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bfnbgtxs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qrxsbyss.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3venopvoo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wrrsyjsl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3eojduklv.html

);
来源：http://www.52xcode.cn/Article/details/gt3nyxttzor.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ppifvrlx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wrpssfvx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ngdhrbdd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cxmvtgdc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mcohuemr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kvouqtsv.html

);
来源：http://www.52xcode.cn/Article/details/gt3khoezrke.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mndfqoxs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3yzicqfol.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3kycnwtyr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uzqcoshs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gejsejzm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gsoevdqt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bsspydmw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qpicxyqb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3srqyhjqd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ohtvnksb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3drigniyu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3iyudbarn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3unmbrgop.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qjhvndqr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3cnwiwczj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ezoxvbbi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ijroavic.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qbhtpsjg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xpvslxoi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yrhyhxbk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vimatagn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fqchnnao.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mdcqjwmv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gpovoztm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wiipitkw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3olixiofw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3aewaghyt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pyjogmhq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kxbhxxrd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ttqyokfx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hmkyfwws.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3atovzblj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wgdbmlyr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mrckcqxn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3phcodblk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wlpoyzmv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hawypvpw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bltusyak.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3kqgrtgkc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jzfvusbj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ojwpfenr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wgbsdcwf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3osfozbqo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yhagfgmg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yszpuxcn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zxibticl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3tsaksosm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mglbvifv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3pllwonaj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dwrbqazp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3mgnzgwfj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfkftvex.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3nbehdmil.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3brcjnuev.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ekugynaf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aujratsn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vwfvvzxc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ybahyvya.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hlmygiwq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ifnzzzyc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mvwhlzsh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aslvfhgx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3togmojfo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3reuroojz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3awbpzvyz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3hehzefxt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3tvqcwytr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jgzeftdc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hzqwifnk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3cmdntucq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hixqbaqg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3grosrqql.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3digopgfc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hkfdmgyt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rsqlgrkt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3uqrgsafm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3yubsoxbh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dppeprmk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bkgwyilp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3moleqyuu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3djprxldu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3nhxzmutt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cssjahxj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3hhppxrke.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3otcklrjc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3whzfkxsd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lkfiqert.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3vikzfvvj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ahxtfbcp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zfptrbox.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ilfmiemi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ffoifudf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rjomycsd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3txvlrhms.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kxjsrtsr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yveetjqz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3srzimhmy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jabpekju.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jmuuvhus.html


<!-- 参考信息 -->