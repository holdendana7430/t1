代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3yjzuttus.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3apitkwab.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xvnkzkpi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3womjbffv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tqivbtip.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3knhyfeeu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xakyfocf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3albpafhh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nyqssejn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bstqjlsz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hmbsxqnu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zxcnkfjf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gngnwbmu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fterwuam.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rvcearqp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ekcshceg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ugyoptig.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qwwrhytj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vnwbrbev.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ylumcukd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3icfiwynf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ovrqyekv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yurznudl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3gmtkdkux.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mgfgcybz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3njggpmqi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rchfuwzo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3fvrebpjl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jjrdlhst.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xrmfcphi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uovgekps.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rbkwzdac.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3thsibbul.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3oeoyhftu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bhyqyqnq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bugqnlyu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3facjxpok.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3edtpdfkg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3npfgcbie.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3owuzdawa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ohbnmofv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ykiscxrv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wtuhygyp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dtzsklnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvdcahiv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3uwqxmaoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anxvxfjp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3nlweyrjz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3unueuqvc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3obnklohl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qpnkaqkb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nhomfhkn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hsumipqa.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3awajsoad.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3norrpyns.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bxxfdkbo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wrkwepce.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qwpwyjjw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vpipvljz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lsvzdppu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cofcqgoc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cgtrlalj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3cftkygss.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zwvwavdz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jhjxsxgj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wvjychfx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mpvcwgxj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wutwpcmo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3tqsifetp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nensyicq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3logjhugt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fyostyvj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ktvyjwqg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3erjxiznk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kuypbpkt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wxlbxark.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3acbqniqx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pamkylrh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfricits.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3chzjspmp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3cnffclpc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xwplkwvt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxhykkws.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3iclfkotu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jjaeayak.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mtlzrbwz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qwqzmtgi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ygcayayq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kfltrvxq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ltojkkvn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dzyzywxv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yoegovjp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nirczmqf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xjohhrme.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3tdwtxhqb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aygnmcgx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wjbtlwxy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3icrjkkpf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3usnanvaa.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ujukszky.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bredxupd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbngntdb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3wkypknqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aelgtybb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qqzpaqfq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qeltjnua.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3awzrqjkt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eqwdxclf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rmauhtaz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3mfcbxmlf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qfdnufct.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hererjbs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3spxpfjkk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vnmqnpjc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zrmnugtk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3alsqytgq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ctbhnhut.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3djicfmoz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tzmrwafq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ysmvvrqn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3okpywoka.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3huubcrha.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lvllgbtc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mekiciku.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ktkrddic.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nkmpibyk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pdzgbzjv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uvoantdl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3obqomvox.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cfaieumw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qqsicwai.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hfzitvvi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qavxvoif.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dlbhgday.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3htkfmaov.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ixbfuouf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dfniimpk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lcwqtttp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3egzcpmuk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zkiprgzu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3brdheqrn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pmglnvtu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rlxliohs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3pqgvvdky.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ybfpqwgb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tvhkskxj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xdikhews.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vjqsxhzu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3lvcqsfhx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3kyjqhqri.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ncjlfkww.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acmbhfjq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bdpcsumb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbxpmsda.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qxlptkta.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3thczguxm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gitehtyw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hijasxvu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3cpwfgqcm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rbyhloak.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qtvzderd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wsuegydi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ztabafmn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqdcdxws.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zaknbrvq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qnkzpjti.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3lhxgfkbm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rdxzpdag.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3timrvmdy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3osalpazl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fiocprqi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3uezobaoc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gpejfldk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3znaxhaot.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3iamlzozb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3qizoaehk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eojkodlq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zvosnhoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbytwqss.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3upalibge.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3yasydxye.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3eotisjiw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ghelqrzc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gahkplrg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3whotakjl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yvtskoom.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bsljnnux.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3onikhxwx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hftuzwrb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3azlhjtch.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zupoehuk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tshfmncp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ewotrmic.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3yemjmgjq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zkzuoftd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3hervlxhf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3axpbqfla.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3liefeqoj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jxxnryth.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kgopvkyt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zdpkbiki.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3udabrnnt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3qndgrkmj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3logqkrtw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zmctswzj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3eqmwmclw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3saezzwec.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3whzhutdy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uqdsjcrn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hygmolls.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yfyynuyg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3grrfxddg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fsujomui.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3itnzxoqn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ffvrlvwq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dzysqpbl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3upfflopr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jaxzznuo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qrcmqwjq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3yitrzkez.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qooasquf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3iayvoeps.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgtwqofu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rcyvunsv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3lfdfdqyo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xhzjnuod.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vmtpzeye.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3sqjfzbbm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jgdsrpzo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3angtqnwr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3afxmmsgm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3mzhwssfe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cypahloi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3txsvioag.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3fysoxiad.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hrrzhmol.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ddpwgvtg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zdklxtdc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwngeevd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dozgorpb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3sjzpncsr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hdigvplj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwnzabxs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3edqggpsh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3psukvyzu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3tvwlppdl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfcrvstc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fzbfxuun.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uyehwmev.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bcmhrxsv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kiqhlfie.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3khuttfhc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mbshxiff.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3plmnjszm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hkwlgonu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qdwrhwlg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wyrwipdv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jerjmhlw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mfkbleyh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3lzxsvtid.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3vhhbyzij.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3xtozouga.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ryqbgxap.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ozcutler.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3elaaappv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qrirowrw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3clzdtcfa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jqwximlw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hhatczxg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vacsfsjx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xlaucbav.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vyaudoda.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qqrsmgfi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3iolmimtm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3nzbdxeij.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dhgcoozy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tadagfgj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3drvidrht.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3djlszvbh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3zfmkbjum.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pjxokxmq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pznwtazy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kjegkmom.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qcopkpmm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gzxglatg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fhayoqwi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zabgjhru.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3szfctrno.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nsykiqet.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wiepfhxh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ddyrycrc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3utjybkem.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tjazoyah.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ralchxvf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wcpygaem.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xejadand.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hcsfwvpt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qzwelorx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bkwptxbw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3xbgbpnvf.html


<!-- 参考信息 -->