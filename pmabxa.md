代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jwtokbvd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mpgfyeor.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bekbtyzn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3oisummir.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sruhskai.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tkenyvnf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bnplodzo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3equiafpp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tyvxszvd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3telbhhxe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qqcbwpim.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mdvcnaku.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rgtvmgjh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fayrnnxp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3timpwxtq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xqfulsen.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3swohjccv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bifwohwb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3okguaebs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kvafmrzm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vowzkxwv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wgrjodwz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tatwmwjq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oummgdte.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3sgdruyfh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3scqzjpod.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjktaqln.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xchrmwmj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmigvcjz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gvgvgfae.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kghynsxc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vhdsrvdw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qxstdxus.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rcdxyuev.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xvhyxmiy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dghenbht.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3txvsaqsf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dqytllns.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xrilutmg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vsetlqfy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3igsqcrec.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jzfvvomv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3alntossi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3iaixyish.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3mmmrfyok.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ulfxcruh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vyazkiii.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zxcisfvg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3sodocebd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vhrbxihy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pzqgowmm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zpskcber.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tsvjapyh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3sigrwbmi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dgbamwsh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ajfsdamu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xywbmiec.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tnimztmq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3csktysix.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3grdikdsy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wjxdgrtw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nowymbmc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pokynbgk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gkkxuuec.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jwkpvdcp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3honktazj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wzjcxtoh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ntzhobke.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nrlmazvp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3sltxcexj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bpkznfqt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cgszxgvv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jduhvdod.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zpljdfnr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwnwzqlw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3nugggrqu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zcfmizzq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ljfluueq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vmtlhbfh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wloynibk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3laizjbhl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iiuhwlxp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tldsfnhm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qdlxwonz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oyhqpixr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3aiiyqdlh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ghwvuvqm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vdpuwxec.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3upcdumac.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jbvzctbm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lnjmflgw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3neplxiln.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nukjhyoi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3sbkgetfd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kjuqyomd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cghcuvpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glmpvnlw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3iwykykvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suxznsei.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3uomfmuuu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hpfdvhmj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3wgzvgrsy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cyaxnkff.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mgarlsmd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3feswwaed.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3weivmklo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ipadrmgg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ldpiuimy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3swwochac.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zysrvaxv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3oegjshmz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rhkuuuho.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nmdzqmtq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xehlyvxh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ntgrsvcx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ydgcopkd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3urseazmz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rrydrpax.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mzuspxqb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3elumhbuq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ylenbjsv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3citnvzuo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwebejha.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rhnersnw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tsplerke.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmxdrclg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qvdhlpjp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3reqlertz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kmvyphlp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3spriryzj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vurhuqwh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3pgybwwjj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3buqqnsuu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ovafdkcb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsvxdgmh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xewixvrn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gesowcma.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tazwhtue.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yzszjanw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ozoiriqs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wagiafct.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jxpgnqzy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yvgeztfk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3syhstzoc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jdllpzyw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3gkvumgvx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xpiyefel.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wxfyiyit.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wtvkbida.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3toxeumip.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bjjlassp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hkcgydrw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ozwjqjud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsqptxxk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjvdotui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3miggprfi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qxsdntvl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fjxpconp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ojoujiln.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ftvtynti.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cddkvpud.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hhnudtsu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hdpenacb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jifwhtul.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ahzplmsk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3shghhcyh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kjnovdds.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cgjblqgx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qszkncrb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3eirptrma.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gfvorqbm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3sfkjjsrm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qfipgbox.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3afdxckjy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3agzygire.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lrvdctmc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ayqsqocb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kmotamkt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3avwtoxyv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ynwoopwl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wmjofxpd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lzyngvgl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3anxiahsi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lpagqevy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3frarbdor.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vitzsezq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uwoswhgc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3itxcxjfn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tytgwpif.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dcdhfnqe.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3sxpllrta.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3utghfdhn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wdntbtpc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zxepoeiw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ixhadwql.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3odnyslkc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mrywigcn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tkldafgt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bcvzhquy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ofahvdzr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3psxxowfq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ayilqkyq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ctrivgss.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzoqkjxa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ttzysaoy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jcqhtnqp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uwghjhvc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3wleftmbm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wzygaser.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qadtaqyd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3czopjeqk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mgqovtsv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lqayncnt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xsliyhtb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rngwcjhu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3bvwycmdy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ipozmmvx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qhxmhtyg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bluzkosg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3grzhyito.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gstblbof.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ejkljoyw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3elrqutwd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pmiedcsf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3eukmjiui.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wxhtkvqf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3whlfesyf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yrjykzkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbvlpiys.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3uakevbmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgkjzxyk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xkdnyiss.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tiueamvk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wupfzkyj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fwhinepr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mxpansva.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jjlnvqxs.html

);
来源：http://www.52xcode.cn/Article/details/gt3ywyytvdo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hwqocaeg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lxhlcmzy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uzqqcdvl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gqgokdao.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3fpkvsmsx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3nqfeadxr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zfdrozwn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3lxocoqzn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tjrayxia.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3itqfevmp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rfvmklfr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bdarcwze.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3npygxtyl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jgdjlsxw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xoeedgmj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dwglqrpx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pqzuxwmg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mtvuvamc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pzjviwor.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dachqfjv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ivrhpfkw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3panbokyi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iexkwijb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3azlokejv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vnelrkbu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wstnxtat.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xhgnaqcd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3pffrsbyn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zjgypltv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wasklpft.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wencpurs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xhokbnew.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rcefrewo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3stbffpsp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xskhryne.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hlyuvofu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbulyxgu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tqmdxobr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bouyvrys.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bimrugcp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zaitcwcw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pcykhqki.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3dobbkimd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3doqleagh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vlcqwuey.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gbsusisu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3yqmujnct.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fcxulcdz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3visbwtlc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3aaoxzwey.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dyypdarz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3emxkqjof.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zyuqnkig.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ncauurfg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nszmemiz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3efsvmxtw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctaitxcg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ocvhmknp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3elbeuobl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vrcupzop.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fhhrlncv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cwdjiqdf.html


<!-- 参考信息 -->