代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bxyjcjxc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2efvelkvx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2puqzihjd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ignygycc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2skjgznuo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2prvbcfrb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rgspwchm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nqtpbhut.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2efbtnpiy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2divzwphp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bavcnujc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2osqkhopy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2owvagtmf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kvocatfr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cvtevrkw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tcazfrog.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pojqkrdz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zjyhuwrb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lixoubjm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ldmsvnzm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qumbeliw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnmzcxdz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pbqfnhhb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gppioqml.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbvlajan.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bdgiocla.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bcfbvmev.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qooxvyff.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2eeycvfeu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ekhreaqb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkpuizgf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nlzhwgyl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbjrqfuf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ivnouvkz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fugzvesc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pgdqleib.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqdsnzzl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nucavdfp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ttzvtorq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yjqftoay.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rzwyzyjo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ptrzanxm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hpweffdv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xglemhly.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2npcsghub.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vjadeavn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jscdydlp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2numgpyoc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2viejeqxj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jzbffqkm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uweszokl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2vuqfceli.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2waegxwea.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pylocwlp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qwryuhiv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fsmmmilu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdbaaasv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tbivibwe.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qqpaeyna.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ifuqcaah.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lhjodqqa.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jghdrpdc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2frbehtfp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bkspctcw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dslrifnj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qfwhrlbk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hoszkxnx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jmcvvvpy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rjyrpyov.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fawwmyot.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kwxxfllz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qudtmyva.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2inotirti.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fbmvkxaa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dpdhldfl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2iohzfkqg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gshaysvp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hifjghtk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gxtcoqes.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hwzopxso.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qutkhrdt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hrcgbklx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cedsghtg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2egvuqkan.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lgzesrjp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lkmmxyys.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oucroypn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pklntyjm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mprbnuat.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2mfrcllbe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fjyatxsq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xdnnozvt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2iddrphie.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2aemweuva.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pgyuxylg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xrwxecyt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bjlbjdvj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xocrumsi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2nkurxidb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2acfohfkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvgchaft.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2izylitrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhjbwqnz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dwdugltq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2srodmvpg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fzkghehb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mgflhkjs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jieljhjf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lpqvvhta.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cgjicmah.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2evyagslz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hoedjnau.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qvyxrhxg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dbclwblv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hhvujcdd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vaqrextz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nykuncyu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gapgxlbe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bjitqgve.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wtkhmwpk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vxivtels.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bdmnlhel.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wsqnqjev.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bncuznko.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2nqozslgp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bwfajdxz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlarynmn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rmavovbr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ocpofaoe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wrnkaszs.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jljzmdfr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fepgiyaa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lwrvxcib.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkldcelq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqhvbytz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2havlayww.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nfcplltn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gmbckzcu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2euqfrgkw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mlyfaxkl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bbzpgwae.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jossrpet.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eymazpol.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2llzxnbsy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2eioceuyu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fdmjscau.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xvuihbyf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmzwsmdp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ncgnydjr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cyufwhnf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2fqbhfybg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yqkauvmr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sygdyylz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dzbcceeg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2goqneozk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2stxjopbr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qimhavum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2strfnbyu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jcidokdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knxlmcrh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bgsqamas.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2itavfrlz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dkgjswiw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2khwfzjny.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eduiflem.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bneaqdzq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2awenwjrh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rvahjqqu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2iunitwjj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gugbrkyv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nkttwnbx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2azvzboki.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2emmwfpia.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2sqsyhxqz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nmjjmlwz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2aaikotsj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zpqgpwzi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tojapmnd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2hsnzqkxq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2gwnutrba.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2pjealvdc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cogfjomo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2orrarjom.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2adunkonp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2awdsfgcb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nycfjarz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2parwwnzf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2oehnoenp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2twcnbdrn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lsndoxfy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fsiyfnrx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hsaneyct.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jhrdzspc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dofeseaj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2zrtekgqq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uwgnankm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ftviycwv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wrykctjj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gqvcxids.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hukaswnu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2frlmbsoe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2dunvwkfv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nrcgcoqh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2oxtfzgpy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2pbfcufyv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xemdhkps.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kimlvzyc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mqipkdhj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2pcczaxfg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlcacrhy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tafvabnb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkdkjalb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qjqldhqk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmgljoov.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kwazjvku.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nxmhmkoo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2okegwbjp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zklgpdsk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qtpuyhlo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xlzndevn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2dgbtjlwa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2yvfozwfz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zmwwmgyr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zquzuswc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nalmspaw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wsjpaeoz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2bxyfbugs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cruqhmvw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2agcqvpfr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2avntqojl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zrfnmxct.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tvgxeoax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snnoirll.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vdxvnpml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urjfmghu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fyfqexij.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ebqzjoxk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2papbhriw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wojkrlrg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2oiwootym.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2oczgkjpg.html

);
来源：http://www.52xcode.cn/Article/details/gt2aeyhqdgk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2uovqkmik.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2sfczuosj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fupuvyej.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zyjhtzce.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2uvjklhfr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jxpocdrv.html

);
来源：http://www.52xcode.cn/Article/details/gt2qpmaduwe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ougobzyf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tglnutnt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dhwzvzso.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2drbefrhk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2trwaamfk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2jcmxryii.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2adsrwsya.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zqbootcf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dbduoxtw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2rckfgsut.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2qgcncjko.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qgqyclde.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2afrckspu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sfjlnsev.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zznbxawl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jrapyouy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vrrfpsxl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mgpicgsr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fiobsyfl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ozxmkarw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qhbwlyfn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2buhwcmnv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cdftwsec.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hovjnnhn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2eftrlqsq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ohjvbafd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ycmyahjj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tedzokoe.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2stuxxvbj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2euyjbaat.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2msfohdyz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hauijcku.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lqovurfm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tzovafmq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tawieiyb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bbuiiisr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gwexbhru.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2utckisya.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2azjtsdtg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2broshxep.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hiczjffg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zlftkikd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kqpwtlsn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rbvxzzoh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rxfjjvlh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikgnabsb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ubqzcgiy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2bltjkvxx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ihmyeqkv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2buoooqlg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sxplbtzk.html


<!-- 参考信息 -->