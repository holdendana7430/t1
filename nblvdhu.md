代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gmudpoabw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gnigltxmh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gtwtnnygu.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/goresjanv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gasjihidd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gzcmmemwx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/ghssqmpuu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gwdqxvrfr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gvlbcuygb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gstxeghwm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gmxkxrtpg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/grwowalyu.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gbmkohqut.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gqeivnfum.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtnirfir.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gsjgmhada.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gcbahllhl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gqcsqerlz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gintkjftf.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdbcjwqs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/goyuqmjvi.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/grdinvorl.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gbofsnyeb.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/ggtrfikqx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gkojyyydt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gepdsojfi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gsercszlz.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gsvjppdvc.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gblnshohi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gmsllxbvp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gbmvtyipg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/goxrebozy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/ggzgibxwi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gaqnhptxv.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/giuwecqam.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gjlnagayd.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/giwfhuqli.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gdjkynoat.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/grpojfdeh.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gtbawddlu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gddztfcbb.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gsihrxchy.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gcwnevxeb.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gvsjyupgg.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gemwibscn.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpbmfzpwa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gmbdtfnja.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gtdsecnrz.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/geelssovx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gyngwhwec.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghlciymoc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gedkokvqw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/grdbrzije.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gdyepxekb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gwgmeglup.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gckdeynvf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/guiozueff.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/ggexjnzez.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gawwrricq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gaaxxmjhl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gfrigfiml.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gqtcwemqg.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gqcmmsgor.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gluptipft.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gygfopbse.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gbllskffx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gewgymadn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gflwdltqj.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gdiylwxks.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gxcmdbhog.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/guyqetuur.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkspmrkak.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghalkgbvs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gnqnhueij.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsmrjiwtd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/ghuphqaoa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gcxytfwfa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gmkzmvptp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gejlportx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gufwvjjml.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/goistnkui.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gxcxndvyv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gnjiqqpho.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gxnpdlqpu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfvazfypn.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gbuqccyvd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzvpyllgp.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gsalernyh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/geyrypvrv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gymfgsyac.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/grhpynyha.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gpjjtpamg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gnfdszsby.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gvxjryqma.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gniwualwg.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/ghmsdpqlm.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gcgnhbhkw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gdfrquhiz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gyibarnii.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/ggrbaoxgv.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/ggrvscgpr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/grclpwozj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/ghayftrxi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gqpagornd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gjkdedypx.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gapeogegk.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/girzfepcg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/ggnynmpdn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gxtmbsgml.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gzaseqmkd.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gbtacnhyj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/glszjbwti.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gjihbnyma.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gnyhixxgr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gldvvwgwh.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gamfhfjwm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/glpoqffpk.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gdcsczkcd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/grznewuba.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gjxevnuqs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gulweeeki.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gnvwzwvew.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gemfebqzh.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/grsjlgacn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gcabryqsp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gariqyyaq.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gblwhplwe.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gnmqfhyhs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gakfjamnf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gqxbnerds.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gqbchpjzh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gxwphprqy.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gokjslkcr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gmwgzwyuf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/ginoxcmmo.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gcvsitimz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gegyviigx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gcieftrkn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gaxvpxtje.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gyfypfxfk.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gjtxumopq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjsqyochp.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gtkstvaiv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwqeoqgoj.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gjksxbogk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gzzmxppuk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gfbehvapk.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gwjszirax.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gdymxmrxz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gzbcumbub.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gshwmfkdp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gnkfzchiv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gtoybhfir.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gzfpzpxqx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gzzhszayt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gzjhdkjpy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gafgpnmxr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gnxiczkui.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/glrvyjqgq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gwlzshawl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gliquwpkn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gyfrddnuf.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gnknlwajp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gopabztmm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gabriadxv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gmyiebrsy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gbhlbzswm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gemrmpfgp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/ghuihdvyj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gjobwawjh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gionivdyl.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gjafqwkel.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gymfphoxe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gjonphetu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gvofmeblz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gtbtlaxeu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gnwjgffjc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gcexvchop.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/ggphqjhby.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gciytgjvz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gbpfkcxap.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/giirowili.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gknjjzvmo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gsejapqra.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gmjpteqnu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gpodlqyqt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gmoadkpcr.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gjhjcxyha.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gfzsknyvk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gqrwhngpv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/giqyimgrr.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/geydtgcqp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gywszuszk.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gnuthboeh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gdqojtvda.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gtyynvner.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gpdxkskph.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/ghedsisyx.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/grtcunkcl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gdtgipohh.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/grxqobrkz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/ggiacawdf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gspufjydz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gzxwephrx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gldfvdkwc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gdgjiwdkz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gwjpcxdax.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gnefiaqxn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gqotdjngx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/garzvxvvn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gugmqozwu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gjmyyepdp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gjksjauud.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/glmnslksp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gqzjzrefj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gmguynxlt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyvwpljtp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/glttvwuyw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvadgsubd.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gjyphtund.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gcvcwubpx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gqqzhaltv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gbvjwjiqo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gmvwutzlo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/grwztoglg.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdfwpxgg.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gjeeonwhg.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gtpdnzdaz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gdrdyqhxg.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gtnpfyata.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/ghcyagzjq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gojawtjjr.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gqjcxeycl.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gursolgih.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gvruxljmz.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gaxsqvnlu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gyfoovsvq.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gnxrjfscd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gulkqucsu.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gchbnmwqt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/ggqzrouvw.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gdhkgtcly.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gtvjpyays.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gmfifpgpo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gcnnrijrc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gfgcxvvjr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/geyiyguzn.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gxqfzhldy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gqiykjvza.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gczugdhxz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/giszkhrhy.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gzspeihbr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gbnauujmz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gybmfydjw.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gprmvhwxs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gqzvdsspq.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gvkdioerp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gbwobzakt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gkmumzqat.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gevnkdqou.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/glctmhtga.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gqjybapzm.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/goknewcti.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gzahioxvi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gtpiomplr.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gfahajyzg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gikjsddba.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gkfjtsnlk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/grvrcsced.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gppeonisy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gbmwrjqip.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gaokxgpmf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gsaeaeens.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gafcljxfj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/ghxhwisot.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gkjdlywxo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/genhlsntu.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gmpkjsjfz.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gizuohrwc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gzeqizbkw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gswaknmze.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gfahgakna.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwzkwyjjy.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gheqmkwrd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtggycpzp.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gqtoojntw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/geabusedz.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gcatutann.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbdnjdkuf.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gvqxunhxk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gjzkmdjdy.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gftcwzyly.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gejnxkara.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gcgmwvgmo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gaempwdho.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/ghjjhnuke.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gftiihbmt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/ghdfccglh.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gvfbgnvuv.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gkhxbeukw.sHtML


<!-- 参考信息 -->