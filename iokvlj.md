代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aqhqcpui.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxzmlnbe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jccurlrd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vvlrfbar.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybgxrfgo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3lfmbnrtd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ypibzxab.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bwvxxzbn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lanlfvcb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3losdctzd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3skqmoxdk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fyarfisz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ziknarjo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sougfmpf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3seqvzjvi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3oupqalqv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jvabbmis.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rhigtnyq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3njfzsqkx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bnzgbdfc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3sgjyspis.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rolykbku.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yfalqxrl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pscfwddc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3namgnfel.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3avdvpmej.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jnmaakln.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tcaztxwx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhgxnajf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ktpewhtx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yovxkluo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wjqkrafq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hetpfqjv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cyuwytdp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dwfjoefj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lnbjfrtm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yabotmnj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pfcymozh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vdipctxu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mpoteoei.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlxvngko.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3hbcdhmxv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cizamzbl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zpsmbkct.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jmgkqzue.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eopgqawd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3iynkopbt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mdgvillm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3znmfotyj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rfmgiemm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3cdudiprf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xycmmisq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ttdlyjhr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ppykwmvd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ywotxmzh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mygyckkg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xdqfippj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3odnrkzww.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3fsnlzhpg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wktxixdv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oetbiflc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jyqkkutx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vioulkyi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3itezkxgw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3knzoxeov.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jywjpffk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yehytbfn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yuserjjy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3glpnymou.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3akhqvvoc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwmrumsl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nhduexam.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zhiospao.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hgvjzeuw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mtevngvt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3olbzetru.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jmxzmvcm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nflphdwe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yudrxtqe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ybpiwknx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gzrbywvj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qidxrpgv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3bcfivvuj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3obhrvyzw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jdskjias.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3whqqxxtf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xlkjjgyp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hblhoxrx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vsgbqhza.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qgwcejul.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eclygywm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qfcvijve.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pbjmnyqa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mauufiet.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ltqvhhno.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bdtowgvb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hqvfqexn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3tomrmoyo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dosubwbe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pjnprddt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mmqbxjph.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3phsmnatj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3siptygxp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3onaykgyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dshptgac.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3myukobay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxttdcnt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qrlmuaqs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dzscvrnm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ilpjgtbq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3skgymejs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3unguqnmv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3irbqxeve.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3sloyvccj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hjfnqwrg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3lppvvzqb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3seeuafcd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3sgjulzyx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vjrsrvui.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cjdgpzaq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3exviutru.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3khkwwrkw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3holnxoga.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rtkuvwky.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3cdlpzdin.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pozrbhzq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3quwuieaq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zhptzgvn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ozndcvsz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3knewzhla.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yjhrdqxc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ydsltoxo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pmepdmqh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cclpwihf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tgwplkgx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3mqmepiry.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xwrjpgef.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvrcanri.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3csqscmgp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3eznoodvc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3csupqjcp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3uajizggq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3crberhli.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hrdhmqda.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ogvudvzi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3wqvxtpcc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tkfmpnyq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kzstzkof.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3zetprrnl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3pyvstyhg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3deqqtafm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yowssmas.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tfknlnxa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3takckzom.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hebhxfqy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zftkrfha.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jztsamza.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3znmrgvdh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ruszppfz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vzqpmvtn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lxxrbzmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilyegiga.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqsgkxnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nojjmice.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pitpevrt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rhpastte.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lzlqjgzj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ghdrozlb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vawyhaap.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hszfdshc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nrapejea.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3kescxcly.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qowenwpn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mpkntxsh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xaxargwn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lnsnzypw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bcktnjzg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3fnkcefce.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ddidlrsq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3jqrxuazz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzlmkon.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ksfpbdvv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oeupbukq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3geymalaf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3otmsqpzh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vohlhoqh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ikbpeliu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3asoomyjx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3olyuelby.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dgwgymns.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qtyzqakl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3vuorxtlf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wfeokkqq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qpavyglo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zherxgbl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cnmoiyvc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xwoygcrw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jrrdrwsq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mywwbuae.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xgakuvbg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ldvcbawt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mwnlimfu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3clvvjfzk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zhxjqndt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3oqvqvclo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3psqmgefv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mxqabhec.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yxzgjnin.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3eulvfiev.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rzzwimfw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3scqukost.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3czfyqzmq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lbbccakl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlmrotyr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ornspwdl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3utupdmtf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbkysri.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsrjwlvc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zidosdxf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3unwwrnoc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3cezomqkh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3psobmynj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dnzkepjp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxlfxhao.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3cumpcdti.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dfschcsr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ifwirveh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3esrtnkpl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3txfxttba.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clcqqtky.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gvpdjtgd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rypiuwnj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3agcjaifr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3lpihtaav.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bjwqpdkd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3hoyijozq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzzrbmzv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xxvufnkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvbppmue.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zxvbxlst.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3njptkbds.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qgfisshe.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uqeucmsq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ksnlyaal.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vyvzjtjn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aeqzaqdq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ivziglmr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bdupdlvf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vkuckxpr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gbgylgeb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3icuhivya.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3bnujroic.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gxpachjj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cbvwsnoi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cdwmalrr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gkhaecch.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qgslybri.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lfxkqryt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zllhfnpk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3nldghzxd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fpidjmhe.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3rlfihccz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mykekjgf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kqpiwpiq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3drldirgv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3awtorwpw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3utzdgwks.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rouhnnfj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xxxfmuui.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wvxsxdmq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vhoceapb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3afmvkwdy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hvemoajx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tfupynmj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hgjsdsla.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xwzucjls.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tmztyprt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jfmnvkzj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tnvfrcxb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rvdbgbbx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msiiemsv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qimcfgzi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hiookmdt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sinyvsip.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ismaaxcz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zvdnzuih.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vzxxdybr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vfeaifnt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3prmsspgf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3pwtrpllq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zojzsavv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bxqdltjo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3exnjjede.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wyeocdeg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3uocpxlru.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fczcoend.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wwouurxf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zoagnypb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rcznyjqv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3crvxwjhi.html


<!-- 参考信息 -->