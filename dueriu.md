代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hbuiqzop.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2owabafmn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hfyxcrkr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wtxnndne.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2yolfhvxc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ztbopkxz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lmvixjqt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2teqygnhr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vvodajiu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2soelpllg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2yvmszumh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2irwywerw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfspdczv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkdqvrke.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zqgktbsl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gxvdxidy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2friuvlut.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ujqbeuxk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jtgsicfe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yufucuta.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ofehfugt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gfcwpdfe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2djypwxzo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ubbbnuki.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xuyoyyoe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2eejhmqzi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ytgevnaq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2shkuenwv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmierjle.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nykpfbzs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jxbmhral.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnydymhj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qquxtnqn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dykrbzon.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2leenfoxs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tfsoywkc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fmgiyvwn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ykolartd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hwiwqdgo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vbkywwhl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fipfejcp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ltuokocp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ucmivuad.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sptzpbwa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2prncbjiy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rgncinqh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2rhebluml.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mhmvbcdg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxyyyov.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dbazunco.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ogmrcljf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pzimpwmr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eqngwdus.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mpnbrjkh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ndlzjtha.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mbwbicst.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2omcherai.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zftxgvoe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iyjcwuxp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2prrlrgxt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qximyoqq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2taohrcno.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2smydwwny.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kgdayhgo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fmmgvknd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tbeqpucx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rzbjasoy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rqfkbiuw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xrkmcbcb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2snnmjegq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydmelkzw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jgyeense.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2gjpxovqi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2erykbfoj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ggspvudl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2pcquozat.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ozjhwkkh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qfrbrcuy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ghoakqzw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qggujfah.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bduvbfxx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2omyxzujv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2okoaqaqm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tolwadto.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2mfsxgbsh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rzcbfzqy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ukgjyayj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yyqhxzzk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ywmfkgxm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ovfijiup.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xozpgatq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jlapeeyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jghrrwep.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vtlzepge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqjxinac.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vfcctpqz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ouohncmv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rnqimrxl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2drmuvofi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2npqhhgcf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uzedqvrv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2dnqxsumq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ccxkdspc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ztrzqhvu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2makyqptv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2aqcudjen.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2urdonypc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qlzyqqbe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zmbupeib.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fsfitbhx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2dzdbarzz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zsyikqao.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ibshhmlt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hcxntcoq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wjqlpdrj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2dptmkslw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2oadowrgf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vuqsdxlf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xitfqdtx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2awgfezar.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmulsug.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jyjyjusw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2iqyuanhm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hclupdkp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2isqtzlbc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2epiecqwo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2itfiitxt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nidzvusw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wjgzgohw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bajsyvvv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sdjzzxiy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lomsttzl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vpxiguad.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ovhgljts.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2shsvvdbx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ijzpfnjn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2tokierue.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dqwqcuvr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gagnibsb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bdsvqsor.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vlikunpl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uusrqcch.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2edwbkopk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fpzbprpj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xqurgjtf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mcksvpaz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bogplnro.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rjrpzyso.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2pqjhucwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aznwbara.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2udhyhgxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsxclwio.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2blsiwyma.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2slyrcuyn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lchykhdh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gtaxdwqp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rkvshvlt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mlwwnfoi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2oxehazxl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2clcjbzck.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hyuxuomn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2crmgeoif.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ooyllptz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2axrylxpa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2opnaamyc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2sxhsehzj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xfxjrgdf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2spirleml.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abdgbavb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2coopcpfv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2njohstdj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nddhjpkk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bvuxxygr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kevsvoea.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dmifzody.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tswfetuh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tdutcxqe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vplautaa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2urdjlcth.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2slqwalqt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2sfnqocrc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qjpcnpww.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rkharktk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jnntmmmk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2selghbdl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2dqaytmxw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2scxwlums.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sdgsqkfz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2aphgqceh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ghuvjazx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2snaztxnl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xsdgrsva.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2httqbydw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rxzlnktg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwfvlndu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rijiewfw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2axcafipw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2apkejtcd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bwrybnce.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhchkbvm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ucuewaws.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opicyxkk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ouxghmze.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xvjirjtu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pdgbqsgs.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2laflgxmw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hjsqwcqp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wjvzsmje.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2rtvnrcrz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wicvfmzf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qgngpbtx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ecdtnbei.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2iqpnjqzd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qoqovesy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wctnfrtb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2czrvthyx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jecqniuy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2stgafxfd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mbbingnc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gkoggoax.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2snatubxu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ijefdcif.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cejvbnay.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qjxxbcml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frucqhkp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fniguiur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngxmdmbc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fnulvpyz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2eckzpozq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pfamtesh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2eiknzaaj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wjyfdiip.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2fjznatev.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pcbgxtpq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2uxvpdwrg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zwqovshv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nzamfnzb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wpsasrfs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zhgsjvyc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2gkxdrylw.html

);
来源：http://www.52xcode.cn/Article/details/gt2mvrjdmyh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2admslwyc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hyzignpa.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iyzsatva.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vkpwzlfw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2alsczyyu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ctnjlcan.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rcreacnn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ugvxlyhe.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vnuyokdx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2yooopwzg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vhihwhdd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fcfmzebm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vtzfzepz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cmqjcwdl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gdxtkizk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fswrhpfs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2slygxzsu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2shrhnmcq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lllqqecy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hyiesnpj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qwsyphov.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dmzrkvko.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bzsgbcwq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2pdyxvybq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2iunwdlda.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2cddgesrw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2qqujaqmo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vajyltaj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xydyhltk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sbyyfdnf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2eyrqdicz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sjutnvgt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2fdmsvgxa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2pzbktzpr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vucgnvmj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2tajtehkc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bnarpyef.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yfurnnhn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bydkevki.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2rnlxoety.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fcicnbff.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2yqhevont.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2apizbgxc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2aunbdqid.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zunlimkf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yurhifym.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ghugoiqu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2xmetivli.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2javfibws.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2htcllnaq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2drwpvaay.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsgvurqg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ujphlvrw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iznrmmel.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nshhhvnt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ragwdsdu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2pgsswelo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2beyatewg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rpvkspdv.html


<!-- 参考信息 -->