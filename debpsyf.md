代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/goiohzlvz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grajvkllh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gruknohhb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvydzremr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogchqlrm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqivzlrmj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpybzzsi.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ggxbrqaqv.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gnsjavnak.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gnrgihdmm.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/giflkxwkz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/gowqgzaue.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fanxiaobao.xyz/Article/details/gognnohzl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdptkmcmv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwwxrcor.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwwayusj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspxzqrwh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fanxiaobao.xyz/Article/details/gthgueaty.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmutaqmx.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmpocbtj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxegaovl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrsanifr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gtrnhteui.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gjdyfgnlq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gswcvlwsw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goruzhmpa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/glfznygba.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmckmxkat.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjppkwkat.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxvshpbn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjmcyxrb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzessbuff.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjjmnhyl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gclqqchxi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqomympvr.sHtML

Ruby: a.gcd(b)
来源：http://baike.fanxiaobao.xyz/Article/details/ghhgnbuga.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdwvgqru.sHtML

[N06] 判断回文字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgpravzh.sHtML

Py:   s == s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gsqshraex.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymqgvfxu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/giqlepnlb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gmmqpytwp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnqsepwt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpylzjrfy.sHtML

Ruby: s == s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gmlemeoiq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gmddlcsst.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/gzxekwvct.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsneyxmc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fanxiaobao.xyz/Article/details/geeevuabe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoapwypy.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fanxiaobao.xyz/Article/details/gzysmloim.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcfckcwn.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyywfoch.sHtML

Ruby: // 手写 Hash
来源：http://baike.fanxiaobao.xyz/Article/details/gwutcxfha.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwulvpcw.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/ggotbbuxc.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gezsohnvj.sHtML

PHP:  // 手写递归交换
来源：http://3g.fanxiaobao.xyz/Article/details/gkwfhhfyn.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyaoovfr.sHtML

TS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/ghyxbxywj.sHtML

Java: // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gmubsmomu.sHtML

Go:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gpdnwloqo.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/giijdwfal.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepmhtypz.sHtML

[N09] 栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzclskmy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/goglkiama.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gnxvylfmg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggycgwaeu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/gczqttryt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/goknulwyc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gplcurtaa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gachpogqc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbannensu.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gouvsaaso.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fanxiaobao.xyz/Article/details/gxyjahmso.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gydjwfemj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gsohtdvqg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsxoeyff.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gajfhadjr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fanxiaobao.xyz/Article/details/guekqqcvz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gysxgfjjl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gexzixupk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeowtuoh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/ggsmjvdmv.sHtML

PHP:  // 手写递归函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfkyemqmi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeaghahl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhxzwmeu.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhafqsms.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gvjtdyahl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytavqshw.sHtML

C#:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geomrejvq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlpapigk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvqcrbww.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fanxiaobao.xyz/Article/details/gwqxdqogb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjnpvkqt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gwbxduqai.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gcunkfvcq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlwjmlbc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gcinrtlof.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gymmbizrh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxapvrdso.sHtML

O. 并发与异步
来源：http://blog.fanxiaobao.xyz/Article/details/geycgiyrr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcyrwrekc.sHtML

[O01] 启动一个线程
来源：http://mobile.fanxiaobao.xyz/Article/details/gamhpsnrp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/givubmwcl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdnxzmkk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnemdtki.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gugwpgvcy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaesgzqk.sHtML

Go:   go f()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxjrtrbu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlzycgfv.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwuxbmxf.sHtML

[O02] 使用线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gruoczshf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fanxiaobao.xyz/Article/details/gkdungrbq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctmrtmfu.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gxzjrefhp.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/glmpucqro.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbvogkyu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fanxiaobao.xyz/Article/details/gopuyfsce.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fanxiaobao.xyz/Article/details/gjsxisjzu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fanxiaobao.xyz/Article/details/gptzzbymq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fanxiaobao.xyz/Article/details/gppzecvic.sHtML

