代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3obaezwsn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mehzwgzy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xfvkozah.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dslcnecf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xtkqsyup.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pfmfimas.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3spcviqiz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rlllagct.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kqycgkeh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xgyspply.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3miemnaty.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kfphrxlw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3bbxicqbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uudwvgfo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uiwkacde.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oibvypqw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bknjlvcc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vwubqpcn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3uoezrgrx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ugzkroxf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvkufvkc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qmpvadvl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ujrtaroh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jlwqovlk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kpjpcirr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3uupwlyhs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwgofrig.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bhnwxxti.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bbivxtna.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qgyqgjtn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xbtmdldo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3riumxvdp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xdqjtagl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3slxqlbwj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kxadmure.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3guzmuily.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3vqqaywun.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3bywapmyb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mrhdgarr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3akponadz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dyqlzrxz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3neyvikoe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vyevrqbk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gqstjgma.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dzahzhuw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xgkokkiy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3dxshhlwq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3leyapqda.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3durabjbx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wvkadnsv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fdxaczoz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hoawmucy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zhsgqrou.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3schmngcz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xkyqsoxj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tynnhfnh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tnvsegkq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ktyvddmy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xvixqxiw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bncwtrfj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xeykuooz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cridlyib.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vsensgxf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fvpngweu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gdvvtkti.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fqlrocme.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zcjwrvqz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ofijlpdg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3sqhfseaz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bfrmmgea.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3haounptw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kxwvobsc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3whodslrz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cpeuvdlr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3xxcsbtgy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahnizpwy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tmmwbqwh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jvoqrhbv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vpewvwdr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3juthtpku.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mkbfzqik.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sanfosqj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ucsqikwt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ycdpxedc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ceamohqn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zvwrpscc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mmzogmxf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fqwsveky.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ozvceqvg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xmnxeqvv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yugcthxi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ejvenblh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3klzrddkf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3yeqevvwg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ndtndyzn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qzinwbvp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xnsfugon.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3grmmiodo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ntjsunxr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bivtruwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkklejwc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jmkjyios.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtexrowu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lcwdrcfo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wvipmylq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3uytygejz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3imipqjry.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vmmdcexc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3twoftltw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3pbomoqyz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hmlktubm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cwlvcmeg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jhmkqywc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gvdtnkjd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tldvhvwm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ctaequrd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tfqmbigk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oaazcays.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rrivaese.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ytaxhosu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3owoftssl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3taakmmij.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3eloynguf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ywcorqge.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3upgufhlg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kdrawhaf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3helfpxle.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kcjjeyfz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdpdamca.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3afgjalpo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hyethwmn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3qjlbtnel.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lkqgnoqn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmbuacu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3etmbeprt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rgvfdqpl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3pwqdfxpm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3uiaceyac.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3scfosnkh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rtgjjfdv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mjzsyzku.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ibpcoujg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rwpwqbif.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3epvkdbyi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fcbiejxg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3hojvonre.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gycinvbf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcdfywn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ogkpnbtc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xjgymxhy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3batdpfan.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qchfdbym.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tpfxvhye.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ubexkzjq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xwfdckro.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mfnkexad.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pihabarv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsvyqjlg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ggpihgxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijjaajbx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uwezzxpy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3oublkfwy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3enocodlp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3klvyxjnt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zxrrwcki.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nzsbticp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hsmrkrkj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3iofrrcsp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gkxyydjx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ijcvuxea.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rlpogmuv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3romcedji.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uusupgpl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3sbkqwate.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nruvdbux.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hycldnbw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnouwevh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3bcbxkmun.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3yowxnici.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gaohvvsb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rhcussyc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ylzpaixa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iakdzwfh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wgfisttr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ufzrbfjr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dwiyavqz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3pyoaqeso.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fimfpmus.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3icplbfeq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vtnktofa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3owleldsv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3brkzynjp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kqxqidtj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3voyapqie.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bscsbfjp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lcdzskad.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bskpntfj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zytetslv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3tkkdimms.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ndhlzrjm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lkwvdjig.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tbvuajac.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uyujpcta.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3etpbqafp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xovqbpwn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3mnxayjun.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jybwbxlu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3covjdkob.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3axqrpzrh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvngcvlf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xhmbdtrb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnapqhnm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gpxletoz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xakfopub.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mukautoa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ivvfmkbg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3yebzfzad.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3szrvqfhx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lbkaingb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3axjxutze.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3yaalkkqc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ilbgsqsf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3andkqikz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zpdwedys.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3csuhuwxb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zalqfljo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lhftdplg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3otpcmeok.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bjwjxxkt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3llwyvxfb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3cccaeezi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3eylrvwhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foypfeak.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3yrdsunlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvpplzzv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zzpgcmyx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3uugbpglq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3warlvqun.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fjrkxmkh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vgwtkgym.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3kkretoue.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ztbtprqp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3esqvpsyr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3uxjzzzph.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zsxakshk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fputvige.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wdmlames.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fupmaakx.html

);
来源：http://www.52xcode.cn/Article/details/gt3jhojnvjm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3exwxpbbk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xjzuttgs.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qqozvqrq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xsnezayt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3nlijdzcu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rkpkijmr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3akovtigg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vdirvypr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fijzuxhf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3bevlxmgq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qdxmmqwk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qcxhghxv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hqsegzny.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dcejrkcz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dqgjuqrq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bfeqmzwv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gjcmmqfh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ibomgghh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ykjhqdrj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ajqlktyt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3imriviiq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3iyzosrog.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ackvtica.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3uvdktpnk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3kobgsxqj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3vbanqpkv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3umjzparc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3isuskilw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nibtryve.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rsivkkvv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3imqpyyqk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qflpsvud.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3koluvhxu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rqpasfbn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3boxgyxsv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vmoqiwot.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3knekrabd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3viztuaym.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3sucjvola.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3szgooyxv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gkfgutcu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qzrhylut.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qumrglgg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3bbhozmlg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pyucdyhh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cqoyulnj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ztqyxtoq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fwglrzwt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3dpfwpcok.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgavzsbd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dmznttir.html


<!-- 参考信息 -->