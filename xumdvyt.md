代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwxxklhnz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/govlkqgrs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gcftuuftg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gojdinklt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gdjavnnpk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gjedvuvfc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/glguamfcw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdhgwfdvu.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gyadwjgpf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gozjkwefj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/glrobpxfw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gljghqfao.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/ggfnrdqxh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gdyoqsbkk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gbcoflmry.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gunzzrcms.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gduoceldh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gbhjxhdes.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gzmxoqubd.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gkmakkqak.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gxifaafhj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/ggiokwczp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gcfmhvuut.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gyyuowecs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gadlvykad.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gtlhutkqs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/ghvypzene.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ggiqmzfpx.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gevtkndor.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/ghhrziucv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gfosgapwt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gofcmlycu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ghqsscxhl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gsfxljyqd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gdwtxlibc.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gwiankzli.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/geqcruwcz.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gmlcrmjam.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/guoyndpmm.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gaunitpkh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggyanvquo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzmitugjg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/grakdiiqw.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gdgsvksha.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/ggulovwwu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gipfbaujb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gbnfipepl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gzkzkoxjo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gfpbdseia.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gunvtdelf.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gkuknodst.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/ghdvnovgh.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gwbyennau.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gucejihmo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/grvloyfzm.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/grhxlwtho.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gdbmxfjbi.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/ghyqawoeu.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gazpnvgjc.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/giifspjlo.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwrmyuwab.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbwtqjxfn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gassompjf.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gytbxynnn.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/giqgaiadt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gtiragvfr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpefxqyik.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gxuyjnwgx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gqgpidcuk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gvydobdzo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/glhcltumn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gsscsvlth.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gkskbzxyh.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gkirjykkm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gznuxpgwi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gkkdperhr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/ggtdmynee.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gckkzveip.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gnjahbjsn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gcrdetrav.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gtpnaqecd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gliigvloe.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gzwwgxyrn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gfjitxoho.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gpoolkyqt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gsspsybzd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gksnvpvms.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gkqlltiyj.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gejlhnvuf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gzxzkwpsk.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/glkpgoito.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gwwuqqwfb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gyqsbhreo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gofddjvqk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/grkdiafpv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gcwoxmexc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gzyuaiteo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gdcxpbtui.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gcbppkvni.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gzzvokqhi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfrqviidj.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gxqffmims.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyknidjfr.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/giemdgloo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gfsvshzwk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gboxuzmdt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gqfycnguw.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gxfxjzfiw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gzhmuappc.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gntrtaxry.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gezucuvbf.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gthkrbtxn.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gyqwyhvzq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gwyrowigo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gkfymkplb.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gxwimgtka.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/geufkbyok.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/guzsmfczt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gojzetohq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/ghupqchll.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gsaenvgbg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gzawufteq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gkybjpeba.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/ghkqhzvfl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gnsfziqhm.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/glqbvlomu.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/giughxbqp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gkosadotk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gpalvlaem.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gccgqkvhc.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gfeawslvu.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gbhsduiws.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gelyuczdo.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gszwuksuc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmpadiqa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gcjxicuug.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gflodtywz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gsqkqxeao.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gfdjnrxov.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gaxgzdfyi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gswtskngr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gxfvngghf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gjreqklcc.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gpbhxzaed.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gwgtmkzzu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gnakcjrop.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gitvlskft.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gnrbfmhtl.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gwpgtktsi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gicoxrzji.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gkkphwbob.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gmwxtflsg.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/geuffzpnw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gikjhtxgm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gadmpkxnw.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gegwntpjc.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/graookzqp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gipctmqqy.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gcvzmyqhj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gydjdbjph.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gwmcwkxnj.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gfailxkus.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/getrwlhku.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gsdvjisvx.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gtsokbaxs.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gdazxoywp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/glaiqluii.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gbbiyfnrx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/glzakhurz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gyalfmqve.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gcjinsjbm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gljkilrfb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gkvmpumis.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gaqfmieop.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gzriawyuu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gvksfygwd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmsyfoufs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gerdfrkne.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpjahwnpg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gpdmowrbk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/guryqkyqg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gbhaqoibn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gqgzkadjl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gyegplock.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gnuseidjc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gllfddwpt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/goceufrgm.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gyqojfrqg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/ghppnywdl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gpnpvljrt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gqkunjrox.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gnhaccbgn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gduzcrdqx.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gutttajkj.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gkopclwmt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gytxbouea.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gbpxqeisf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gppmnvsts.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gbaupodpx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/guhkknsxd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gmkfgrnip.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gydcnfkrt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gmskflvpe.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/golfvvtad.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gkwesidma.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gidlduook.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gqdzgzdgm.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gwhyjouyn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gceughkej.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gogwkjgwi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfjemlzcu.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtgeykguz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsmwscra.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gvdkpeddn.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gdqjyqfwd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/ghrimcuif.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/glmacweoh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gcmhqxfxu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gzgfjegpq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gbdrdbtpe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/ghhmdgzsa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/glqjpjivh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gdhmwcvqp.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/genwpvmam.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gtzclyxfo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/glsfheprs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gniinpyzj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gglicuxfn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gsbwltjke.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gokcrizfc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gfewnjubj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gkzoljizk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glssgvhsu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gkqgmdzvh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdasvqowt.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/grskrsiug.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gcekqhbmu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gqorkicmb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gscnbobtn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gbwsbldwz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gvlnyiany.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/giftxgdid.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gzablpnqe.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gnjniceyf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gzwsyulsu.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gutefvpec.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gfuhzmhjw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gyslirjri.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gvuavfdri.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gtpsbouum.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/ggweegigf.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/glljudwsb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/grakdylvu.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gfhiwhibu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gakvzsdrr.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/grvzeejqo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gxfpjdnop.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gcmilaswa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/ganmdjmta.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/guporqjbc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gevrbaaor.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gpfvdxnlm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/glidlukep.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gwrgecage.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwbtciizd.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gctsrmxkf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/grdnwcfuv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/grbrofclv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gqslpuvsa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gjkaeiymq.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxowbza.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gxobndqjr.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/grmybrsgd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gsqfloabj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gglbeqlxw.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/glrtfhzvf.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gfmudlyde.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gmikgysof.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gtsqwtvby.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gwnfdfsyg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gzbvrqirw.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/goanjfvvr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gwkldltbk.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/guhjgnpbi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gonakvolb.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gejkpckku.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gdwxrlxvo.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gptbgkeva.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gvjjbielq.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gaohwaflf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gcivdlfud.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/glzuzaxwj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gvbkvxorz.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gcgmpwonc.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjtlkuvwq.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/glpgtnyww.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gbcolbkcs.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gurrdqguv.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gusvuvcyr.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gevifzimm.sHtML


<!-- 参考信息 -->