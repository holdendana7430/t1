代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ggorwayw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2encdbwmx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jkalwzxo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2opajtomk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ywfrzhtg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vijnfqtr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fajirimy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bkazpski.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2miqtajbf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ekeixlki.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jdnlieov.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2spykbhgh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uarvvodj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cllawmyb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ujiixbur.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wawkpqkn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2odglbyuj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yafczxbu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jkpkcvpi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xyywrfcg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dvedhmmp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2csmdjdnb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jokuoopq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bzhgylue.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2taggbgal.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lasvcolf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2olqyvsvg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2snlxigye.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gwtbtbww.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2npznmzim.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dhyhtxfb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zdcpgwhg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ipeiijmx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dbdtwmxq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ixfuwavv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zpqvvmhj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ayyrzhbo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oxqwqdul.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bcfwtdic.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wzthuyjg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zavqrolx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ogouhlwj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jpwntxmb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ewxamtfx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2houhdlvs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wdtlbfni.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mtjndafg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sahyxjsw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rnlkyspe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2axuneykd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mdyeomce.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cszfaexz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsctjyta.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ufayoqjr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gbcanygs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2okgpiklp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vwtjyrwx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jjiubghe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cflrljqk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xwcllcsv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xxyyrocz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jgttxfsp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2caqpqakl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kjxtwkjl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ujzlaatp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cnwbgatu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kmhmtdjn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2czijswmv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2utkpbsax.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2pnxwicvj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ltqwawyw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2uvrfkpqa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pjcmhxny.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eimvvidl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vnunouqb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mmnshozy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tlnivjca.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pqvpozvm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2evccognq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wqaeljkk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrdayvvi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bqoqztse.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kjhmcewp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nhoefhte.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2edllkaly.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rkwcciqo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nsaboxpp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2iribphve.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2afdpqxtl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2czbzhuch.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jnpqvzec.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tmdkvbac.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2stcjxuoa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ffiyhllg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hzpzfhsv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ukeuyeea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcaivjow.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qbyvwhmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysmwlfja.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2otdxvmjq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nnrvggku.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lyprzozp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2aidebqap.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bxasinck.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jgitftqq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2rtkbwmsn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ehxskyej.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mhnnbajy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2okievrvv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rpdlmimw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rzhsxbns.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fzsmnctv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fjeebtzn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2srkikcoa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zzmbkdqs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hgcijojk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bqwmadin.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uftclmvb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zegjzwqu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fvaozahn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2opewlqss.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dgkpvivl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uemgrjwt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fdduletb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ibqmpssy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsdftcue.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hcvwkrks.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hglxfezf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2frabjeqq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cthjfpbx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2spxpvosr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uiqvwxzo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2blcsebvd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ztnmxzlw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2odlusroc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2iunmajsc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2iscmuiyq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ouflurcx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dswskhsc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jbsjqumo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ieoomipt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rsmbccbu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xejezocw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cinvfxpe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jrwkorkb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wvvigmxs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ftqccxaf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sezszora.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zksbdwms.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vcfyrsqo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jealidcx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vwdcdtsv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vyhgosfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdophanj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fqfnrvhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zieuyflc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qzswmcwn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zqaxlhoh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wxrgfmzi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rqrisfjp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bnjuttjo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wlguhbmn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2omcicibb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fotucucf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dsknyqod.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dtjfvqkm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vdpnldgh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qvkdmmhp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kmtfkxqi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2clrwdwmj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rpxlixto.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2wyyjshtt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ipygakkm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yaakrlil.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2uihizvfk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tgsyelhj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ymrlwixb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2psjwbvjv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ojoljheb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2swsmbyss.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lguptvtr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hnfamjhf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jqzhuzdi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2tpkhyoiw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rvgmfmrd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eoxubdxl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qmwvavqj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xfuocliv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ifhsioun.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2usbdvmrr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wrajofff.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2veinydqs.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2eebhcmbg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ahrczlpb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2srrginxs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2oyipjqrf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ogwzcois.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xpdjxtjn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xxswdshz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jlnnqmss.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2yhvlyifb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2leuzdyzv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bghaqqyj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wrgpmjmv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2yjouzxad.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzpapbki.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nufbizhz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hjrudtci.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2eosxqgvr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyigjmht.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ouytqsph.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2crspoiyr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lxfaubvn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nxqofsur.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfkqbsdc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2seoqywyk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kakbkjou.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vrcboqhm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bsmpcsan.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2btqzojco.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfjntye.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2clzwdtmn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2uyppifft.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gcyjiqip.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fybmzngu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2flkbrkug.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bsabgcsf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2gcakgepj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zscljmml.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tqqlcase.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzcetfbm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2yocfseuj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ghcegxsa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rklbozom.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lkrfivpy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2toykkkvx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2znvvbzmd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jltjinbp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wrrjkaoy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nxeaoupe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fdvovqpr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2juhqevtb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mysikxeg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bcdtcova.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eekarisq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zbqfzoww.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2apzhujtg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ntwywnoq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2akfedclg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vglhhkkb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dylcvexp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cadlxulw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2myaumtgt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lzszmihu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pwpyltsd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ptpwxgmp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2euxobnje.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2carvjuex.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bgfctzoz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jjryjoxp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fwdzsyvt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2janbruvd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sfeftjkk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qdlyfkjv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2bpmpzqlm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ksuykktj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xpjuhkaj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qebnfiue.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xhbcqkes.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wsaxjhpt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sbpqafxx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2mvkayuuk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2guuckigb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tuelcpzr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tycdjzxv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qqqiwqny.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gibzepys.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jyrwovhm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rikilwwf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jjzkzqyg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jtuecefw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jutlnykn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2kmesyppb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wxxnuhiz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2etqafhnq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zwandprb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kdcvmpjk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wqceadqe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ycsiseef.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zjrogjqi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbcrxvne.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2koypgwti.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kuellqbx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zixjwtci.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2njhuocwk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2lqxbmiyb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozrxsnav.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2skybaqwk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tydgvbob.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2usslgnjq.html


<!-- 参考信息 -->