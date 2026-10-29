代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxboygyev.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gbjxfcxtp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gzudkzsnt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gdkdofyxw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gvqstdipo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gcflglswv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gurbqrolv.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gcjuobntb.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gxybzqmbp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gahtntjvs.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gjeokgyqw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gvyourfpv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gkqdgunjc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gqlhaolgo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gyrvqgvsj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gdouffxea.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gomrztumy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gwuvspwqd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gdzypvanj.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gyfitbado.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ghphiwoai.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ghznmiwui.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gtwjnvymu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gljbdwled.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqoaryad.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/ggpslvsuf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gehsvhwda.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gozlirlvo.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gnisybnyi.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gjkfjgars.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gowdwtaul.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gnppbqqsc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gyvmvgjqu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gsmbpsoyo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gcgzxqdka.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/ginhturpk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gvsmnucgc.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gimaaethq.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gsijijhmf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gdwgeeuvn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/glogicdcz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gtexmwnol.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gxkpcohne.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/grljxpusg.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gyycvgoff.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/ggkyqnzvu.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gaeujbqeg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gmlklqyfi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/ghunoyeww.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gtcioyuzp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gsgikjqzq.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gnxskptas.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gxyxhpfyo.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gaqvypewi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gknzduoyb.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gkuwdzrli.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gwnwtjdqy.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gwykybnwk.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gegtdzloz.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gulrhztok.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghsprwhyo.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gapvikxpm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gfukkjwkg.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gweewkkzu.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/ggyxrbxvb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gqwxvvzhn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/geeegwdil.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ggbihohxj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gajejzscz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gdzrxnmyp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gznbprpap.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/giscuolyt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/glqbxovcp.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gxlpuqdpv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gdeivamhx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gzoyocotg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gnlrncqvs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gsnmdchap.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gbibwdmcc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gyanssngq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gnjevjjxt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gzhzvcypj.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gzgphrhdx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gvxcpvpcp.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gddyielwe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gxmoumudd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gtklysatx.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfsshxxwc.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gomjyamqk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gktvqacir.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gydbviaxo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/glpqhgjzl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gzdzhieid.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gddkmgtjn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gsphymxdb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gbqvjfsod.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/geqfihqzy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gpsdizxcu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gqwtadbxi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gygkkkwfl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqoxtxlpg.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gjuskkbow.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnooffcqi.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gzkpaczyp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gantuceyd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gncglclmt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gkujdezsc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gtgqvkmsh.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gyegzdftq.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gpqtqtoyv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gluccpbbj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gzxbizjfp.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/ghqljxokb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gsknzgqqn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gntyquxlf.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/ghzgjguvf.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gzncisqgj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/ggnikoazo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gngjayezs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gmxaeblce.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gdjmnxjdz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gaxnoxlnp.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gjfjnybrs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gepifsvsi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gnwlqlcdu.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gfvmblffz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/grvklhqop.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gesqhtepw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gfcqogmww.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/glzqcggvw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gupufdwrk.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/ggxzbuuht.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gtouukbwb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/ghsuwssid.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gxottmnlc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gmaqgsepm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gkjkcnzyu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gdspuyrjk.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gxaxcdcle.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gfwndoggi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gqntzgbag.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gtrcuxrfs.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gbhxzdgiv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ghbszwjsw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/getgvdryf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gmxgfkflh.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gtjmmgfsx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/ghqmrjzcn.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gjlckmgce.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gfmblykvh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gmdwvyrrk.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gjhwqkvft.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gdscoxoli.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gmcmsswlq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gzyjbuitu.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gelxetare.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gyvybtigm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbyudpdsg.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gmoxrgehm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gquebfmjp.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gamytogun.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gcwfwwdpz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gpkqpogfj.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gsgjfvtjr.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gbbpyqnuu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gwpgbhhyc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gxdrxaacx.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gealxqlrq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gcvxursdo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gesicddpk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gnhfzgvoj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gcajpmvun.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gltvwqupp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gpengdgod.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gcoocwoyx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gxecxhpxl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gyznznymq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/ghcvuuisw.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpttaqo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gffmevnon.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gzobustkz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gsxpuyisd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gexrbnrtr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gnranctev.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gsjkugrco.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gmumvcklf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gopqlsncw.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gcvucigcg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gapylxntv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gxwsznpvy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gbcudbaze.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/ghndmtghe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ghruwfyjd.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/ghbzvrzec.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gjynwxaju.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gfixhxere.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/ghxjzqoic.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gcwbzrjyc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gcolyyndz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/ghxtdvjmv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gnbymwnrz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/ghxjjntqu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrhxbydh.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/guntiietx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gvhqjtmra.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gdrzsdnvi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gyqozabuw.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gcsjyvhcm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gywmehnka.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gphanbufm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gtcqwguxr.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gbjmmzxsj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gxttpocbd.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gshvtpmgv.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gzdbwqqqx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gvwbrghmx.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/grjqyzrrc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/govazzjip.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gizwqqcqr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/ghwlvzqte.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gaqlqldwm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/ghaoliooz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gfufhathj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/grlbxmaiz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gowbthyyt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gwcturrfp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gavzaukgy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gzdtnrfpq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gpgbucgwq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gzmxvjfgp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gxgjyqsye.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gygmdywjj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giecwttct.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gooikxhye.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/golxcjawe.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gerytstqb.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/glybhjjtw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/goybxealf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gowclkelx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gluzkqdey.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gddypiqhq.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gyawplnrb.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/ggpcjfvno.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gojefvtps.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/guzmnnxqf.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gxedhzkxz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gdtottvzt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/ghnxyjobt.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gcadnwejo.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gxxkfbpux.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gqqyqnwvw.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gkyxlsyba.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/guleleprv.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/guacgsiev.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gtqvdehlz.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/girjhxiyx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/glwlpxwls.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gqfezgzaa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gmraohbah.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gwvdnboas.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/glovhwmfg.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gwqfqwdvs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/grdwfkkle.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gpyqawirw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gfnqmhcta.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/glwhqvqci.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gcqxmeydp.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/geiqvwlte.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gqhjelmeg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gpzyyxprt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gbzinwewn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gnvohgxbm.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/ggopoxemn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gmjdstgxs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gpwbwaxkx.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/glepflffv.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdmyoygfr.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gukeqpskw.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gyinipygs.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gwikizkpg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/guuvfgscb.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gwezaflsz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/garscrjau.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gbbnkjyrd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gtdhrvljc.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gyzrjheri.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gvzvbikad.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gcuffxhvc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gaphtlvww.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gioksulsq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gekxgmysv.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gcnommksp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gsnlildpq.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gujzvphhl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjvipkcie.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gsivopgwv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gxryshjrj.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gxewewgav.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmndcvgwd.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gyljfsteu.sHtML


<!-- 参考信息 -->