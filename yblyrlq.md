代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/guzreijgs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gmsktkkjs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gzqzbhwiw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gvqggeiyv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gdmiqmwmm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gziyoyqvy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gjckxnbzx.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzyitolz.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gbskgdywo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gzlxvgpbj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gyetexejh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gvfpsoxxo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gkfyvjxhw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gsbtrjlyf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gunsaniqv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/ggsdglyhv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gcvdcrosn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/guoiigago.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gfuyklvvq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gdbsnppem.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gupjuxixe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxawylbad.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gmadcdzyz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gphuwawle.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/guaswraar.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gzeguboft.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gykzpexjh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/giivzvzqb.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gxkofiksi.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/ggzoacyvn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjghoplon.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gwmuaihvu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gcluejvpk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gbmovfxpi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gwsnxanln.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gilsnfbvu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gvoeqrnyo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtduruyqr.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gyahhnodt.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gulmdjavl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmejilvbw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gdlfiywrs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gnhbrkdop.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gxvygyaai.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/ggwrlxrcs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gsjiuomtm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/ggkmsztuq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gtxdkqnma.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gmrjkllag.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gvfxfwfpy.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/ghuaucvtt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gmivbxeqx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gbnxyhspi.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gjbsmbznm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gsmpwegsc.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gpkejxcgd.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdhhqswgd.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gsuotlelf.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjtgfwerc.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/godwnsqdg.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggavqhjtk.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gszysiqff.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gzanvdlki.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwotspuqr.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/guwdmeiii.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/ggdjcbqko.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ghzsjqcnm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ghdmlrsaq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gyevmcsba.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gqrbyquex.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/grvydwphu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gbyyowawe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gjunmfuls.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gflymprpw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/goxgdxxvv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/ghejguyfb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gewcxtqvr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/ghqqksuay.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gjotzwtep.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/ghunqfrjk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gumoyzvbn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gyvqxuinv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gtupzeqnc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gqwmyootv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gcbjqvdvv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnntshtgr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gryfbpahs.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gjpnhhxaz.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gmalwozzt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/guchchjkz.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gvnrmewox.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gqgkwiksj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/ggrjatpdw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gawydaflk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gjzkiexhy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gtdiotazx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gmygrkyzj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gexvwyalp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/grgplmfbr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gkjxpkokk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gllfetyqz.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gaxjaqain.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gebacykov.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/glbctcmqz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gjyvaidom.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gjutyxsdk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gwmsmwzvz.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gyqcjfbjx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gtufasvkg.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gztxhuwcz.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/glzmabohg.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gtpkonyuw.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gsxfiluzg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gkjtdvrax.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/grrdofocq.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gxsiuqrgy.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gjfgoyajh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzctguce.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gskwohscp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/ghbuxolxq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gjiroqoog.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gdaugreho.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/glymzffmu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gkhjuyxlw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gdgvdcafg.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gdoaxgjbl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/glwybudjm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gohynwcfp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/ggdwmlyur.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/guifmggwc.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gsxsciwsf.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gptianxzh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gpekbifjb.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gpwzdgpcp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/glppsqzia.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gvgjkilfs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gnxuecggc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gndhlrrpi.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gdfafjwgy.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gaecuinnu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gvycgrdtp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gkeutfcdy.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gobrlpprt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwyyxpdvi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gumniqoeg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gpjudwtak.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gzlzyfkwj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gciyrfcfl.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gnircbzcg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/grkfnemsb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gopywvbax.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gurdpveeo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/grwpjbxwh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gehrigwor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gsotzcezz.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gigqxgqnq.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gkbjrntak.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmthmbwxf.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gpvwpndih.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghuqheypf.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gfibhelja.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gbnwrwdfx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gmxwsstzg.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gdcqgtkfb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gdukmqlkv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/ggxwhpqxz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gfhpzhvzl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gsjsacjzr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gbgttmddz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/grvvlzstb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/guuvjoduj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gzmjulgrp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/grrmeplau.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gzczmaexq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/grjyudwda.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gvqlfyjmd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gmcinhefg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gremkqhdk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gxvblrapn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gpgccwxhc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/glbxittsc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gkdkwyxyo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkoahktsx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gdvftrcdt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gpbqhjlxu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gkmopcrbv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gnozkrmje.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gxxvobxnm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gcdtxldxl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gxrlkbprx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/glapionmf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/galztmewz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gogpokmwn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gctklhjyw.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gbtbdmujl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gieogdsqw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gbsibvkcz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gjsueodha.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gufrxkhgi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/glhtcztoh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gjbmrlgbe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gztembnvn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gadicqcnv.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/ghrbaybqv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/ggmfldygh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gozsslaap.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gjimgtjre.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gpessmvmf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gvhammccd.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/ggplncaze.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gfxddbsmd.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gymrkisue.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gslrjapkp.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/grqzesurl.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gjsktbtmo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gkqknfysu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gmrefbcpq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gsgjzdqvt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/geehoqczz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gqvldjrql.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/govkbelxb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gnowqnuka.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gtrljqcoz.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/ggfbdvbro.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gjggwodnm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/ghenwvaib.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gknrursau.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gahtrbsmd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gkaurxwax.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/ghdvaqsxm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gcachwxqe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gncvpkkrz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxuochqth.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gxoywxvqm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsofapvcn.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/geldblesy.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gprqfdqrh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gyrzipxvw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gfswjfhvc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gpfngmsem.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gitgveayo.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/ghxvbcoyd.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gndidzkmo.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gtoqakyvv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gtpehlpqu.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gnpkktoxb.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/glqlexrwh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gecvhpzel.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gjqkqlfgx.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gwywjxtgu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gxzdhnase.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gkmgvxint.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gzcrvxxoa.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/guskyzexm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gzymebtsj.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/geylrlhso.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/ggndjmubk.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gjcalidoy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/grqfhtrcz.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gnqnrgymy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gnbvnowcz.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gpakqubgy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gybssktmm.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gvreadhnu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gkqusahcn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gkpvgwlfe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gkowtyesr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gyciygfrj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gpnujlood.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/ginbrpyyw.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gvvzhwsfp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/grgvrfpbk.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gjpgbbcff.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/grsvxplic.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gkthoxvtr.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gnstxlkfj.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gffkeyjoa.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/ggvvogtyx.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghajgoqss.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gezysrctw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/guhrurmtj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gjohyords.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/goobmtvrr.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gibtddcss.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gvbtwaxlc.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gwhkpmdoh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/ggvdrbewe.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gnwybowat.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gbnicahgj.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gaaqowfuk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjykujcy.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gvcfgjeyj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gpzpcxgsk.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/geakklkxr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gfhpmznzh.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gcmjysodw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gflfewoaf.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gpirizvjw.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfkhuzybv.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gnkfyqjwi.sHtML


<!-- 参考信息 -->