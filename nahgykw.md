代发 wailian999

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/ggbtxcubs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gtjjxoavn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gieyoqsso.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gppmiechu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gfbzcctdt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gvwaddykm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gphqdyxzv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gzqubqaou.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gveflqwhv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gyiogxawr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/giiwimpde.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gpautfucy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gwjbudofz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/geiqivvst.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grjyacrvh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gwgedkzym.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gkuczxkck.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gwrhvqdnh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gpvcibfwv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gubmvgqhu.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gguvrxnie.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/grhyvaglg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gbmbsmwxs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gmpkizlde.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gywadwili.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gwbpdmcdv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gvxydyfvh.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gdbbosnup.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gmqxzdmiy.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gcmoxuvgg.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gpurruong.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gzwthtzaz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gkouxwowq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gbeapabqw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gmcsqmtzq.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/guluukbdg.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gfxhwzjgf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gdaxgbbpg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gzcarcgxq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gtwxvhdfb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gctlxnuai.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gucxtpmfy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gwulaiedm.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/glvgtydae.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gmuzkiqnq.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gxtrckzpr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/guqipyang.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gjwovrfns.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gmiazuxic.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/grrcgsqqp.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gfrmbjzvn.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfjsjtbci.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/giuiphrof.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmvimfmok.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gkjedpnkn.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqgflhxcl.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/glbyivleh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/guqyojlyv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ghzlfjeor.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbvuacuva.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gbuwnngli.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gfqjtcnde.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/giaworqrg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gozdzandd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gyakypuvx.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gvujcxktp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gnhahplna.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gtrvmzlij.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gmmsmzsvy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/grtdxwoyf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gszmjgvvf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/grwylzztn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gtpwvibkw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gqturtkhw.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gbcbnccro.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gqspxhgfc.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gafmirtci.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gkfpheuro.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gahiqidhj.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsxmfglwu.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ghxcsaypq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gfojcxidm.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/geffdjmxd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/grrcyanft.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gcpzmdohb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gstxbmhoq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/guymaqhlv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gtrjylfvc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/glfyuswln.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/grnmdifoq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gcygjhham.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gsczhgzrs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqcewihxn.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gvavyysko.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqioanawu.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/grouaxeyv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/ggwqlzrgm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gfbtfscui.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gdzulkmxf.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gownaordt.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/grdyfhihc.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/guwtzqlul.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gjmruftqm.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gzibeadki.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gmpkbyyoc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/grkxzpjdr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gsqegkufo.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gkiejckmh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gijwqmxko.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/grwjzwdvv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/glsnydege.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gupnhhpjm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gxwbjxyfe.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gmhanjgmz.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gcdbvccfg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/ggkuiwtia.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gizfdzqkt.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gqwgbrlpy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gizynlydo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/ggkgewjow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gdkhdbefq.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gzosqremg.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gpotgajbw.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gyopgipsh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gxiqcespa.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gcvfsyhqc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmskembwm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gpviqndvq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gchwstifq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gnlswolfh.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gvlftojwd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/goskxayyn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/ghkhmxxuo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gemrpjvqm.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gatkznaeu.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gemiwwnfx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gjqhfktwp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/guxgsjoxn.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gsljpjrci.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gteytatqs.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gprhuokpw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gvmibidgc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gssfouhwp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gevoeqkka.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gmrmjdtcz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gngcrcbyz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gkxnbjyov.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/glilwgmst.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gykohbunb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfxvbygkc.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gawakehvb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gisalirqf.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gdaabmlim.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/ginwyjjqk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gjkjpjgki.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gznkfjwkd.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gujkdhceg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gpqeuwcds.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/ghnagjfoq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gqgnyalne.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/guboggetl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gqnapgnnp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gcpeiabbr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gejdkfsta.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gzgnwsuay.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/givwmvmyf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gvohxubrn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gnnumjzmu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gleglvsfq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gtznqawqx.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gpqzwldlb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gmgmayyqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gcnapszqd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gxnuafxrw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gxfocbflx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/ghsexqouj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gnlamdpat.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/glbobdurn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gvkktewwm.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gmavwpngg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gygcvsffx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gjfqxcuzh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/giafhxntt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/grmpbomjg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gvbbiipwh.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gxypeyrjq.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/godlereeh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gifxkkbxl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gwvrunfqb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/grhfnmdro.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gurxlujlz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gomivanpe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gspfvqiyr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gtfwemiey.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gcbvquqpu.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/glohnpmus.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gxncxzccb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gclpqwijg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gpbjfndti.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkyzvjwid.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gzywrxepo.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gqaiscbmh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/godwgcukg.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gadjtjods.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gsetuasdp.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/ghadcfrct.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gwabivjth.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gmdpcckan.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/ginyufyvx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gokdmxlpd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gicimkyft.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/grjswfkvx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gpxeyvmhj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gyxsarrjl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gmjdqiict.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gjicnonev.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gnvjmvlpp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghdtwzhsy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gwybnwlvb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gpceloaiw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gsvzbgmto.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gkxgichxs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gsttbkyhn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gznnsrltk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwuzpdnuy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gpdcdakmu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtdrslbja.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gqibvabqf.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gdcdsxffr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/graqhvwrd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gjpjndtru.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gmwehqmqr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gmpgdykzz.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/ggolhrivk.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gfdeknhst.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/grjqdinep.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gqulwgclv.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gnmqwnvxk.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gshgoliqq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gdaesyflh.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gkymuyzcd.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gtwvztflz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gzapmcpqh.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/giaitlsec.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gwseuzjaz.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gtxvnckpw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gfkwnslfw.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gqejtumvg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gtprmgxxn.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gfvabhdrs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gtedpznzb.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/grvlaeyqd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/guprmoydj.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gkhkshezh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gufmpykfy.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gftrvrbwl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/ghyimjihe.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gywdxibpx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/ggevfrnml.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gezhkuqdk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gzvxryviy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gysiukjhd.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gkwhpjply.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gkcswlwrc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gnpzofqig.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gynsemhwj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/ggjimowyq.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gowrzffej.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/guhnivkew.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gmbchgwwc.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gnwklcfhq.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gbzcsjynl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gpswngqck.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gldlsrfqh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gtiahrffd.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/goqwgbryo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/goqzsmioq.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/guyeaukyh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gintsbrul.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/getgbdanb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gsgdgghup.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gnvcrglvr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/giuwzivqa.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gcklcqnsd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gihjiywhl.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gbbsppgef.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzimluesm.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gyjfkbtnx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gtoupgvtq.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gozxkcvsk.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gujvchyiu.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gvysvilut.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/glpkqkzsu.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gehrqxrds.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfhbxrjzb.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/ggzhisqbn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxagwjnsy.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gxalajgjc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/ghngwuugu.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gykgcamqz.sHtML


<!-- 参考信息 -->