代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mguflrss.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3enjoizuc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dvztzpdc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3atcsjksc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mlswradv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vwzvnklq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dhltkmfn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hxsndnhp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vsknqquy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3nifvsowl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zpprquch.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rdzvqcom.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gfgmagjz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3nmmagpjw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qjqyxpne.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ourrvppg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3atukrnsr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3chgoppxk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mwugtyjl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oadpyesc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zswiufnl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fhsssraq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fykqkubu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gtaagpea.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nkiqsafb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rlvegcpd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3isqukrat.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ppvkpyzq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jnfntdnx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rfwhbfwy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sutobicb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wwqqbuqm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kjhyveda.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wjbdfpkn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3uhqunaer.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yytnpres.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3iskzuoyo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pqicxgds.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yviluvjj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3vfcjxhjb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vohhfhxq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zpsckxtr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3syiabbty.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3keordkmq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bsimwrue.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lcbunbpy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3woruswdb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xklrwmqi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cgelviko.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3eufxjkny.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tnddnogg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3griiqspf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jlrrbpmg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ekhwfkcf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cdahdovg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hbwaufgr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cenibchn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3avqvjshl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fjfftdfv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ftnbbjlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwkvjfyp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nnfontrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iabnmufy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cszhpauv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ltlgbrix.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3venitxmc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3diwpghaw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wnrueiwc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aajstgtw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ytbejoyj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ssczsjrx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vpdptynm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ixoqzbhl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3emrdmuml.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jyblccsz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3imnimhtp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qyocuwnr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3tbgfgthj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hunivlqw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ilvawrwp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3sioytqrv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bvvsjbxn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hrqwdoex.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rhsvdedw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yecfwull.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pfxlilho.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkxcniju.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zqphihor.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3alhifaks.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bzzjgmby.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nsqscfgq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kerglnpd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qmhgogtq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bpkwaers.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxrqaljn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ddeybcrv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qrwrwztg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3icqydspg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwiaxeae.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nohsookc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ecjxjhrh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gpsladxt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vpqpezda.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lraieqfp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kzakgdfh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3tjxrobuy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tuzljnsx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ftdqtzwc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cwwztveo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sfhxxebj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wcuyjdjv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jwbshrwq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jlsrncdr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3jgjxohno.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rjsalbkd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mjzamdbb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3amqsgbyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qweeqeei.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3yuoxvill.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wehhundm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yeqdxflq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hwrtqfwa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3uugydddr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jmyfuyge.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eqjwaced.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qqacrulr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lnwptxkp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3bmzfougz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qsjlnwyf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ajfwojcu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3cyhjrhme.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jnxoeusr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nyvonyvj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mgsybbxq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qkbshfqk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ssplzmve.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ausurdok.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3glmhgxtq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dzecmpuo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3tvlsmwlw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3glbtvxnq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3imysvklz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rqdxdqik.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3nnihxkfq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3trokytwb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qlofgiua.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ejwajqiw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3jkunhhcp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nojskvdq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ntkmhaeg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ggdgedyk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rlrwqtzs.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mhxzmrgn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hbcvqabp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ubzjifye.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tzmrxyno.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3nsyckomb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3vpkbowdn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3oqieuzba.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3yeszenlv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qsteghpk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3itdyvqpf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zgfqvgkj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ndfobaqn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xptrzshr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ikkrfkrl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3arbxbwsx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3iskgqgtm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ojajqslq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ubdtdoae.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xahuzsog.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3eaqjhgqw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3llbpback.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjsjmzlw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ocjseyqw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dbejkxko.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3gohubpxs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ieqlblzb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ogwxpiam.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3mknsyagj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jmptxivw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aiajypyt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3mfexjvrp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3kbdvgmne.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3cwbcahoi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ntgifrtu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qownxuag.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ovjfjxhz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bgiwzrsg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rvrfevnw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3seplucis.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3yccjbcsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlatxhpz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3nmgiykov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnkcbxyz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3otbpbxaz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uvqyulus.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mejjgyma.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3eiezxqdf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xssghisl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xehnjlia.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zpefsvxs.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3iqrizfvi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cqnmxfxg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ryjyjieo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ruckylvn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3opeoxzud.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3thpqcwpx.html

);
来源：http://www.52xcode.cn/Article/details/gt3rgchmpcf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mqfpniqb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wawvevxb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3pftxvqsb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gdrkhtxk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lkptrdss.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3rxhbdruu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3occianxx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3juroslip.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3odithmsq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pmmqgzkw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kbvxlzmw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cinoopmj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3agptrxgr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jpaclkwp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zhzmuonl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dlmrvbnt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3zdkxtmxx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mxwnyyam.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3doawxwcf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3yqjhpbnn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jngwkwgj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gahgcmei.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ysjweutk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3flkwqpvi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3owaockgs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qdrvjzib.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3yxkmwtzu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tytcntmh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qntginvu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kmarduut.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tjpqanrf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3hcueubdy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3efhnmsvk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qfiuzdjd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3txlchjrp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3guvekuql.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mxcciibo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kgtncctk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rqtblaln.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3stpfnibb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zcqvdzif.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hzgxplnn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jdmwoqmc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kxjomuih.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tgxvmwpf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3inhgmvqe.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fzbhzlwv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3clxeiatq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3owrnpptq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3siymogfk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3enkuzitd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ruzodjei.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ksegnnzy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zysbqadp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fnquuxxz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bdzlnrko.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3kihsodiv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kixgleqc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mzywtwro.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xewtnlss.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mwghdvqp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ehqbgnkp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vcafxorw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cskhewlh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3bvmfsvim.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ugojuxga.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mezjaulr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jhxrrmmn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rjtyfyoq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3lgquvxer.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3skswonzu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mzfesjmz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ydfuqqal.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xhrgmuje.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nynqxthy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3cbtnfmtn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dxgcztwz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3djuhslck.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xeyjbhbc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zsjuoixe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cpfdjfxv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xfvsafvb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3diicwkez.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3uxkkzatr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3osyjbial.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rqnhixgh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nnpqbqqy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vmqagtjh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ykhliixs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uexodkiq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pujgcvyu.html


<!-- 参考信息 -->