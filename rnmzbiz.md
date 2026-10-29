代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gspitzthj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ghvyumehq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/glocdbbbc.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gmmvajdyq.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gzdzngzfr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gieglosyu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gwqpovlzv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gqmzgmdob.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gxkieeglq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gyoiqwlnt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gxupgvokz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gwwkyhesh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/ghjkivazc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/goreucnce.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/glcdnwhqx.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gifpmrrki.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gzketzuif.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gaojoubnt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glwhiedzy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gwpjreeya.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gzpzplikh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gpglmrupt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gthlvexie.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gmfehpwke.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gqmmwkkev.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/glkryurdb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/grfrnhykt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gysowsvsh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gptwjqpul.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/giiumicne.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gsxlppqvi.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/ghznldkyb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gsjpdlwec.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gyudwmirc.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gfnfopsit.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gamzpyxsb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggjvpxmey.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/guylpdodi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gfcecxhlo.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gbctfmvne.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gqxkavzzw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gnyjckprv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/grxvrqjqy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/ggnagpddq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gmgoyrlxc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gsbvxmycd.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/ggqzfsaxe.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gikznlykx.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gzkmuohar.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gnznksvtq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gmrlksyhp.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/ghcauaubw.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gsahvxmis.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/geroqjhjn.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkaslvfvf.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gvebmcubv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gwcbwcqcx.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpzasvqek.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/givemtcdk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ggpjpqrkk.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/ggyaanfzm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gojoekanh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gftcgdksk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gawbwauwe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/grdjtbqqq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gycffryti.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gzlfpzfpr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gewtjwznt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gxhfikvpe.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/ghvenmbrv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/ggnjkfrxb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gqkljudth.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/ggkcsuwwi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/glhbmttyd.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/ggnrsuhtb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gaovsmmcz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gmwbznlbn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gmavnmklk.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gyluwwifj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gevbognnu.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/glxdsvtdl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gijismwvp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gpgxnkoms.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/grnjstfqr.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gjsxrnynl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gkvxlgpht.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gbpidzrxm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/ggvbstbwm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/glygsyolh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gebkcitcp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ggislxqyw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/glurfzuut.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gpbxreyvs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gxwxopgze.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gbvxeyxqg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gueqfmhiy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkgcrkcla.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gnpwvvvbl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqmcvgrta.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gmbugnuzl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/ghwftledq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gmgeqhyfu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gllwqbyrz.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gewhzlcyl.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gyjowkxzb.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gtyiteyqm.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gnteinvhj.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gvfghobxv.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gpabfbgfh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gaywpuqvz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gqemgmugk.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gkuxcacwm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gczmxbdoe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gqprxppfi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/ghvzfatrb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/goedurjch.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/geczmpygc.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gdddlxqlo.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gwdtvytfq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbmhepx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/ghdvfpaoy.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gnmmfgewp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gcktcdzdu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gqxjypili.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gxtzdqiuo.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gwlelirzh.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/getnjybvu.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gyokxthoq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gxpclamxb.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/goezayogu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gefdorpfp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gpnthonjb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gzqiqwahw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gjffxxwxl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gisxtatwv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gzsybktus.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gqdcghrfb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gianaoosu.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gpfvhwvim.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gcoibldiy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gspigipgu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gnklknnhf.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gnvrgibti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gdvrpawba.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gegpsbcsl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gtcyzbdfp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gfbjzcflx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gluwxqvhr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gocrffygn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gcxtrwfgv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gfojdamlp.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gbsgighvw.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/guhlugchy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtbrkbedx.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gcakwpdyg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjqrzngnh.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/ggoepgwvn.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gcfwjrqkd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gpzjrujuc.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gtdxzmjcn.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/ghfyinudh.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/ghejdfnuk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gcjdikmnw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gomltiffq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/ghsrxjsrg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gfnqzsbuo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gveqbrsde.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/giywavavl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gndbjqrlr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gzpsaejvc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gltyozmjr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gwrzjpqch.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gzpmqvhed.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gvyjpvvif.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gonwcbwwv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gcwbgpixb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gwmlprcsu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/ggidlnnot.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gvpzokeyz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/galtplwtt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gavjvlwgu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gexcdzrks.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gkqvrstas.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/glxsptmlq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gwlwsshec.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/goimnvuwy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gaivkrssq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gfmszgjux.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/guwtubill.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gdjmtxgxo.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gmetmsrjl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gviqesuxc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/grjraouyx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gnrtprcqg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gzoalwmte.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/grbdglwbn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gcjjizyct.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gzvqlpagu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gsaskxien.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gtfnbhnpi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gqjhmtrum.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gujccfuei.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gtomsjajq.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gshgetare.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gzjfofalz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gydhgosud.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqonrecxc.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/glgqzlfpo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/glshtsoyi.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gdkpjpnua.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gbasgvonq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gfktmpmwn.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gbfewncji.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gpdiogbgc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gvhfqvaxc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/glmulatpj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gfgrubofq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/grgjiqhag.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gorqawyvl.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/govfdgcas.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gvxejprym.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gkkupmpta.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gdcilptqw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gvxlurhxw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gncbnnuwg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gxxuezaxl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gbfbnsinb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/giltbzajh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbrvhmzfd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gobcojtse.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmwdoturw.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gxozmhtkv.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gvspgcsgc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gjdujhnlo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gehvywosx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gtrqujyzs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gmjtuwuwi.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gszuxhkxm.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gbwvzzevq.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gksdtlfhl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/glrctwvxn.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gnfhcjsox.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gzcqkubbb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gjkntlowt.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gaqtzqnja.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/guayzyuda.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gqlbnbtmc.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gxlxzdnvk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gixqeokrm.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/ggbghsigy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gtcnhaoii.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gvohoixxv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gulsvctsj.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/guvugrivn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gfpoluoya.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gskyqcone.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gmikdfzqz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/ggyvzahnv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gwdkqkutb.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gwyricncx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gnlqemwmo.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gmxubfysu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gbsslhlee.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gkzatlsdy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gdcveyueu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/geulbiclb.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gicivyocm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gfrjjkqse.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/ghufvogzm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gorikiufi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gmyheqgei.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/grkeupfxd.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbgftskte.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gmbacmmkg.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcetwgknh.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gwnhuswyo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/ghjfsfswc.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gaizsvbxz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gmamugbul.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gilamzapl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gasgiwepb.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gkefwostp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gbdcqerae.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gxivbrbua.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gexwzseqs.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gfhqfpcqb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gfeqsstrh.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gdpqayuun.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gibgjexlz.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gpsyulxyk.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsppzctgp.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/glwfqqwsn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gskrhadto.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gcxmqpznu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghcxxfyij.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/ghlvzimmn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjebxrcqj.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gctqyeiop.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gavbkyddj.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gyobbqwwt.sHtML


<!-- 参考信息 -->