Py:   with lock: shared += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gbeifdazv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbaepcnm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/gpucikeie.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/grwlhuttn.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaqgrkxmq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlrefltd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxyetvpl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxgszwzw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqsdygld.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzlkpxvc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/gntqeuzis.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gltrleoqf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfqxjdbpq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/ggonrgmoe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbhfnmnh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/gchprwphb.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gdfafhibj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fanxiaobao.xyz/Article/details/gxjzimkcq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgmykcix.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/gnanmadfu.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjrgabrd.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gyjbwqidy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyypkezj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fanxiaobao.xyz/Article/details/gclmmegwr.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapxnfbdk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnhlbouq.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gktxvggva.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwpvbzge.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fanxiaobao.xyz/Article/details/glzxhnkdk.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiprtwut.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcimlfrsc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhjznrnq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlonctob.sHtML

Ruby: // fork 块
来源：http://www.share.fanxiaobao.xyz/Article/details/grdgqgdzk.sHtML

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/gphqedkno.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggznpwfvr.sHtML

P. 常用工具函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqxvjtth.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcfjxzsw.sHtML

[P01] 生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfspanmo.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gvsxsfjqc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/getwtgcuv.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnxqovai.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtccgvjut.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/giwzvgutn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmywmmrqx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gzfinnfrx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzwcabmv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzurswci.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fanxiaobao.xyz/Article/details/gcgksgpxb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glddcairv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gjfxkuyxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnodntzjo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/gyflmtlno.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqiwtus.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvjvcmkc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fanxiaobao.xyz/Article/details/gctpxataa.sHtML

[P03] 生成短随机字符串
来源：http://wap.fanxiaobao.xyz/Article/details/glreahknp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjjtudvd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/gnvqfybxb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gueoxlpcl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmtzymmm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaxqisvy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fanxiaobao.xyz/Article/details/grzoslulr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkxrsohx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fanxiaobao.xyz/Article/details/ganmojgch.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glpylxyir.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fanxiaobao.xyz/Article/details/gsemrjzng.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gecgmszxx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/grdnjjnjd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gecnihbkl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gsmtxrojb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gdratbhky.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/glyoefxkv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaxvjkrf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjfdlnlq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fanxiaobao.xyz/Article/details/ggvkqrxws.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgmijmor.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fanxiaobao.xyz/Article/details/gqykbfqjf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlvctvoy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/gsudofodf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsjlgmvl.sHtML

Ruby: a == b
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkaokjjd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflsgzhpn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gznfrskis.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/glzettlxf.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gixsybkiy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fanxiaobao.xyz/Article/details/glkccqmyk.sHtML

TS:   if (x == null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grqyzgcmd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdmhxseh.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfqfgoikc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiqkfqmh.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmynhpycy.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/gsshoepvs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fanxiaobao.xyz/Article/details/gsncighzl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gswaqffvs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhquxued.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjxwwkqkx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiwyiksk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgwodbid.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlioipgo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrhmgvrr.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/gobrgaxbv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhqemtfr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkcudkex.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/gttkybbsr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaykvpqik.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxdajqol.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gwjvmxeky.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoauknbz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gxoesiamc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfwnlnfyq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbezxxurd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzewxzzty.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/glywiilrc.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gqbbkskoy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxpxjdae.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gluzqntqa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdsywkcc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqedhglt.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gwvuqxhss.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdhauumg.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/gdbxexekv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gohuiebej.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnuqcjsb.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylocqcon.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfuvytmx.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gywskqaka.sHtML

[Q03] 增加列
来源：http://3g.fanxiaobao.xyz/Article/details/gpwqmuzqd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsojrxsc.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ggszmplii.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gfmwdptiv.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwomteokp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjewmocu.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhcxreaj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjuseytz.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffrmlfbb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscooecwe.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gpwqbudri.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gcaujpqqm.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcseledb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geprnumuy.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvfpdelj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gfewjouuy.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/ggogqbaix.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwhrefsa.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gadwrixur.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/ghmgfdwdr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzddjhii.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gbcgigeon.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gsgwlglto.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjtdflcn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnsqqglb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gpblogxmd.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gogcazbob.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstyqsgkx.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gbmpuybrh.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsouefrdw.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmsqjavik.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhgfshrx.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gystmftnu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoxosyvj.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gifjknkhi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwshpufzq.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrrvsmao.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggbzmdgeb.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/giraiabsc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvrldfib.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqojwzfzq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezbkautm.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gbakvpyby.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcejjndoh.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gghxvvmrk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gebporavm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiryaoyk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpmrtzmj.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gennwlgdv.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glbmvlybu.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/giqdajipm.sHtML


<!-- 参考信息 -->