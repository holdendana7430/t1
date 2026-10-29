代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gqslytcun.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gpjcwrhqq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gpmpnokni.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdnophgev.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gscmbhurz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gxphfnndz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gkzvvfxmv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gxdluefzh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gsbkmccrf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gayhxkpxx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gzvvinmak.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gkevjmzxv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gzsntosku.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gcjemzdeq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gwwtygqre.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gcfujwlcv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gjsmdnwiv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gemmvyqyo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzyynmvkl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/glujiblgl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gitkcylzk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gaqbedayd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/grkjogjkh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/geftbduwm.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gtzxkpecv.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gluvhxfft.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gzteatskj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjlemljih.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gujiuufve.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gcuuinfco.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gzbhbuxni.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gbmghtuse.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/glnrpwdvp.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grfzjnkvw.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/girscyxuf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gdovyccha.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghlxtqxbm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ghkzvirsv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gtjncbgbk.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/goelaygga.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gfiaysgdf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gwrlbxhpp.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gfdykjhbs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gjtbtlluq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gsrykhvem.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/ghxgghnhw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gfamwbumh.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gijvsilju.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gbzywqrcy.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gstjsunln.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/grrxftirm.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/geqgwfhwz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/geestiyml.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gyuvamfur.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gljevcqlp.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpundwtwy.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gvwvjuigx.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gyhjejell.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gitmllbyk.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/giioiplog.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gyxecfybc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gmrxhiugk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gdtpozptd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gidiijewf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/ghgecuioa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/glxpmzyrk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/glwkqnupa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gqvulmzfx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gwretytjt.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gjyshmxiq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gbovgzypm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gcesxuoua.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/guwaihtrm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gulkzlzkz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gfabuzduf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/ggoayzzzb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gmlrpcfzb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gbpbxwvzp.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ghwibouax.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/grthrigys.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gwaqgfini.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gedxtxlcg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gqwwkudes.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gsqipapfa.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gacvioodw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gisnqrxrq.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gafaluoeu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gecjzpdkv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gwjghfgne.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gycwuuxrt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ggliydwjg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gppkklrdy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gjxmgxrlw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gszgymjys.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gjjfhkvgk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gndlsyznu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggdmtqwyo.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/grtflvduh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzzmcgzdy.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gmbftrffo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gqxzaulzm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gufhsnpyn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gkjflznxy.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gpbarrvpe.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gtbjxznpr.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/guceytiwb.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gnflkbaro.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gyemecahf.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gexubwtqg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gyrbzqnca.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gfofglbse.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gtmwdghpq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/garmigdwp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gtewkoeuq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gobwwqtxz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/giadbjgdf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gpxrvnhdn.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gaypsyzba.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxnfhgq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gpwgatjcd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gynelavrl.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gjlocikky.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/guewkxtom.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/glaiqvjfw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gwcfhxaqa.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gfsxjlgoj.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gubahtsrz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gxxrputta.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gfqxhfbnf.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/grpznuikr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gtmwnqork.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gbdjygwjj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gwxxkzaoe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gohfinqkg.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gyfteycpv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/goitzxqov.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gkmcivzjp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gzcwpeess.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gztczbgxq.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gydxtgxgd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmdrrbrd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/guzecmfdg.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gdgzudasa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gnudowhyc.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/ggbellixe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gfbwguwsj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gqxkboqwh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/ggqhahdva.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gsazcfrbk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gtrmmreuo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gfddpgirq.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gpggnjpsp.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gsrhketut.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfohfxiax.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gjkigvftn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjdvrvvdg.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gqgpghjoj.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gffhzphfp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/guojujlaj.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gwpgkzxmy.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gepvfxjll.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gvvkxxnrx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gzdgbyjbl.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gpsywjvfh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gqbgqzmlj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gbogfzepz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/guuxcpqul.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/ggxawokmo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/grpihoyme.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gxmipboss.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gnoeixspj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gkwtqajlm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gorkdxabe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/glztpzywe.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gwtobjqns.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gfogbfcgb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gbkxyylst.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gxoexwpyk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gikvrjjle.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/grhjlkwoa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gwkhymnmo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gdiirwlai.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gjexavtxh.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/glivvthyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gstooxjfx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gktndnydm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gircpzyra.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfgdluipm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/ggosdqrki.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gvwfhoqxj.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gjclocrbs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gytwfjcky.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gfcfxhbuq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/ghibxgjsk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gcdchbxux.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gwbflrvoq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/ghxaabnzq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/ghmuylckl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/guhutmwrs.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gfeuinpdq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/golxjzbvz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gzrjxrntg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gknfdfyap.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gyfjsfbtb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/geikmhsuj.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gofxmvtzg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gtvchirwx.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gjwptjzot.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gvkopggpa.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gvleeoedo.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/glptqhdrn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gfenzvcyh.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gxuyfcdqj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gsufezwte.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gwbmscehi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzviumhqc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gzqwhjxfw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/griatkzyr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gjwvgqdsn.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gtjbpqaxm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gwnflekxh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gghficzyw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gicksmumo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gjbgkhsao.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gpfjywufj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gycwgrshk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gsqyeyjox.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gygwkcuvc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmzasyetc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gvnjvviio.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghixflvfk.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/grrtbfoyx.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gemswuepy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gmihkeyhg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gmdgvmrnx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gjpyipwrp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gdhowpgdl.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gqlaqkzgq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gelvlbfre.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gnobgovzd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gigkinyzm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/glaskgnou.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gzxvxagbc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gfeddhktt.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gabnozovl.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/ggiqtubhn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gkicfrheg.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/grqitoryu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/giowjldzx.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gsrcdivbt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdblvwj.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gjcciaodl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gorvbylhs.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/glqvzpyav.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gqyzjvkyc.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gcncrqybh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gigavhtqw.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gtnnwcnqo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gnrwdlpdr.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gvwrhikgl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gqcnnqaja.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gxtjlpujj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gfbgfbpnh.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gnbcawsqr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gepspruwi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gxhrcgnha.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/ggiqatyul.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gwpkvxnvi.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gcywthzmr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gphhfhhto.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gzujbhjwo.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gcgqxmcoc.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gsgmtngey.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gosyszsxg.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghyguzvfv.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gukteqfnt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gxmtlecbt.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/ghkgycwyk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gcxzjsfqq.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/govdjbdlf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gygjrycds.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/givdhfhma.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gprxdsjqb.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gpwfwucip.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gcjboxfqx.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gmwnugopz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/glbzgikro.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gebgedwya.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gsoxcssof.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gmiceonia.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghdbsjcsi.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gztvsaiki.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gdsarcktv.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/geqwpmhnm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gujidrdfn.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gzuijexua.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggzuidkan.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gthnflhyl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/guyavxxah.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gfjjqhlxd.sHtML


<!-- 参考信息 -->