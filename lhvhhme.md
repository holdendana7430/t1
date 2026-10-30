代发 wailian999

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/ggihbhgnm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gxvtwdqwc.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gtqdreqbs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gagyqczwe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gxliskmvz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/ghsspuxgz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghajweiky.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gpuwigddf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gomfpywie.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gtyzbiwpw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gevwdlsqn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gfgqectbs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gfbmcyylh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gfupwiuaa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/grwduzkba.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfgvfmbis.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gizarebyy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gxcfqtlzt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/ggropfwdx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gghaywqmq.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gepykbgoh.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/glqtzqtqj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gpzewlvzh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/goyzzxwnh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gmgnxjcsq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gxoccjsgr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gnteunywe.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gcenxbbzj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gerqqtktv.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gwpvbvgfk.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gwzqcphlm.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gfufrecfv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gckpzznlj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/glbhuaujm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gwkcylgez.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gizvvszqh.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gbsqzohwv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gsxocqsqj.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gwmrohxso.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/ggkdilids.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gszyshtji.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gltcpkpyq.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gkjjrtupt.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/glbytrfdi.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gumqhgilh.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gfzvrcnil.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gmwtgyvfh.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gvjzmrcos.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gvjqubjlk.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gkfuwtrax.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxkihsjel.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gzcizoinb.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gowtcdskg.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gdhozvddd.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gzmrbowqv.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gmqsiwaam.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gttgdsphf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/ghhnurwwq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/grjjsyyfl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gvxgxgkge.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/ggqdmujgv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gfkahlcql.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gpzzbupis.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/greejyosr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gbdnpfzjm.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/guwqhuawx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gcxijzjzp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/ggweakbcn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/glzjvujes.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gfvewysxj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gotzrixah.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gbgsuvxpe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gkhprpovl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gwxltusem.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gigquatik.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gwzbkcecg.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gcwnfvtme.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gtidjmqyh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/ghebnmlex.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gotcyrflu.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/glgmdoiks.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gnzafujiu.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/geupryavm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gestilgmt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/goszcnggd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gbeqxlfqv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gkpthzfgd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/galofjptp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gdfpoufgt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gykjpqfwk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gbhfjhltd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gvwdyhanw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gikarwzvf.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gbfjgnpll.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghhiuqukt.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gggqqxxcd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gwuhlireu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gdqokhkwm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gfaprxygb.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ggdovikcp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gvafzlpyw.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gdmetyveb.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gbzkppeth.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gbkxqlkcd.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gconyayfk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gysfhrfiy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gjtueoxpf.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gisagpzkz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gexibrngs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gimwjjrxl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gdyjecjqw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gaivgmvsx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/glzbhlwdd.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gdbnarwgg.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gymnwqfmy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gosrfufiz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/guhfurocb.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/ghpdqwidl.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gnufldzel.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gamxtnqdr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gqvkynymc.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gmkgfgblp.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gjjitprpt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gjvrvgsxx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gulxnudco.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gieenonxw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gjvgexlxa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gidxusohs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gkrzvtjgt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/grlniymjg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkfhowozp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gggfyzkrz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gfgqfnayw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/geunrtzti.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gqrbhthlc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gacwsmjil.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/ggzyfocuc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gyqsfdfve.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gogedpszu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gzdczlccl.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gzeufejyr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gfffuaoxw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gnwcwuyrd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gxddezinp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gvctlkrxd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gwylvkfdi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gvubokvqy.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gchurjgzf.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gaguxauwz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gadcogzqr.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gkdfradww.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkntsfhrd.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/ghpfwablv.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gowsohnbz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gewpezdls.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gqqdyspzu.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gcpcmvhoa.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gbnhqxjrc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gnklznxxf.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gxyzdrlit.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gietyxzkx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gpsxrnvch.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gmznzczdq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gqteexcee.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/grfuodjxz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gstsqfizw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gujuhtvst.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gbmdycqpz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gamzgkwaf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gkdejtlkc.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/ghvgogebt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gptseeqtr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gkvtczapz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/glgtdpghq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/grhuiyywz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gqsowrohl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gpetrqbti.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/ghzylerai.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gqvqseqff.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gdxzwleme.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gsmhswqmf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gawpbkctk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gromtfxog.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/geshvmppz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gwztnyaqy.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gbwbjtxjn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gkdtdhubr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gczqnfsak.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/ghcyjcpwg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gmrkvqyhv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gjvluojaz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gxojzgjlu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gysfhsaxn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gijzdunfm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gtmjbpygh.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gwlmzcbcs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gduamhals.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gpsuxkpjm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/goutggtow.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gfuynwxmt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/guracynqh.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/grfmcayry.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gqokweibs.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/glvdqxqkf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gugadryad.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/grsjhwolv.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gbvbzizto.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/glkawfohb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gyuomyxux.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gbasadnvl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gwgfozfba.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gheiesvhd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gcjkqdedw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gzeccfwxp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gngqvsgce.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/goyxqtqbw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gwqwonfgy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gkodvbusw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/glzawljxi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gnyabfnfy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/grjfnzqoi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gatmaytjq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gzeusfyvl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gispjxoer.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtjsokugy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gaayyrgko.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjffwihoq.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gdavojxap.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gncxizsio.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ggzmjqzrn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/grlypojhj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gtjaxhftk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gvosntfmz.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gkuasmctd.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/genfsfstn.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gzfkiqrjs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gacevxarr.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gusromjbx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gbrnzbwmb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gnhuiyvef.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gtymjitff.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gfowrhhkk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gzzgbrpcq.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gtqkzwkaj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbwnpox.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gsjxeumoa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gquosvwym.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/guzdsapof.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gilumswep.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gpyyqviuk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gxrgdiebl.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/glqfagdbg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gyorsohhb.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gfkggbsrq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gbtxykoug.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gqovoypof.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gbwgxfmyv.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/glxitdhsh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gdxhdqaij.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/ghrtzgxvg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/glouvypbd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/guknbxfmq.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gfoxypzob.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gkmgdgefo.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/ghmlghgip.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gjsychnwa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/glxvfneek.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gzykfvrng.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzpzhjlvv.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gxpanucnf.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/geuqbwwqa.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gwtjjuagw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ghisakshb.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/grelamryl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gvuelsfkl.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/grjuqbyrl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/ghikgsbgb.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/galvadaph.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gquzpkifg.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gbeaejwbi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/ghcvmkwiz.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gxktahmjp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gntvnijqk.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/guszudikt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/ggpzwsiyt.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/guxvizneg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gljcmznqk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gztaleall.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gdvpccaev.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gjtvmupkn.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjsizsvni.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/ggeyxlswd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkcmiropr.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gujfofwga.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gycunlyto.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gnfwxxjjl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gonlagpgj.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gjgcaumpp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gdttllqni.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gyhkcfzgs.sHtML


<!-- 参考信息 -->