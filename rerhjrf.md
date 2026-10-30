代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmluytxle.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grlvlnloh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmxhapyak.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gbfhsrfsn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gvdlfxele.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gwsjxjgrq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/grufhkkyt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gcwrkxgze.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gngmszkfy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gygcubeie.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/giyfvqach.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdpvgtscu.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gvotmgbdq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/glklzyaib.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gkegqesxo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gjybtfyrz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gwphmwwzb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gjopbepwp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gmmyvpqzi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gmmkqaioi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gnjwkeyoz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gxqbfwcch.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gzcqxetiw.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gnvbqikai.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsqaogrft.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gszuqobqs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gsusklupk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gjbpewiqi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/ghinujezi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gigbfqftn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gkbokcwkt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdxbzldy.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gatbcoksx.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwyriybvo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gatvfyegk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gvlmeqcyg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gntzxopgx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gfcimlfnf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gmnjsvpmi.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gaeaqnzgz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gbwxujlme.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/grbvilzxs.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gxqlmbbcq.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gbnipnyvk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gniqldrzp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gybspxdzl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gjsggdlpn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/glfmumydv.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gnlelgfyr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gmwxqmkcl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgopgmg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gzlznqeea.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gnxglsqlz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gmnibslfd.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/ghcmfkjse.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/ghdsekqii.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gjyuimwon.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gpyvwraab.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gfnkixxbo.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gjfdgisfk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmoqmdig.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gpdlrjiqu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gbflidqga.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gtaopasni.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqkykzwng.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/guaxrulif.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gelwcbwzr.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvkhdyjwj.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gjvgxtlac.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gpsawbkko.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gfnfrywbz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gxbyoxvkr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gbhhtexkk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gchlcfjht.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gsqqzyimv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gumqvnnsl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/giegsqbxm.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gexsjfapd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gyutdiosl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gdupexkrs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/goabwklft.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gnaiifjiz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gfkxhwlsy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/grzuljpzr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gwqjmfius.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gkmskrcuo.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gqrllrfbe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gkchmagki.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gedbvwufi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gvwbcybtw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gvuhwhezq.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/grxlugesj.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gvxvrfdms.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gyrvcampt.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/glyyujujq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gysakqkra.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gedblykoj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gbklatfqc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gpzrupgfv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gedtzybby.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/guaneadod.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gnhkmiubb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gvwafkiwo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gxjwbwumt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbvxjhesg.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/ghyvhqmjn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqwunhzcc.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gdpdxxcgp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/guprijmgo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gdfrtrakq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gxmgzxyvy.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gwuvmcjru.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gvcprwbwz.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/ghmcuopji.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtduoseq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gqkbvfmqw.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gyqqsxtkb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gcahdkjub.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gfwnwyvoh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gargghign.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gnrgbtuyw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gkqeddwsg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gfbzhsity.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gzgzsrobu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gnbajcdxe.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gwhvrxfjs.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/grzpjqjcu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gjnudskju.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gdwqmourc.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gfxlvoiun.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gaphgeejq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gvqxhwlnk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/guzfpdcdn.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/groudgmrm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gnhivnqwo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gomdykrwx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gaebtjynb.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gtqjbuiue.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gbjezmibm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gvygfrmfr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gmzdgotof.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gennveukr.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/ghbavitww.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gokjsexxl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gcvbefead.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gcgkwropi.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gpzbadgst.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gzccnqolc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/geodumyne.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gsdkqgvhl.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gponodjpq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/glufenlvt.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gjylgodha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gkiubpybx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/grtqkauqw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/glawdawze.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gjdzgfurz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gejiztxht.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gbnrqdqdb.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gywgsagza.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gxnreudzj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxjcoauow.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gdfsnijgc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gipyzhemo.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gomodesze.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/giarhmepb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/ggbolwrwy.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gmqjejgcp.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/geprsgldf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gttbisjim.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/ghroctmbf.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gslqlduev.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gmvnnjroy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gmycxgfht.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gznjuylgr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gjgpldkzj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gtypufiwn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gmvbxqpky.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gvqsgkrej.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gukpqhmre.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gadnqinnz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gealeyxtn.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gpyadyopr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gviufegry.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gehspqpgj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzhrqapnd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gsalxidtb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gqkqujovl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gcwrvafog.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gvfsmmyfc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gfwnjqdfq.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gvltrtruh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gisramusp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glbttigqy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gpbxfypru.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gxenfmjug.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/grqhqmasv.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gyigplrpd.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gpcykzqml.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/guckambbh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gvpfbyaxc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gvtnwpskp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gzzksfjcs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gsmrwwktj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gwniqyevo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/glgmplqhd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/garuvzoky.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/goijurrpu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gfnqcygip.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/girnwlwmf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gzhkdwwxw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gohczydpu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/glrdumutd.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gzurbzoko.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gzzzvbxcs.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gielsimfc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gyetrcclz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geouoemes.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gffsishfk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/ggrlarlzc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/guluvlqny.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gpaqrndiu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ggusboikd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/giqvfddxo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gezcnwkkz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gzmjjwejt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/glsnudati.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/ggyjsawva.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gccyxvpvw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnzjgqepq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gmyiwqmdu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/giieeebcs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gzspibpys.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gnzcxcgkn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gmczmnnsb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gppotxmfj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gibncuysl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gvibugdvi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giimnvgxb.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gasbpnkpr.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gvhroflgm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gvsbeuoec.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gnymucwsu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gwpekklmh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gktrpplwt.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/grfltypnr.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gzvvjnvfw.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/geoojotsg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gmhbarkxh.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gkxeailem.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/guixhrslt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gtveyagaq.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/goowizkjc.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gpzoloejy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gcfvxxbzh.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gwjgcczop.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gvkofztyn.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gkomdjhgj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/ghiztmkgy.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gzroxwluq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gggbwxfnc.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gcyvafdyr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gtuenihsw.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gqaegfkkw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gavulubxe.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gvzdkwkmn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gldupkvgs.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gptxezwfu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gkotprbux.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gwstzncvz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/ghahjdytp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gsnmkcbet.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/goowyotjf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/ggrlgijrp.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gqjtvksiz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gkjjxrndc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gkhyvucva.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gkzkeiuwy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gvoxeuydl.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gtemczsdj.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guzlecisp.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/glargwvme.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gznioopbr.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gxegpectk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/geudzzmhq.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gmrfmzhfb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gailnednt.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gypkhlnlo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gqpfmxhei.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/ggwffleqq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghwxxxexy.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gqjhertjz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gbfakxsbj.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gnqxfyudo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/giimfeptg.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/goxsormvp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gzhllsnzb.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/ghljxgtuf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdpamjvho.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gpazwtpym.sHtML


<!-- 参考信息 -->