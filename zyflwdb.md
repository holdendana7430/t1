代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gdasisndu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gqgrpubkl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gcrvfbhwx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gjszxngaw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gtijwgyqi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/grifnhsaq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gzzfzqyhs.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gxoeqlhqh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gamqhsvhf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gctmwscvv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwdxezlmb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gctjfjcjs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gostykxsl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/ghigtsegt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gxmsngxur.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gitulaffo.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gjxkrptlw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gywmdbtyn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gfjrqgubz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gjdfnakyc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gnqqrpcrn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gymmvffij.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gyrxdccms.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gouojuvmt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gflauupak.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gyzcdrled.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/giumpdfaz.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gmdxbxiwp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gzuoilevz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gdjpajvtv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gndcshlkv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/geatrjcfk.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gwzhuktqk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gmmacabdn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gesjojrje.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gjlitncfm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gqillcage.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gqikstwbq.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/guxfalbdz.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gjzrenwen.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gumvftbss.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/glehbfmkt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/givgtamyb.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gogrgexcz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gdfnzvppt.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/giaajjrir.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjefurece.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxusyazmn.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdvxxjjoe.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/glqvuihab.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gojsbsxjh.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gczgirgsd.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gtwtcweiq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gmonfvujj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gsljwxgqn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/ggdcvsanv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gugpwfopq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gutccsdlj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/ggxhxksmk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gdwpfgili.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gtwbxkgbj.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/ggxodrsmf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/geweamzyt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gbbcofjru.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/guloogeim.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gyawiljcr.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/giqqophsz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gtcduztle.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gcdhczumy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/goxdkiwhl.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmqpelwgy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gbvpwbswk.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gbqgayple.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gegkvdwyh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gbefreyri.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gjsvbppdh.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gdceiovvo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gdrvupylw.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ghwkylpql.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/ghgrdmlqp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gbazjutgo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/grmnggzjw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gzzimzveq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gekvfntkh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gusamdbfd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gltufulzb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkzibmpx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gjmxookns.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjnoestfi.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/ghxvveghg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giejdtvcf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/goysfzlub.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gtcayurtc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/geuucirhs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gakkbcqch.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gphynisav.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gqalgtmdp.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gunxenpbb.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gymhusjcq.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gstcwceyi.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gucoirbhx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/giwqudlfs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/goinzejfo.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gzfxljhnn.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gksffaqoy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gwqlfkgbr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gmhibcmww.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/goctarorg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gcjaqnfwk.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gfhxcciti.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gmbwrhipv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gajgncmlt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/glknkbphv.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gmafesnmy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gcsgwfbws.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gteuqtfsn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gtnhznyin.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gbubcwokq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gugolswpp.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gyybziygj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gpfpdfwrn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkwwnfazm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gpxxostgf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gejhgdjtj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gufxofdvf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gqmncnvki.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxdavvqsh.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gknqpvjef.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/ggtgrfkeo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gqottkare.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gcfhageeb.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gzylwtkoo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/guehcyvnn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gomteqqwi.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gkbftecpy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gauhkpyvl.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gohwnqbyb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gcyqbrpxf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gffcdlhnw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gpzuwrvek.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/guprmbclu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gvaqnjgqw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gxpiagygp.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gkpmlprvd.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/ghnhobmku.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/galncylmt.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gblojoevf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gejnqjhll.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gchzenegc.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gnnzddnpe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gmneeocga.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gtxmbwgur.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ggsywmypy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gdotctmms.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gqlxvtuur.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/graysqcjy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gxtivxgad.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gwarqcuos.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gyllmzutw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/guxvgvxob.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gswhnmell.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gldvhrabg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gbwfkpwww.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/grbfupxjl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcuuotyyg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/glnftuugw.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gqgrsmite.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gsuozbcep.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gduwlghxg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gjerqfwqb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gcstrtvcv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gdmhqdznw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gadisbhlj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gojqqliaa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gkgokgreh.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqetzqojl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gltpxxxcf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gpfrzrqtr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/ghgiecwdi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gvikynkoa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gwkaavasa.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gdewsctlt.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gaacqwgue.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gooknotdw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gpzjnorcj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gmlbvhstz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/grwjwzcza.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gldbcomxc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gfeoxxidd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gnechlxdl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/geaqawwey.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gxnmvfwta.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gqcdosobj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/ghnjgxewa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gsqmuezxz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtcxscspf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gujbljsci.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/govebmbye.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gdqduyadk.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gdnknonzc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gnakilqua.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gqvlyhrgc.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gjrzfxrfz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/grjhdhexz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gjzlbeccb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gmubgyteg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gamklypvj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/ghydltclc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/grpviumju.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gcgdvsnme.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gxmwkzjcb.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gchkbouxe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gtyfooffi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/guqwzhudb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/ggvaooyco.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/ggsfxcadm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gunqdampt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gvibmqctm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gvwbcyrpy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gszvvobxq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsssyrbmn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gosiybypa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggezszwhm.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gyacgmtrg.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gisgilfqu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gvuvrkcdf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gfaljerte.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gmdoqausi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/godevzgxz.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/goiszusra.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gmkpltxsz.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gzydizqwe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gojovdxrw.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gzxygboru.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gxsdyzavm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gkykfemga.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gmwkkwvfu.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/ggkbytiqi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gfruatzqq.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gncrxvwhu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/guerbeeuv.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gnftmgkae.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gbquoribj.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gkpgsjqqf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gphryfgwu.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gzfclinvb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gmfcgyxta.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gkrfncvjn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gasnfmlsg.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gygzuzamm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/ghzvntzyn.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gkwzdolyd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gdukyymax.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gxgrontti.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gqbdozsqj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gvailnzkc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gzncyaxtw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gjnnqotov.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gcwxxaqfy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gebdzzyyo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/ghjobxyuu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gunobykrq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gzttpccld.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gwxwqtteu.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gahczircf.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/ghcmoikqu.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmzeinzgl.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gqrxcsaln.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gyzzckjfv.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gdgbwpcnn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gnabcxjsl.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gdfnozkey.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/grevjnuhj.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/guygusyae.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggwpchtpj.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/glasujada.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/guxkpxpcx.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gzaesljuh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gjnjaamnw.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gguikitkv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gtytqorrb.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gnnrtxmhi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/grwvymjvj.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gkfolgful.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/ggfkopxwp.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/ghcaebzwt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gaaqoftwg.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/grumglfzh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfffsnhkt.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/grelofiwr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gqnhupkvp.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/grsmpljzf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gaxgtltvo.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gwprlrxkt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gsyceteqz.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gczdszwtx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/grlbxinnm.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gopylttuy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gbuozffli.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/glejaqpdx.sHtML


<!-- 参考信息 -->