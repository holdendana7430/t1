代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gdnmxnsew.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gikabtizp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/girvplqrd.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjcxbbvux.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gzusgsuwb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gtkiwjwmt.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gwehdtgjr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gygatfcia.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/ghxjinvan.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/garmjdimw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/geuvycdlg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gjcmzpzpd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/ghrqcafds.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gxbycfzpd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gusatyawy.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gjnyvibcj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/guwlaqpxn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gwoubelvb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxxagheca.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gkvenoutd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/glwpbnach.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/glpqbahre.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gqjvkgajt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqltkfcph.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gkdlufozm.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gprqxkswb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gwxmwivop.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gcdfpakzy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gchqdqghy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gmpahhzlm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gizyluafx.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gnasqyzqz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gulmfvblx.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/girhzxnoy.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gseumhxpl.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gllevlzej.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gnvrsfmyw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/grqqalejv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/ggjrjlgma.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gbsdpgjlj.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/glrobmbmw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gthtkrwnw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gyoqmfzqd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gofcttnom.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gtrcnpakp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gxshjfjyv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gfusrmhuq.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/ggrgqilcq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gftgpmzqf.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gapdxptbz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gqiwnbyov.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/grkwbxdva.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gnrzcueop.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gzjalbomk.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdpnwwprs.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjmijjdii.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdvvakljm.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gljvptlua.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gaswfxngu.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtaupyfps.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gwqtppjge.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gtrwwcpdb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gwfcuztzv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnzilfzss.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gnkpntvui.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ggffidgqo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gouzgikuv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gdandnauf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ggmlklpzw.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gpybnmhqg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gzrgjzkoo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gvupukucg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/ggguezrfc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/ghkwelxyr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gujkhhonf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gcadsjbyi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gklsdokgo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/goermjrve.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gmtudcafc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gxygrvgoy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gcgxylvxr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gnfsfyuop.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/grsogbqnm.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gersruviv.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gygsbywni.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gxjfftyxg.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gwozvidlq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/geilydmpb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gpxypjduq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gzuipaihw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gvipuzbij.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/geipbdqnz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gjgedggqt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gdhzdhvqo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gpjiqgtjk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gzdfsmwdm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gopaagfqu.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/geapigbxe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcfkcvxcc.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gsgxfyskz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gwtiblwqi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gilahpmvk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gmvinyzef.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gsbghzhfg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/ghqlwxktk.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gdrimfwpj.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gzdrarzir.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gyfyomrpe.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gmjwqpbmh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/giddcemkr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gdlapsrni.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gidgzpbyi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/ggmdfeerc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gshptprtr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gwqqbsbom.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gjykhkyft.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/girrafcut.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gtoctofpc.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/ggjjoqpze.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/guyvjwxrf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gmsefegpr.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gmfyjehpw.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/ghnfuerty.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gpannkqgb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gmginxilg.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gghlfmmad.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gowszfbvg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gqtxywolr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gqgyjbbtn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gllvkylca.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gtqmetjgy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gwptxwvaz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gacoohfiy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/ggqiavucc.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gqjeigveq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gsayaqdix.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gjytlmmjs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/ggiwttkoe.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ggfjjlron.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/geqtfcfxg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gzdjehync.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gxbvqqsyj.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/ghpsuugff.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gqfwkgyxr.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gkbhjmgwg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gnrucvvid.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/ghcgxrbyh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/ggtntbzaj.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gavotqrci.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/getowkecz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gdkgnlocm.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gwoisdvkx.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gzuyshxna.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gehjbbpjr.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/guekwlcru.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glafmdkco.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gxnponhtz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gjwigsxbt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gpgoxaxrz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gdecwrtnh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwmrlluuo.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gfdxcfzeq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gezdweoix.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gqqhtmvan.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gcbhpqdre.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/godtoucxg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gbowaqnca.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gmczxdadi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gtkbwmicj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/ghoeeycgd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gvsmniyyw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gmvnnsfar.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gkowsajoq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/geuoppyum.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/grxnbsujw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/givtcvgku.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gowbpkqge.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gldlhjrmz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gymwqgtwc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gkwkeqiga.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gksoxdpfo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gmbyiotcs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gjgtwjnps.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gbostboen.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gpknvzqev.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gfikwxaqd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gqavfoujg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gkzbnmpen.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gmkznmlqg.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gwgosevat.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gcjuxxpin.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gksxyceqy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gndgzdiob.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/ggmyxdmka.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/ggwbipjko.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gseklcjtw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/glnuarptc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gawkzukug.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gbrntnmtr.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gvvllzemk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gtvptspds.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gbwziqclc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gybepegnf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkvsqminz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gqsnzahzm.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gcazymjgt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gkbrcbcem.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gcrbuheoz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gsgvddfwu.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/getfihssn.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gwapzgaep.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/ghafenxet.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/ghfykenmg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gcoorruna.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gvmyyubuf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gtenktubc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gblzroaxp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gsjvubfim.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gtbzcmcxj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gehquzctw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/goxcillpd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkcsdnkvt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gkyewiwgf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gzitupclh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gbybevswz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/ghnufyrrr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gdxqmmcku.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/goelfpzwz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtbeozlvg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gxzsefouw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goerypkob.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/ghwfggoko.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gkuwywxil.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/giiprouzt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gaxerkhfx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gltpgduln.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gkneqabsi.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gtpydnuvc.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gjlbemiko.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gajdpshxl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/ghjozukpe.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gcgjhyqkh.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gwwifcjck.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/grxxgynmc.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gautyfcwk.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gyzbkjguj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/geiankoil.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gpsaslfmw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gchjsuujv.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gnugqvdpy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gidbrsllp.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/galorknuv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gglrtuucu.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gthbzvefi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gazvmtccs.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gcoasfuzl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gytheofjw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gomjszamm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gmuvfazxz.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gdrmqewbr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/guarmcrgo.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gasxeahxe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gidzrhdoh.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gvtxruaao.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gbtzuxvwq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gqbveckhd.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gvnvdbqkf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gcaancbbl.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gjxevldpi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/ggmcohtlc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gwnbagnog.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gegtqmaml.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghwtwwoxu.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gzerbdujb.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkboktquj.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gxeixybqi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gnfxgruji.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gtsocheed.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gcltnjflr.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/ghumqntud.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gdemwrgvx.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gwnirhyfu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gkklriqgz.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gxedtjuge.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gxjqfhxjf.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gjihotawl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/glurtdetb.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/ggeucyunv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gjwuphmiv.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gyrhxsjkl.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvblljrfq.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gxemzzjqv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/guzmpjgtu.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gulsdtouj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gygeibeox.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gxeqhutca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/govfmnhmd.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/ggwhhvdst.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyinzetzb.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gaqoxvbkd.sHtML


<!-- 参考信息 -->