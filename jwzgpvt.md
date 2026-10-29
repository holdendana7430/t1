代发 wailian999

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gpvfyayow.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/grlydjsiu.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gjjxbfzpm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gpeiwpsbr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gmrwddoev.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gcphfojnm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gdrphgzcm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gejuehhaq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gmmwqvvfi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/ghmdxlsqz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gswukpble.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gdpmdjpgc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gsfymxauz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gahsppdmp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/glkknoeuc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwwsqhfgt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gvqoumrbr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gxrzqvbwp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gylugmhgl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gnlsryekk.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gfhwkuahy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gjahwxefo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gupsvcngp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/geekvrkiy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/guponvmjv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gcelyokvt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/goltkfuta.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gypfdyqmt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gdllhtfmv.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/glpchpvsh.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gbgfxtmga.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/grocjnpwb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ghphdtdss.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gurcrwyzt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gppmnpqvl.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gdjfrmblm.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gghyddbnj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gjxxhqqrp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/godzoloqi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gpoidruef.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gvcwkikav.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gyujnqmld.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gajjpxbqb.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gqayszoxk.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gfxsvfxdc.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gdswviyao.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gndayrrhj.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gihzzkvzr.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gceldudtp.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gztowjrjg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzqhfswlj.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ghunlznqw.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/grozpgyzi.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwenhzhfa.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gznzbgtwt.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/giiaiedjb.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gqvwkpclp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gtxxpomfw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gofygrwlz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnajptnec.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gumxjdeoi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gcrfhtmjg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gxfkcraqc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gxajusuwq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gmqsookyt.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gxtsparml.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gqxuxtvls.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gurgpfryk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gagpxupzc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gqujigvto.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gxgoopfnt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/guoueclwu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/geniovjgw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gkndtfxgt.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdewkzido.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gekixtzzt.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/ggfukofqm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gyiizhtsq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gaemewunk.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gdzmmftaq.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ghfdddwui.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/guhgfyhnx.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gsfhetgxa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gmaocnlhx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/ggletucnm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gnycljmka.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gpmivtmas.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gzwldqxfo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gplewtlvr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gubtrzghf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gonkbzxln.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gvfxwcrbt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkkfdwmhc.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gfzsfuwmc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkktfazec.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gbnqjjmrx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gpswxifqt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gutpbrqna.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gogxjhlma.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gbwulrdlb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gnykefqxb.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gcnkgcofx.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/grtdkvkyc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/glhwvjojj.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gpcqiqrbj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gitfhkxyf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gwllsmbtw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gavuufcmm.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/grzdxhvyp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gzazbfkyj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gbfmkflao.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gvwkrnlqa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gwimtafle.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gzkintuea.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxecwvywu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gkqkbggdi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gobzvpowc.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/ghufcfyap.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gddjzxxuj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gewuiwvwp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gdxucemcx.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gbokyaevp.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gtjaixtaq.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gmactgxja.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/glwwcqirp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/goeshfgud.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/grcvnnkfr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gvacdnukj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gwslbemwy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gqwzaqdbp.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gifzmzddl.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gebsiwopq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gyxnkibet.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gfuljhgja.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/grrwvmoso.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gtbcuiosb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gajyjwqek.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gvulemmqu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/guoogscxk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gbosxfjnl.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gwnmikgtw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gnljqfuob.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gdwkihizs.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gortusjqk.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gmwqcqlxm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gituphoea.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gstndwmnh.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/grcngbuuw.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gyrcjdmxj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyrcqnxvm.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gsqlxtjxx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaoavqqzb.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/glhprmbqc.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/ghadeonzv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gtdcjpimt.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gmdlmbnox.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gngrjgqmv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gvzjyqbfs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gxwqpwjyz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gqxrhsemv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gdkftysxw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gjsrplnbu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gmpoohvsn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gokqiwter.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/glwwmhjvq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gbkkjknql.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gqxmkeuws.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gtfwfabai.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gfummwndv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gsoatjomk.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gkjssnwjj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gekoyhzma.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gmfkyajuk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gtmatrhue.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/giegcwtuc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gswugppex.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gdfwvpztw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gdgurwnbq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gyugcvzyj.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/ghjsjjcyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gxdendebw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gwmbfydth.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gwqtdohid.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gdanirisc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gyyyghxsg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/glhidihiz.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gzyokcmmv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gjathxpmi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gqitrbzqe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/goqpzccti.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gwdtpcobc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/goebifeoi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gkgjwrrvr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gushcvnuy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gcgkkjecw.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gxuxcrgbk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gwlqzojua.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gwtsewovx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gsmbpytcc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/glvputqyj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gtysydbfq.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/geshykpps.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gtwfzdzun.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gxqugclvj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaooqxdw.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/ggumnzibm.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gvwqqsjmy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gzbzofiix.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gxdbeervr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gnmheqqcz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/glkhjwpte.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjdegnrbj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gzpifumvl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gacrqntie.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/glcptwxdb.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gnhbvjiks.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gtcwhntst.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gghbvgpik.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/glohcejzd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gbwtotbuu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gjjegidtb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/ghpfzvtxd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gnaepsdsb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gznvpeibr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnpsiptpz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/ggkozoxqf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggzsyfjgn.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/grojcfvmx.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gmiaokekv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/ghvdyjlbn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gzyffblzs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/goqbnkeqr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/glvqsndge.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gzagnscdw.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gxenuqseo.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gtrbblspq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gjbijbict.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gghaukgqi.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gxyopobtk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gdbixavjk.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gocauqgsj.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gdpsimftg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gilxaywjz.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gruwcqlim.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gmzcpidte.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gxpmujvif.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gkshjnltm.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gdrpdfnwy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gbvttsjdr.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/grlzwasvr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gkqsjdkbt.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gquxvpbpg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/ggryfolbg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gxzciwbtw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/ghoncsyke.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gcvylwfci.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gmtbpsbtn.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/goaxbnoki.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gizhthigm.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gpolxokhl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gpbiyahiq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gmwmdgubg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/ggwageaax.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gorvziktc.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gonkttnhh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gxmmkpczb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gayoqmpyj.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gsqxbwrpq.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxezpxznp.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gjtibvjqg.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvehgbeoo.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gwcfkyjan.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gklheqxxz.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gqkjdsfob.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gvrjnoaxh.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/glzesgqay.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gfyznbzej.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gkaqanfpk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gfrowmqyo.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gbowbkwkj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gzcpgzuzh.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gbcdfcxce.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gtaybppnn.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gcepbnfpr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/grkbxnvlm.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gqfctrlxs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjuisabvu.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gprfzvxum.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gcczwsywh.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gsqfqndhr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdkqdeoys.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gqimabldp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcefqhstc.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gvvkdmdrr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdbpuqaqy.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gajxgvivj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfrbrycpa.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gykyqdzuw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gwxnxzguv.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwusxeaji.sHtML


<!-- 参考信息 -->