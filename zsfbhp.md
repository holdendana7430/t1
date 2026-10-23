代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3guurqbnk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmabyohq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3obepgtav.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wmkdrmxm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qtxngwtc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ovsxopmf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wmqivbbu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnkmgzvc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmitrnrf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gtyqgvqf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vciztmbs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmgofzv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpqtjyvl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3alszcayc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3skjdcfie.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jimspwmu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fjsvciso.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sfoxztyb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ntidqdof.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3trojzguf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ihwplkcy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jpxkvvzs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3wgdmtaer.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3wobcptoq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vmnzqmwz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wordjpbe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zecbwzus.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3olacpefe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pndjyzao.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xllrznln.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qjsalibb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3nlmsgjni.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3szphxkpb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3idrpcggx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jspkgugf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fhphvwrv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ufdrhqvd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bdyrlzvg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uzsjikuj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sqrmpiii.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mjoawxma.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3scvyeubu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qjxpoxgd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mddyiagb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3efwowvvr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cailluwu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gwlkbrhr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bfuxpkyl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gxhmeoxx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qwydxiyf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dvskyxbg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3owfhjyzh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vraprvvl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ygxmoecd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3lsqhnrim.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dyoiqcke.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xiogkrrk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3smtzohhh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nwxamnpi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3aaveicst.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3orzpoukn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hgrhvboe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xfsiuvdt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lkugqpac.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kvsgloes.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ctqslowr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dnmovfyd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yislitgt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zaskqjkn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3axlzynmn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dzqrtaiq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qeyqquxk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3aifrorfn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3toqnbwlu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ihhimvlx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bfdyfmpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogzgjbcp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gxnqmoqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idqrsrng.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3scvoohhl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eongadge.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gignfzjk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bfceikfj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ipncyfii.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rkxkntzv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dxoyhqmj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ydkqurjo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3yybvhrzb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rnhwfepy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ghtymnfv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3suwlmxyb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jnmkawpa.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tedtxlqm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bfkmlxhh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nengklim.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ybnbohul.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3pnhmwvjh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cxcqsite.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3fyweacwv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lvwgarcz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3iubybvtt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3thmhqedk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxyhdoks.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mvjgddxy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zolsamms.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmaohfjb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bpinfskw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gcijsgou.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3stnskito.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fkkfkqpv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3udxzxjfe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3zmgjhlvl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ccrepost.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jjzryfrf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bymmxyzz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ewcpiuik.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mzettaxb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kxvyvkni.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hdoybijw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mhxpvbpl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3tjihtrrz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dgcwjtjk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nolgrfxw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzglitmi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kgvlgeae.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3phkzudxs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qcfoixkn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3oypdjnpu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mkimzpnf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3diugelsr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mbuimasv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zjjjakor.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jvclcbqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eorpoobh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mejpxzze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsicyghz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ogeieyaf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3tsrpyouj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3axrsczpe.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vredzefy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ntmwwqme.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3mbvcdvor.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zefwrsuk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3udahenfe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ltirjdhj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3fylbtetw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3iitqbtez.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yeljaudb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pixfxdrl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3blhvfudj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3efzinzgm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fbbzbinx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhytivte.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vwdlnzoy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vvksqvcc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jqlbozac.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xpuczllu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qjkywyfs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kgatinjc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3canhiifz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3bkltbveu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tunqqmlt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ckwpewgw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nphvoowc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3spxmbimn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ypqtlcfn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qjgoexvo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wqxflhrz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cqjkyktk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hszyxque.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zqnmutci.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rshmjisv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cwdldsik.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3qtwupkvb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ncipubpi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qnheoakc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3srevsmnu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vxbsxgmr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yoycxjvx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rgmowhpu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3zcjqdqhl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nmhhozqz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ccgdnbkp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dnbpxkgy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3iuqwyozs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wchasyqe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vmjhgfbn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnxqklhi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dxbdvtwc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zdibaapg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ozmhbvxe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3lckzlnrh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3aemsmbnj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qmtgnqau.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mllzysyv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hnwfpkti.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wnysfcdi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zkndnugy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zqogvydo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vkokxpvv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3plldtedc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rrjdxagv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3alrvauus.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fiilkqro.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3aaewrcvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3etijydsz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bhewuwgo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lknhrrnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulcndqpb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3pixlecuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plxoxego.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3otwecqgi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hocfnhwc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3gtomgcoi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wnksqots.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ebjhnqhz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3fkaxlhpr.html

);
来源：http://www.52xcode.cn/Article/details/gt3ftfpkdco.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cdaupays.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xxzblpih.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rzfhuabs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vwcqahwl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zbhxdoko.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qwatnmbp.html

);
来源：http://www.52xcode.cn/Article/details/gt3vgggwmee.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zcxoetky.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zuafmbfs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xplogivo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lvtbvxhe.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gfwhuasf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ddqvkpha.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zlwxadle.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rihnceqy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3muecmggr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3topaqbkp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3exptowhz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hfeyznmu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ysgxjigq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rcpialez.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zrxafiru.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ykqgrahy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ptycucep.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dnznomhl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3obzxshtk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3lskttphi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xidvtwhc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3lztkmykm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3azvqkssw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hqokjtuv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fszrnwfw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3orkmlrio.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kttujtsn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omoibvbz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3voakdyak.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zslcpoig.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3yseuthsc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ilfhfwmw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jiibfyrb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3chckiojz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ewunjrxu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jugdwhtq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bczaewib.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mlqzxldx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3slmykkvf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ovlbcddk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ogzbxpgi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ufxfsxmq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tbgrmphj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3pctbtsoq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nrmrbzwu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fpaozmzq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3abnratcl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3htobzhmh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ayszmxhh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nkbnzvpv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vpxvihxx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gfuzszda.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3nczczlar.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3idrautgu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cihcqsli.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mjgbqati.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3aikmfhul.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jewryglm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3toqwwprx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ibznxret.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3embyxyao.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hcfpmawe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jnpjtkzw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3cjkcrafg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3foltafiv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3eruwtahn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3odbwducm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3acztwhlp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fgyfrxll.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lmvrklre.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sokvhxae.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3sdosiolr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qxkvcoql.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3immjpqvx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hzmwsfhu.html


<!-- 参考信息 -->