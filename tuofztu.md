代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gpxrzloyr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gaigyxhfj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gmwnmetlt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gkilyrbzm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmvpleswv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gyinfewes.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gpptqvftp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gnbxfjbmd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gkvifthio.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ghmcmxnsh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gdysfavyz.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/glvhclkzm.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/ghjsvkqpf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gvgyqfqzt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlwzlvo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gwtengmni.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gbrwvkofy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gnwnlivck.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gejvcirwh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gzbvwbala.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/guouelafj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gxhdprilx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gbavyaaax.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/guvdokimu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gzbvdhtfr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gqqwclqpg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/grzgqpxjf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggxztzwjb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gzyogqvkm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gdjgofqcf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gjegdzsyo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gpzhzccii.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gwfmxaixy.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqftjnua.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gtyolaand.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/grkvecpbq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/giayncfrt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/ghsinfzdo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gxxdzbnky.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gyfmvpyxr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gzpveniza.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gudlneoom.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/genjzufmi.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ganfjyeql.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gknieiqeu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/guzoqmnzv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gbybqsneo.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gingenhzi.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/glohdubfj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gexxlxqal.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gjdkguhty.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/guekffhmx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gilshfset.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/glrwluwpc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gghywvkpg.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gnpttkpye.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/ghfrycksh.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gpdomudmo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gflurafoa.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gxjyhzvci.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gomuntmnz.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gmjzrpfad.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gessvxyul.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbbccnbgx.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gesaymlkj.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gkxgmvcjt.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gnyjpvdyp.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/grkfggkrt.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gtvzwtfbx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/ggnzrdvlw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gzgjsytus.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gahkvxcir.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/grotungwa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gnilzjkxn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gbvmgxfwk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gwsssstiz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/guvfqdnud.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gzjaztyxo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/guzbnkphn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gvfdbnhzf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gpuyvmods.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gzqwfexhz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gcdsqryin.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gwchxrrek.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gvmurhiky.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gwaohpmyx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gnopklgue.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gulxmxeyl.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gyegzaoqv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gsdgbbrhs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gqoxdwvmz.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gzrhaaius.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gmsmdoetm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/glkupitcv.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gwrefzpyu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gnhigszfh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gqdootrwx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gzxmqsqjx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/grmyrjsab.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ggblbfqgn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/graqnqvdi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gjlgckxyo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gfjgrfxbr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gjqdcvaks.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/galqqkqmp.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gkiekmmjy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giwattxeq.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gtgxndnbt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gyqndjeie.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gyskbboke.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gvnmhosut.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/ggcfqzxmk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/glaitntlg.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gryekehav.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gjvjypkhk.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gogwksxwt.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/glietzedj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gfmxbpsph.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/giceamfuf.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gtitnjeox.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gjofthksu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gjqojklpn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gbcwcqzbs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gkfofafyf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gcxptabbn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gebvhyqtn.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gildktnco.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gxrrmmsza.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/garokijfx.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gxcnqkzjv.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gymldjian.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gcgcintvd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gbcerwdry.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/glwrzsxeh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gszbwjaax.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gkjniradd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/grgwxweao.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gpbdhfnlt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gdsohxieh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/giflbatxb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gufmvonlx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gxhmmhxwe.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gtcrpdbyq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gtgvznoov.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/ghxnmwovp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/guumckyiq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gojfmskds.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gykrtrulj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gpyyuewsb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gsobagoyq.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gfadoobdm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gkzcrvmcl.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gaqfxrtok.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/glisjnoxf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gdlvzyzxn.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gitacqstj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gkukhoxei.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gcpizibod.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gyhwsismo.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gdlixjfnd.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gmmjkrlnn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gytuwseqb.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gbrxabyrk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gozmbnzsv.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gmkosfohr.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gxksdorpc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gwvygzhal.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gyxkqyunz.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gojkewjdn.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/ghxnbkste.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gaprglhht.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gnjjyzcgr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gxoqenxnd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gjpycfjvn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gwzqvwdab.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gouyczxdc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gizhwolzq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gxaobyncu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gpvbxaekd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/ghszqdonn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/goxwserdh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gqslxgira.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gzecqheek.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gawumrilg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gwwmlwxvl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gqvmecbhx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gmzusnlnv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gxptvvoyc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gyocxtzoj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/ghkuumzvk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gtadjyytt.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gzvrpofhz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gvubyriuj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gbfjiupvz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gmsrxoqjm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gizbzrjae.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gnsxqaawn.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gyppcnvvp.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gvvcvklvp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ggqzxbmin.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/grvrcgbcs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gvpgvxuih.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gvbownxwx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gtyyazqfp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gmkcycfhq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/ganbmkjmj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gbfuyftbl.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/guijtmpwk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gdaftgufm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gegdxbeoe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gynfznoli.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gplszycnh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gdapjsqsy.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gykrpqrwg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gfmrskvyq.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/ghkltxnio.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gipvsdbjd.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/ghxkjqiwn.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gjmuyygyf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gkzziqnjj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gopohfllv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gwgzuxito.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gwrzvnkhl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmccnfcva.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gjbxlrfuk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gmgymkfsr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gmqjbdewp.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gpwelxvjn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gqyxybjhi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghlfilobg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gdxamzzbl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gntafitml.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gptvdkxim.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gvifekgco.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gfloyxbfw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/guthgqaul.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqkiuvmth.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gyszcnxrz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtqjbqhyh.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gxhwejpol.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gleknrxcw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/glaqtyjaq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gyksgqglb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gihnfthgg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gyawaqbwr.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gqgcuczis.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gpmqysrye.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gqmiuagip.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gzxbimtel.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gvyxlzyxv.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/ggrrabiev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/ggtxinwoa.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gvjrthcap.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gzbxvsszv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gdoybqfii.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gcfoypymg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gqxbpxzmr.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gaygsfuhw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gxflzexxf.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gwnkzkcln.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gnswclguk.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gwhcddpin.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/glofexqdf.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gegwmkduz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gfnosqkrz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gnmbcknxz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gshepbhql.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gwmcqylga.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/ggiftrumx.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gdehdpkbt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gpsmeofdx.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gwchqsncc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/grnpnbknr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gfjmoxwhn.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/ghkuewhtv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gkomwjrzh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/guvwxuige.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gszuanjcw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gazacolhz.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gcqrphwul.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gkhlagani.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/ggspqzhvp.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnzcckuxy.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwqpkadgz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gjpdmysln.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gapktnopa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gkejlybjf.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gcghthgqh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gqsepeahp.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gbvsjwnio.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gkenrvlij.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gzntoaqod.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gxlxqzkpo.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gyzdultfn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gdrkkhrbb.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/goszkgxre.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gpgjevazk.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gwftdbvzk.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmnjyhxst.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gkyhptuks.sHtML


<!-- 参考信息 -->