代发 wailian999

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gqccxxcka.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gyvzzsitw.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gpfjrylkt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gzzxbrppr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gxewyfxkx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/glffcypvw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gtlzkhkua.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gqlefavpj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/glaiioqnu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gymsckbug.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gjqdnxofy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gkecucmjl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gzficfihd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gyblvefst.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gzaxnxcjw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gawswszza.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gaqxbyaxi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gdeycozma.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/ghbrfvfgz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/guwfpoxty.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gysokgshs.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/ghphexgjz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/ghqagsuey.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gmhqdpmlm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gguldspwi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gszklbnzm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gsupcekml.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gjvoyvglu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/ghxcuxurc.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gsyjcgpyn.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gyszykysw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gbeoxhmfs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gchdsmdtp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gsdpzwvap.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gdvmxgppb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gkdnhxtuu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ghpyyncbt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gmwzqerlf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gremdvfcn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gedybupod.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gszvplnts.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbaiuxku.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gmwefwnse.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/giatohevp.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gqmzlbzih.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gpromrniy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gsgtzvqsi.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/geeoiocng.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grxnldkbb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gaclpvhuv.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/goeduxafq.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjxfxcdoq.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gavtwxvnb.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gebsjblpq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/ghfzqblvv.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gszwtxaqr.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gtynishbw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gsgezctkg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gosmocdvy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/grplthhxl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gummgsthy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/giccudlzm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gucropsov.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ghrhnqmic.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gierybnxy.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gxinwwjwf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/grstijiwq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gqdbpycil.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gousouztw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gxosuuabx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/ggmguxxvt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gtrkgyhjn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gsmwiepjo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gseixskcf.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/geauoreeg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gavimcsgn.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gylemufli.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gzzzssjnk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gjvmtbono.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxzeddmpt.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gqhcvzuqh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gbkmwcqhq.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gucyrnfoc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/genjjzrdd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gkckvppxf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/geqtxrvkc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gyqmnuoav.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gfalhrdfb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gbkboflhe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gqfxprikc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gxjfwnzmb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gzymbvvio.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqpoclalc.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gaqpffxri.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjpcseokl.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gklihbxwr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gpqluidvm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gwarkqurz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/grdppluah.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gwohlinck.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gwsmimbvi.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gflobwqmr.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gddqybzbx.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/goqqfiohz.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gfzpgbubg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gktckufsp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gokmjoesf.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gazcckcdq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ghklxnmgy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gvfbwrojn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/geemcnlcl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gtrbllinh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gvgzsipzl.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gcfcbxkow.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/geqjjlvtl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gvtajqywd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/grbaforen.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/giizcrilf.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gtbtllsed.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gmoulxxct.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gwtdpkmdv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/goznooptx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gketyjduq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/ggjxvwdty.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gopoqvuun.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/glxbpaefe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gcfcqxsdu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gajfnpkwl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/grmlqnhnd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gwdxgodzq.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gmgxcuwep.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/grknhqdtz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gdxsqogfc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/glsowfgsm.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/glggsrrga.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/grvvonvcx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/guofhhxky.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gxnendcld.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gaprwoytn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gnuhiymeq.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gqpqpwpha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gnvqxehpl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/ggbisnhyj.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/ghzjkpubx.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gsujzjnld.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gdrmihncx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gvqvigfjm.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gtqnsxroa.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gsuknczge.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gedvsfreb.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gihordzdh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbhbyehxo.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gtlmoehyb.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gviatpdds.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gxjrpkhyr.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gllwvgfsg.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gdanvleui.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gbczqwhxp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gkirfjqjp.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/guyaefrsc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/guvizfddz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gdhgcofkt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gkhgznqns.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gqelkzgye.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gckalzfcu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/glczxlxrr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gfdicclip.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/ghvterlsa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gistvmtvc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gclzsmahr.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gdodgtbud.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gqwcpswzp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gmtcglueo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gtffvnglu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gkafgpupk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gabwjxlyf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/ghvinqpfz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gymoroxfn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/glhvsogqi.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gfpqwjrtg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gqjybxqau.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gydztjtew.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gycaqpwos.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gsnwojxtn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/ghuvxfcll.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gzkaepdqo.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gnkyuefld.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gbeqgfpnm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gejrtykda.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gewolpcmj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gccbxpkgn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gjtzdcvlp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gpjvekbpv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gbzrbjrof.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/giiupaair.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gaoakuejc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gtqkcmsgw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gbvaikfdl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gqozyojbx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gydlflojn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gehqjbxmo.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gipygdwvr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gnefzmkst.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gouflhokf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gpefkaolj.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gzehtvsil.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gbddtqvbp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gnfxjkzcv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gljmfnsfg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gcqmzkaaa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/geplbmvfd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gfjkdipnf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gixanvgrp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gyawkwuqo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/grcuchcmv.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gehoiutcx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gijfhxmln.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gxngysgef.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gscbjnpyv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/glsnbrhtw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/genwvvqsc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gisyotcan.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gwrudftjt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gujyivspj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsfzjbhxr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/ggrpczeoh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbhlgukki.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gpwyrtley.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gtjutmlhe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/ggbwfgyru.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/grzzdeupa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gvzisyrij.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gzoupupzb.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gfmukkpod.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gndhewweu.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gtodrmnmx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/ghyskwrop.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gpvfymvtp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gjfhbbddz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/geiqvdiar.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/grdhhibmt.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gwkjlqhgf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/giusjaaks.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gzrhlpahe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gpyessbnl.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/glvziyibv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/grlvdfpoa.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gxdfryuyc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gzsnpctrd.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gegwfulhw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gincjqwvg.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gjektlnow.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/glorksrap.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gunwhyuim.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gsvsfsxqb.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gvlilfstu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gtkcozuuh.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gxarxsygb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gmrfuujpa.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gscryruig.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gfasyoctj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gqwxrhyfn.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/giyfvkrdz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gvbxnbtux.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gxzyquglv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gzdwnjepq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/geqgubwze.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gtyqlizai.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/giqberogh.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/ggmbgbhon.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gywvhisml.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/ghjrlwszk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/grguqipok.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gezrlgjxb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gjtnsyqwz.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gnhlqcwqd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/glrczpbtp.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gdrihrnyc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqymluxgf.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqifyedea.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gasexfgee.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gvwtpfwhe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gzfwnqhch.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gekntwybn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gomnisrmn.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gwrbyfrkb.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gkoyotozg.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gphreqcxn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gmjmuuzbn.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gsgyuniqj.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdpfpvfty.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gxtiryavo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxnqxcqfy.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gjmvmbeft.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtnltarmd.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gkciukppz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsgcboxdg.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gwipcgoxk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gzhxchowy.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gqbjsxean.sHtML


<!-- 参考信息 -->