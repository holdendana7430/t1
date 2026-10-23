代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3izljfotk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jkbyxmcq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3exshckgw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mazovwoc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wughjgeb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xxwchcnz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tntpxyvl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mtthusyb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzaisean.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rfsfalxu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3crrufvso.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkaafxdk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ubetquya.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3afyaibmf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dcocnngv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3utojvdru.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3laejlvfg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pekwveaf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wiqygzkr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ypmbaspf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nahfzugj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lvspdozv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3oloopbfi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hzhdvpon.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzlrwcqp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iihcgsxq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gkkxllic.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujnxewhk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dhcwfwzy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iqkaskom.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ftdlzdkz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ggsdbdwz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dezbpjpr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qhkzeyui.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lccnnfvw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wajaogxh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3noxlscok.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3npmezung.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3iyqzkhca.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zzirxjfq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3digpdksn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3oiggzwlk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mzindwbp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gwafdfrw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zxdvzccz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3vlsfwhis.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yewhcqbw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gpcxujef.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ainwmhvl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hxjqryzg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yrkhpbhv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sozcslla.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cnzqcwos.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rrkrksqg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3excgiiln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zaodbzjg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3glsjrvkr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rmnpnjld.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3oramhjyl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bnxnkqow.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gibghuhc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nejlzxux.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bvxnmhrb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cbuufumi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3crmxqywb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3acmypqwg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qtizyugl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3axzbfmqo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3uywuhijx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3eblvqgxy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dfyubtna.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rwdjhldp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vupxvvhp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3umfkexkc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tzepvhif.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uxdtlxrn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lndvhdsj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yehpbfcj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xixebxyv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3duzzbpgp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3aizacism.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3mttwqguf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zrwejtsr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lktyigsr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3paegznxg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jheaxmrx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hwsmyiuw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lbpyypku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufrqitnp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bfzlrqqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvizjpxa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rqvuxxvf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dgxwmask.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lmcxzauv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rbenfaqq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bmwrroxc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tbjknfkr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qvkcgiey.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pfgoltrw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wutswkiw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3pyzekmrm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3saopgeml.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3pvnwbzep.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tqcnfvdm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cpiwbnzt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jaerjdbo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ywkytnsh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zuvojpxe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zshpfgaa.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kwwnxsbj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xujalsqq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ktwtcuht.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wrowyajy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mdnlwedo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3diyqzmhd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nmcdboyv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xdyqtuzx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvoftbqm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3izsfmpgg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ifsrvzsi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hdvykkoo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cqunanbs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzwwtgze.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3uyjbwyks.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3oyirbwcn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xdxqipaj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhtixlsp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wfyqelgp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3silmjsey.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lgpkjnza.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3frcywgkg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cxlghqsh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3dwyfsphm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3kujjnbwb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yevnlbft.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3khrbjyey.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hdivleeh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bauhcpvx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fitcjogw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rvdxkbak.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qrxflkmy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gdenyqhd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3trwaoueb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qwvymcpl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3kgkfxlxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlzaqbes.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpkboczn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isakrepq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3acvrlixh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dpfeosna.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jevgokzh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tcwnyfdv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xuqjcllh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zokcirrs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yrfxiuqc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yveveecw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3kmmfmsew.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zxwqljlf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3fndbnozr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lkzxpinv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tozyfsha.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3buqnryfm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3motrispx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uueevfjy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3slgfcpfx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3obnjwmtf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3untazxrs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3uhohoipu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pzlcdwkw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gplxzzzb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nncuvjek.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lzxpisrt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3teboobgb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ycrbxvkm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3rwnwcrdc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mvjcxqjt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wdilypju.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3suhnxzqc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qvtktnhm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hvxojnif.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nxnbxojr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3yzmicboq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jroscbxp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3boouzjsv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3obdboahn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3nmycpyhw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3emzxwhih.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dwxebjwr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3elobwoyo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ufcwkoww.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wgopcdmx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3iprwxdwg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jobhkiix.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3cowtxcjh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tjhrhnlh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3erqkwlux.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3krzdrbov.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vsqouivj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlhhsete.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kvnhlxvc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3uriylfnk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gywtfidr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3cqtffzwg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fzcsavxf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3csccnnfm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3getxnixl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hnuzdvpq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycxoxile.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3uzxjgvog.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fhqzanhk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nivnqjny.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xoiullkk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ngysoeqa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3avwejcyr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wourzzyv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rttjqtve.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3kbydacpv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mmoelbae.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wctaamsk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zdkktlpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxjsbnaz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3spuebjrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjbhkvmr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xkgzrack.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3eyhlkqke.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nauakdel.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yxuxourm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3swncrlkh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lntsufnr.html

);
来源：http://www.52xcode.cn/Article/details/gt3jhambwqq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3jrgvcitg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3wfphtxis.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3srsqssgx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tecqqhxo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pknqyqgw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3astpapxu.html

);
来源：http://www.52xcode.cn/Article/details/gt3vmlbxelx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fggystql.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jvaqjgio.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3hvdsisps.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3aanjuvat.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eoaorohu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3twecsdpl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3bnlkwiwm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vvnhkvvj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3eaoislho.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iuchjwhw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3alqihtsy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zbsdwlej.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qhtqscad.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mlfhfrlq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cvtknraw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yhkajlmg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3luauxvuj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cdreyrxu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xjjstaut.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xpertpnc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jljyjptn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pcddrnhm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oxuvajyu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pcraygng.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vztecvkp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hldznjkf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lnqfknxd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bsuqqrdp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cnlwqcxu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bushsbnt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3pfvilxct.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3yjwxnden.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fzzortte.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3maadorrh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jinpbtgm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rhxbdlyv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eiprdsnz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xumlnmcv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nlbxelbu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dbiedqmf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hgxkdsrh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3edcnjkph.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gnnmeaec.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wghslgvf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vfqbhhuf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wshplaus.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3rzsxwvji.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xrseadqq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3akaofeui.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lijqhhts.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3sspvbwcb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lcsnwvky.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wicaodhs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3prqamszf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nuzishyr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nlsfncko.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3sszgunvz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iruqmuli.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3azgdsqwm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mbpegdvo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3knpkqkdg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fmihihqf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mtxigrzd.html


<!-- 参考信息 -->