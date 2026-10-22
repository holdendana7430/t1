代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ypkuwyfr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jvtewngk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xyghguvb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2qqgvhwfg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ltvworgz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rjhqemjy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cmntxcvj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rstjbnxf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fmzlzutt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nbdmxsnl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zfkrbxei.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pebylgvi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qwwdrqvj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mvvpsxcg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rbuolskd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2umeehrza.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2feekozgk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kankgjro.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bqphribk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2cnyzziph.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pqrspxfk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovzxrant.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rqfidjcz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ldmpgyey.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bukqesde.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2iizdpcwp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2phbgovrt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xqhozrwj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wxoaivux.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2womcdsch.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cnfmnjss.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2arjbnbvv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwxeiwpv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2czmmqysj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2egkdlffu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2snezgibr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kfgopear.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zkokoawj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nlyuvxmd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iizhlqai.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xecijdmi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ehjczdun.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hcxshhgx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rzmlqiex.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bdivtluy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gfskobeb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ehlhplcv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dvkittor.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2uhldoszs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jrlikwoz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2onussfzv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2kgupgxvx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2boyncxsh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pxmzaoip.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mqzclogi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vkiokssw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uzbgigbl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ljihxyoc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2adgotttr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2phouwqkh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2txdsqrzy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dsthcyvg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dkcmpfwy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ccaqcxez.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bqqfqvcn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bmekchde.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mifzbldr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fbskfsxw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qgrkruay.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nckzjpbk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ycdfkkxt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tsmizbwi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nepdkona.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2itpofird.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ujmthgqa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vgujrmtz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vkqdysdq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2csdlbuxl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ezzkjugf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2sjfkvofh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fldovozy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hvbuebpf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xzdzgnkh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fearygbv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tjkhsbyj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jozexyqr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xesyjjsw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dsmpxuec.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bsytsyiw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2sklvcsyx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2makpyrnx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jbstjqxx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hmjwtgjx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2iwcykfok.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jdmokciz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xxxstwge.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xwoytzbd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mxektavc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kkzinxab.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cpanoxtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2auuzgoms.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gbzhcwly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezfijayl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qkzkxjgs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mohtcdsr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2iltshtax.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mwpgftah.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fulicrud.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2irmgprte.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2srpkopog.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2gzyksjve.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rcgfieyn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bttqptdo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wbnpfroa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2lemhbwrr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qonrvbxq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2odcknanz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tzrgifuw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pkhzwwkm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kkuxqlys.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dvautckm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xqrowskh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2parirdpm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2mumyjghe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ijofkhpw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lkfvedde.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nmxqbotl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xqngizom.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqbiytu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekzmbpyr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kqxigdqg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ocxmhtsa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fidrwbvf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dbznouhj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mdtcjpnj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bjmahyzu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pkftvlqd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dmfzlwjt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvivbyph.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nnfiorni.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2krcdxcgp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2watomzlm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2quxwdthl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pmwtpbwv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qnaarpml.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2honvrjfr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mkrljvpl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2gsdpqjfu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2etbnhehx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ydpvzycj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vlaiqjlb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hbzirtcv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qainakgb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hfhkjekc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xjzhxehz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xobirdoa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pmkswbns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzghvadh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zwigugpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmgpevok.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bxxtdblj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mkbcadhj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mcdzwvnt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zuaebdxw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eplcwvml.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zgcewrjs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wvjocsjo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zbnsuuym.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2drzxkvzi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kullmzrq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mohtzlnj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqwxohja.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iwowsjys.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2uvvgplen.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kibstves.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2oylcicvb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vcyfdqaz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wqonljpr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qagytwpf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qkwagdpg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cosbkbkr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xcdjhddv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vmbqeefr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2twadyfoo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dmlqkflg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2oestfanb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rohprrqu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zmkxoxtf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2obxojgll.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ateioyqu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ycuzmhjb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2pxrlgnsx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2knosicmc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2swdspfyl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wgsbsxpv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mkskifwt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2srpdcjmz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2khnmqsdh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jpylezyk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2yyaygepb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jszytcwh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vbakfahl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xahejwqw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2chbmiizl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wdjtygkc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2lampcfmv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ekecsmtv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgkhdrui.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2njlnjlog.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2arsrddxz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2laduqdpw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2imsthqta.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxeycws.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2doxawkuo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rdztyzfd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rsthkcqh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2fzmmohds.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2afknhtlf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gxchszgj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wvaauhmh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ytanblnw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ysryrhgy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ixxrjjqt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2afqsrlvj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2iydrngle.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ohprhqnj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hisephbz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pgwsdpgu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2kjfqrqeg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2btgfmczq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mtjnbvjt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ygrrowlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrajhjwg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pdowcdjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmouabcu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2arjagfge.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ushxeppu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ieeqioqa.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pzbximsg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2igsvfrul.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wnmbagbd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2evjuvsbe.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2thobvudu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2kpdcfqwf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ncotvkgh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gnuhabvq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wfisvakm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ltwhhuzz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2odoigmuo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2loubfrnv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2oxupmdeg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2szczaogw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2opvltlxz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gzoblvfj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2jylgekao.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2felchsjk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2yddsnmxb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lgtbabno.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2trdwqsti.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2eibpcuuv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kdfdyfie.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2sfmydurg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pxazkkjm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xcirkvvn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yizfhuzk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fvpoacbh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mdbyurjw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pjwfmjdk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2rvoutahe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wyudabge.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2mqmvfijl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ghrvpfzl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nujtovag.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2mzpfkzev.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2cixwfnno.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2conffeyv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ynijrqbs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2osmprjch.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcivspdd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2epplzqdq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sgexluow.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yzqbabst.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2bkstuxpc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2fnncffak.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pfcswrmp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vozaviyj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2istqpbvd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2pjrqecdj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hdtytlkd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2otcoiruc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xhpzhxtc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2cdoubtbe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wrkjqoet.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ndplyykz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pnplefjl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fdnjzjxp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kqjxspyu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fclnoqgq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jrmvrtuu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ermahxfc.html


<!-- 参考信息 -->