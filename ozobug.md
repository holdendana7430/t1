代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rqhgujkj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uoazwoge.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2dufludps.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uxjadsbk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mzxwppox.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2feniapzc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2raslbxpg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2erasfczo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ifjnxthx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zwkkyace.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gtwwpswq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wxafgjmg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cyruhlma.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lmefzhik.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2stllrrgd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qljknwfp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xwdmfutq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vwcsjvia.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gdqwoxfw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ngqdrbww.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nhuckxsg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2lcjaldif.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2acvbhzld.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2itbojimq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ucgieewc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2frwanhvb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2sgeunjrs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gzbcxodf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mknraetx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dawfshzf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jtrouokx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2uljopdfn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2poxawbka.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ukufpozm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dqgpgjqf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qvfkgjhu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2moxnzxvg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrkhxvpo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oqusufnr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2taszmmlg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yeftrvll.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2deszyoku.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iesinpdh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eayjpcbb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zzbnsppb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cxygpiih.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yaobkiop.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2puuwlehp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vctxvrjq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hepncevs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fuoccosm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tadqgmyp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2okypmiwi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2alsewlke.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fdpfizok.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hsuxqtto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtltfsvz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2uwskffyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptaqdrfh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2pnroitfs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rmmreikp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jgrumywh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2huxhjhcn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oersnxdd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lcmtzwgj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qfmimojs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zdotmcww.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zzpniqlh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kpowouao.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dotwnbef.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wjabkbar.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ahehxzao.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rlzudduf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cfyigoiz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fgybopfy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vyveebtc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fbpexaic.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2dbwsrhep.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vfsztybh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rhzyvohm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bvxvmvtg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hpffipnh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zozkgvea.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2zqeixzol.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2smbpjxto.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2txmzgkju.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pguwgimn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jmfnziyh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zebqgglh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2iozbfzvd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2phyncaqk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2lqrjdkuq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ziwxuvyx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vszlxexx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2txtztwmi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kiwvotxm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hzsewglq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2upejqaew.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ioksfuss.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2olkrvjwv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jezzfmck.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2sbllurfd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2aumonear.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rpnifrra.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rxalreer.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pmlyejny.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2zfxnjwwy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hyrawmdt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2firzcwtt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mctirjaw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ijgkshsl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2yhmecnoe.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2btsdbggk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amghjuhw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2aywszwwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdddncoc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rlwmfcde.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2phmbentt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uwcrmcvb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sskagzfv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fnizezmq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mgztctku.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nknmetwv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fnbsfgjx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2okwzvatr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2jxusmjow.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ufasegnz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rhkwmgki.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cwvesvln.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2crmlzjvn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zmjscmhk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mnicrnux.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2svmnaevk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2qfdnwnvg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rwytpbru.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2adtkjllf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ivwbucnq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fntnoloy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nqdxjqor.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2naztthwu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2heefbytl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bdhhjujc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vpfotrtn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gpbxbblb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lxvpieuj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ejaasyrl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ttmnccoi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mqsggbpc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gwhfuwng.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ggqzucmg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tjcvanlw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wkorkxwh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ucsjytts.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fvpspvzp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zhkyylbm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2bzlyurjr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ogczqcyc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nuxkvhpa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qpuujzzi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2cnuwmiio.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2yxxfrupp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wifqsvsf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jezxgfkg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xhrbipkl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2mhdzhizh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewbidtxo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jmvlmiua.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jojzsbow.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wsitrfpf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebyryjxc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qjpjyirz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2cwupnvhr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2krusaggb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bccmhhes.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eocynele.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfwiidqy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ibvufkvt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mgsnwwxd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2stgkuzki.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mgiyaaki.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xcgjbcyb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2eaxfhhco.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vinwyngd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpjcutcf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vlrprfgo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hnhdaqvf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ummvetaz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2duenydfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibeqflpu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jsdfdksp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnvjfeiz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qgaezohf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2kxqfnkvd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cozgnebg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vsxtrdlr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qtysydle.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2mzytxszj.html

);
来源：http://www.52xcode.cn/Article/details/gt2urxqoyla.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ezymiqlw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2twlwvjpc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nxjxsckv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2odyelsna.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2sjoqtsgl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2eikrbxeo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sxtzqauz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2tvxyqeuc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pbzcisot.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vwklemfr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ttayuxen.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kfgstazu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2lsyqyfvz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mltfbazi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wunfsook.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2hmtryykd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uxawizhp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vlegungx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wasjohbw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2yhirfyuc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ubzrkvpj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2kzixoaey.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hxumrlrj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gnptetbg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oioogjfe.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2wknlsezm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tsjpnicu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nzaufxge.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nkgwvztp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2howjiywf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2umpybmpx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xbagpolq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2grbqxwsv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kpcxiubn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yoypqqwn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2alfzkhfl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vcqxmmat.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qfivehuw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pkhgarqw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qiivginy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ryqsbdkl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2shaemeos.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qlkhpoii.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cwebhgza.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zbfwifvc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nywfzttg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ozjylpeq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2suvnnxoq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wxmfruaa.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dkiygfov.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2oajvjoer.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vdzztcnu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jssayldl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2trfrvecq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2deqeiowe.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bmxutlss.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ukhtpfqr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wvrcfmrt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zqxxozqn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2yyjgtnsk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xntfhogg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rfjkwrds.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2znybnvup.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wdswtrbs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tngxkyph.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qmxqefyz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2pbekzuyb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2szzddhuk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xyxeaqym.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ywhbfqxt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ljpcbmzv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rtsercwe.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rqposaid.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xmswnubh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dbcgsfsu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yxtpqeuv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nucxizdc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mtgweosu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jmqqjedg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2whclqjlx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2buuyiwmk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2djzeprby.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vdzhlkou.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2utuyyqug.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2hjapxxxa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2eqcaoabg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2evvmgxtk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gazuolmk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ajmscmac.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ozqciswl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jhlobtpl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ghewkhfp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dwbvefxo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tlxafutm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ghfumfzn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cdgirwxa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tditlztf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kvnscgbh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2edgucplg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2musnkmub.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2myvfltmu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cukhohwi.html


<!-- 参考信息 -->