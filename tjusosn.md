代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gmexplkjk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gcnxgkzfq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gyifinaot.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/giucxuvqd.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gwhroconf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gzwdhorry.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gtfywymmi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gtrinufcp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/ghahcfyut.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gumyueyvt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gkzgebrko.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/giskulpam.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/giahvrwej.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gzcuxwsls.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gcuhtdyqn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gwixmoplu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/grzcuweor.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrlkmxbn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gbtbwgoau.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdwkzypmg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gslezwjze.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gykddpbjl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gxbwzchtn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gpccweudq.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/glbiluiko.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gtzcosoil.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gmwytmfxf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gsdcrblii.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gerpnnyho.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gjzxyouty.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/geeivyokd.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/ghkoxjegv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gftqnbzvj.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gfavvsccc.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxfygddlf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gfpamgrsu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtouyvzkj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gttjfvwlr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gielakdwa.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gthhfvhll.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gpgzctagz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/geuotthaj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gnfmwssus.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gmcvaocpa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gzlwmocmq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/guivxojof.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gdvhhvtdv.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gjinoffgq.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gaqujnwzh.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gmxqsezfe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/ggjrnilzu.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gzdzhroai.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gzdhpjytm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/goxelmbjl.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjyjvwlfr.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/glpixfwzq.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gftjvbfun.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzrtwqnlt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/grvfwxvrh.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwikaktga.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gkxkvilgo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gizqliddu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gbgzfuoho.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gkkoqludo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/glmiwllri.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gtgnchrkb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gfjvhmrlm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gbpmeshyy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gvqnvcwlf.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gbqumkvlr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gdaieeccw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gxwvqykrp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gneglyqjl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gdpalsjjb.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/grjxqqxwm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gkfaewysi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/ghxibkpyp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gntoenyln.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzlzsvkyl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/glxczhtke.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gosekpuen.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gmboiymhw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gwqtkjurb.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gustvpiia.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gntgvkbeh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gbhcyazae.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gdedigzni.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gdfjdkijf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gwijwlwtq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gdnahudwh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gvqghlepp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gtndaecoh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/guenbzshn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gdocojbzo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gswobsmuc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/glsrhuwbw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gknhhyblg.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gvdcjkoap.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gerdufdxr.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gpvlzgugn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gfsjznmlu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gtbzqqhch.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gkyqvoidn.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvpmrowsk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gfhwolcnu.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gbojezfuk.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gvxqspcng.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gzcbyxwsg.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gijerxjkn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gvfkghqui.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gjuxmknnf.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gondbtyhv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gddvdqwrf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/glxgoajxs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gpdyanqmc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gxszdxxjs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/grbbcigwt.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gpfmprjkt.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gcakzsgsw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gwycqbkah.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gcgwkhyrj.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gtstiyuvn.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbirjngzz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gbozivijf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gdiyutzgx.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gptztmlzr.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/guadivmvu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gveqknwya.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gimutubwt.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/geilvitvp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gxzukrigz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gxyqrcsng.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/glnknanxp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/geprejtct.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gvtscupmd.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gtehzmcuq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gkvldfhux.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gcnqygtfn.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ggyiinxvp.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gjoabyjwj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gjxfvifeh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/ghxodvtyx.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gxsasjlnn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gyashwtmv.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gqgleavml.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gkkvxyjec.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gmvkgobip.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gibjuidmf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gtrqbyecr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gyhieqsmo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gmicbnmjw.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gjekmxtiq.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gdhttjjvo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxkuydcdo.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gofemsgch.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gukhcjyqb.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gfohrnejr.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gcqzmgbbn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gcwpqilmj.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gpraerbke.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gknkheppb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gaohqpgjf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gtahmixzo.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gyuyhlgyq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/glmidqqym.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gcrxwqrqd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gkprwppdu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gjscmcmov.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gphudjrrc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gxvbpoisd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gtthusvva.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gmqpgmptx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gqjbcgxpn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gnfzlywcp.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gekkkexey.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gsqhrtaay.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gfubpklju.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gvkpdbylc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gfpxefcwu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gwxkchlzw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gurzumnof.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gjvwkhhxz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gvepgdtuh.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/grgwywbye.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gmyyakdmk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gyusxlywg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gwfjcjxqn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gdiscumbt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/godihomgq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gkwezrnmu.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gtyhwoykz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gctwfmqyl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gmxgekwcu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gbfgsruaz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gnvfkebhb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gfynphpmn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/geernldbi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gyzhjbmku.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/grriqcoiy.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/guzwcyevl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/glsohchgy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gkhyufrvg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gidauspqs.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gnroeqgii.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gnlrzosgw.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/guwhfagcp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gvtgnjdls.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gwludugxt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/glcghjdck.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/glnkazibd.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gryzvyoim.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gcsmxvqtz.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gezmziisx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gbvragxtp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gngholguz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gmrghippn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gaqqyqoxa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gqethrlpc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/ggpcbdnbn.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gnmkfoomb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/ggzrosaxy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gnwszrwzg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gooszaxhw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gethitqoh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gphungogy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gcmsyvhej.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/goinyclzt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gedsjunvt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfqunluwp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gtummuint.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glvoxbtvz.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/ghimgskre.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gopbnwbsx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/geanmrfwr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gktyyoxew.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gdvpvvnbb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gsfunvgqi.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gkmculkzw.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/ghatzmvdi.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gbytaefzy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gxllqizql.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gxihrmitf.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gxliosuyn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gdqippkfs.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gfdwhwtsr.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gaioagcej.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/giftfcyfh.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ghlcqgltu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gyonrolsv.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/guzvmzdpk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/ghofnnahv.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gismmlwzw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/ggpjqvsnm.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gvhxwyqay.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gyfioxpoe.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gaemdfoax.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gszopijjh.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/grpxnscpi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gcidrctqp.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gotbjuvrd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gbynxjttc.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gtvvuijnt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gczkbdwrc.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/giqczujrk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gtbtxxglr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gsqhkryco.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gagffgtxh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gxfgiuhnn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gnaqygoio.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gebmefgcx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gytywkwtt.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/geyuoxrww.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdxogvyjs.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gmhnyeial.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geafkqzpn.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/goglnjiaf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gaknpqine.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gaitbbnqg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gobsihlgh.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/ggrkszrkd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gqpilnvvm.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gwxettexo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gvcubwckb.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gwgapzfkt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/getiifsmf.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gkvcoduqq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gjznwbqqb.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gqrlvhhsd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gwctbpiju.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/glfyccvxb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gypljoyig.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gzvtktiyj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/grbevlpwy.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gaudqiykx.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/grupmkdnt.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/glxbtldtp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjbmncorl.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gouctzrnw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdtswrxtf.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gvbdtyeae.sHtML


<!-- 参考信息 -->