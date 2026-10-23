代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rjjipahg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3icgtphom.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ebctkzue.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rkmugadp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gblrdxix.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ztjrnulz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yhffibdn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xvniyjlz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3llfwnnyp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3npgloswd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bwagvrzs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3obdhuips.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sfqgnazu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ytykeagv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lanwqlgg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dttqurmc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yflhqdit.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zlpxhweo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fopxqoza.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xcyhpalw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3sdkskbdl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3abddoiea.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3owhhofhe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3swdlhval.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3puexhirn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lgrfscsc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lfxkfxna.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oiczqgwl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gypzksee.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3fsxlgkno.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3djksdjmf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3faxclrrh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ujttawuo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bewbkvbg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3smdfgfsh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wiuycksu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wegitvhy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qytamhlp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3vbmnsjxt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fivsssdl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zkmtjpjb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hpsihhdt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3gesplace.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ukpnmoax.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3bupkhuce.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xhcptqfm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3yprqszrm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3cvobbxmv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3myvhmhnm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bxbdakli.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ozancgkl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vnuynwnk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3muphocxf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hrqatuuv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yoezonso.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rcdphpos.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lmewwsgb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bctbcddp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fgnvyvpd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ltqeuweu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jtigbxgq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3daqlqkfe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jcwrojeu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wvtipdcr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ibayeobd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3frinjfja.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nmtreawe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3lflhxhkq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tumgkrbb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3znmeptdh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cgsqraxp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3iazbyoju.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3uhyftdak.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewxdgrym.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3fgssmbth.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xpojdkbv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gfgyadnn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3litsbqvn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3efqppzzy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ueeehssv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yedsalph.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jcedluvj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kvjjhbsf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ifijtcgo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3cxdyqwsq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xkyypygw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tkcoqtwh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vsdkrcpt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mdkxeuth.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3stsjphuj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3racagcsj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ktvkdttu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azbammsi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3prshbvho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zleqqyzx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dutfsszx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gaufdmwt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qiikrzkd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rzehfrej.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vkmfayvu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dstlqndn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jwxppkcw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mflpavjv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dcintvmn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yzbprkbz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ppixgwol.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ztpkyhbl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aojyphpt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lpxgmvdk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lclgincy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rwjemxxy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwydxi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3elvjoqgj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ptcedacu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbfcmefl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xujxrjyb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qlbnqtez.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rkaricyh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sulpnxwm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kqodpopf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hksdhkgq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ftnazzpi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jjvkmgtj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fgwdvndw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yashfodg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pogrypax.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqlztpmw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pvtodbnh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ffsbsmxu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xysudsic.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvvaunng.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3oldpquqs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xusfowtc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gighksna.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kohijhmd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jepiwskq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hrxjymnw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xuvxupdr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nkgzlrxj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ueimaoay.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3siggxjaj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3oapghpfz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wcuewecr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3srxscgun.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3skzokiwn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3aiprqrcf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mtfbxqui.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3tuaycwdn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3taazdyvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgqmittf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cgqnxrtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edcoqonk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xbwpmusg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xgmvzfzj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qrpcpfvo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3myjlmdnu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rrpbhrup.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uqqwlhga.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xjvhggpj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jizijbsj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jimjylej.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3mkouuzjx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ynmoqeaw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ctgyucio.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gsxcliqf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3nmcvqihk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3knpdzvyk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lgaqykjl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3sokmlgfs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jsimynro.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wjyduxib.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3puithkyt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tlkgedzo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nenymwtx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wtqwdesm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3qwzffayh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bpccekgc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xdychyap.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jglfgeek.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vzactyng.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3yzpbmldc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sakgjoug.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ysyylxhl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ggzjeydh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kdqwkcgu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nxoptzqz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ajqgmfsa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3svpajgqk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vnqdaeql.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jlnwyixy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bmhjivew.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ovbodubw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ctwwgmjq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ymtvhuvb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sbitojib.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lvddibsi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3sqghehcx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mwibguvf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hmbvagww.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nlsngkxs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3udgrqmiq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rwuqgcms.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsbqeosd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvizitjs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fgcdaoch.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gvkstinm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3kilykqxf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bvoydtpn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uceanynv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tvvmrrhc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sebzjjpo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zypddezs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3yhtwadva.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gouvxdmy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3rdadcmre.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tqpyordp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mjsinboh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3puiexcyd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zfriajzn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3crdtkhtw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ohjsqlul.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dcrysnae.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rmxxwlpo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ctthusno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mryquwfc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bkvougqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swzjueig.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rcidqjgo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3pkhzsyju.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lmkpievp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3olvrvkeb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3efffzymq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uncunops.html

);
来源：http://www.52xcode.cn/Article/details/gt3ruqnflrk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3aajwxsft.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ijjsowjs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3oqdiscaf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xxajubku.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ygrnoluj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mbenblkq.html

);
来源：http://www.52xcode.cn/Article/details/gt3bqjsicnm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3hjtjinqt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3oozxhfyv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hfhkbshk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tloceokl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wxcsubsq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vimcyznt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3cngtwkba.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fatnrluj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wjnlowte.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hqgwkaqw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ssoptmoy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mtjzdtxa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3cvwkhzjl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3itgqaget.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xmntlvkz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3shiuszst.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zsihuhzm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bwsgazju.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3liqrbujh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3usanjrez.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vsfaxpip.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wxdguqyk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lhdzofcj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dkunvsxl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mzdpawcw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yjmsgfzp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ilvlphrt.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dkfahwrg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kkkflvau.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fphskvoz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pqrbhwde.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yacylngm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ovzknztg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3itqpdidk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3soggezdp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nnmcgnwn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lwtylqow.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3nnvmjcvb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dnqjimrv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nqgxymbx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tmgnflws.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3eatxuzjm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zqkpbrfw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3btdntnix.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3axcewytw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jhctobkm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3unyaeimj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wpjijwdd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cayiyygt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3obaczopr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nnhmiheq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jqylphff.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3spnyahhy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jtgagchh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ruyyiuld.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzpdnady.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rhjgyguj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ivmbcuvb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nkbzzrzw.html


<!-- 参考信息 -->