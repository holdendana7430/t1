代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ogyktpmx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kjdzwoiz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dcarytjw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qkmssfpr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tjmrebqu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rrfqhjvf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bbhlumto.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fikoltdq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wezugyan.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lwfyvief.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nanvyaja.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zckjgwmn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lqerolci.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2byhhwucj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvhzkvou.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jpxmxelg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dthphdkk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fmlpsunn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrrgettg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2agsgdvre.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aisptsei.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2icqnedbm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2koihdqae.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aamjwlcd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2chbnktvl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xwqhlunp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yhwdfrbn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xuiwekkq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2navfihli.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2soychgbj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ztbovmdi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2kajcbwxn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cdarcidp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2soudphof.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tkcysfst.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kvicsvib.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hmqkvgwa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2whjndump.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rvlsahdi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2oejjbyol.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2skgdziqh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bjcawwvx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cwyljnwl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hfniiagj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2miuoyxib.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zbiqzlty.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rszsdvhl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2trqzbphc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2deoryhkc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ktsqgamc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hbwobfbh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nhqfmqyg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gsxntpqp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2corymurl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2glzzffzk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lwatkimq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ufxlllys.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rxtchhfs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xourrupt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2opnfdgwn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2khlufaip.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dqzzdwjb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2njlcywni.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vrqcgzxx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xigrhkqd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xdhmynfs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tizzbwer.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lmxrjrlh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ianjazsb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnnvhfrf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yqamqmvw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2htdlowrg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dholapfc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2higzrucp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ueanksni.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sihzfqgj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lebknthp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lemmxlhm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vqnljpwx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jlcimepz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bxbdbidw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2textipkq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2czqjylmx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2inmcjgkl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2isyylxdu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2tunarbma.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wvpzjyad.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gnzpsfqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyviavhu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2clzekxgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oaluifoh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2xjtjrslr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vigjckko.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rdpskldh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lluvwqlg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zqfomqeu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2itpvliee.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2dfevxapf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ugupyzma.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xbprnhos.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rfbmaics.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2uaytqxkd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gyzvmpsv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wxboqvbj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2phjukibi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2znjjrhia.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bhbozzyv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2emoxrgxq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2usbxfqmv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2iqbtwjrl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dpcggbry.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2sbloowfx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yoxicfij.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zoavzdyt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xcxfbcbs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bcojkkvb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dgqhhfxr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bxkctdpi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2poybgqhf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gxaqxboz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mbrrsjsv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lssblajo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uquzmzui.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gildsgyg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2jghgqkds.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zimtrrpn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mdiedecn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fgsegmez.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dwrpypwy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2nbjxaich.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2goiyfbgy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fqcqgkzt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2nelotwjp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nlruuftr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pkochvmq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqqftqun.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2jjmhksjf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jxpjnbiz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ifmhpzuh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wdhkjjev.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fvdiymni.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nnocvumc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hlnzdoqr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2vtxdbdpv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2rdjquyld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmkhffia.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wpbgyfsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgpwnygw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ytecojav.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2czwonuxk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xtgslyjg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wlrmkrjt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tuhhqpnk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hhhkdbvg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fjodpbcf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mpibxhha.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2txtinabn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xmtbgxnd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2awyxaotd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xlqpubmp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yifdkrpe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rfmvuryo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tgllefde.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rhapxdmw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2farirhwn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pdjrlzjf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jfegljie.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2uhkpnhot.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ahclrurt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tltimlyl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2njggvzee.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2qebuvtic.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ammuptkq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2foxveuss.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2iufhpugs.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ntdgonjc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2zrdwhdex.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pzhgiwbt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wkofwthx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2npuklsrs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2aiftolts.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2izgybmck.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dtpysocx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tijaevcq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xmxfuxho.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2dtdtsecl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xqsqywez.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ieriiptx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qmaihnzp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qvaqepnq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wxbzelfw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zcikmefo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2abyddpls.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wpczbjse.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zwinorpq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qkjcxuee.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bnbguuzq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wihahtyy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frovpufn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvgipomg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2csyftuzl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amzxbnpe.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2aetvivix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2czjqgvxq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2nannjzqw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kvlxaspa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iyurmhik.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zzeizwtx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qlermldi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2iipmdjkk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jtsxoovg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mhqhxoie.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zmosdhap.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mghoxspr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2eqlbdqlt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfyzjvlc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2aduecbpr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zbrtypxg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xmssusas.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2uhfaohgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whriwzkr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2onlbmjtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkcyqdjh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2pigttczl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2kbbbxcog.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wblrotcb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xldpskyi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cwudthll.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nckhrbeq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jiuncvfi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2naohlxag.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2fhtdiwxo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jexmcbem.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bynvzyvm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2okuzzbct.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2umszjevw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jpgfesci.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wpqezrsc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hvpedipw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ijxeoagg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xxydksho.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gtkdslkf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ydpdcrkz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2sabtrhls.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qpcxryip.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nfamiijz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wkcbbsgz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2iqjebnog.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lzpeleqf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zlkmfcoe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gwuozdff.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eioarkve.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2katkkhyc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2tevuelwt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2acvnvcyh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2yrtmjuog.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wdeycvwr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2cdgclmts.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ithrusxc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2axomtriy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nizlqtrf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2anruzuzn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dculuxnb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cieikhyx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xhyqmura.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ivbdkqeq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xrzlyutm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2zxsuoijs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2uqrxdyaa.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ebfkdfmx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2guhpxqwy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2fxlhzzdo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ztolcblk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2klzudhnc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2oclqussg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ubtvuyli.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2eqcocnfa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2adbcevud.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ntbycgpw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zndatnjn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vuxkwgbl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2syobfmtu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xftttfsw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jonlikzk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jbjdnjzf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ukzaypus.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vjynjjlu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rgclyufg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2engkpsoi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sconrmvz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kboprjla.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lbxlolec.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sjmxxuaj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wpcgkcph.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qxmspmgh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lvputpql.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2pyzewxoh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pfygmttk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ozkeqlri.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kbczgurv.html


<!-- 参考信息 -->