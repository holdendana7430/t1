代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3odwkwcnl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jdhmucdy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3myomivdw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3pxwapgdf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltlmlmiv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ffocalyx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nompxtxh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xtjjsjjz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vrcapkkk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpyglgrv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zuolwzpe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ubrwklds.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3huiyrnmv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gtkeuswc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3eyywsbzx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tgmlgcqx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kaiixczf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qjfzpfnb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3crelfjpl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cqwwxjzk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tnpjxspn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3dsdebiuf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vpotnlsz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3irzebssw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3blufnkaq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bsrctefj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sazzecnc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3koosmqvz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kbnzsobx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3uriauzfw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jskqmvxa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nitzbioc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ymmpcjnu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xgbglgdb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcenhgoa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysyudjkg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mebkynew.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3duujqswb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jshxdokm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tfyjxpzh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ktmajcyd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3esgyaedk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dqyzgjjn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fdccgich.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdfmsuuk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oypjofev.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3gnwmfssj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ispinkpm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qmbbdxkm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3maczzawe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3popnfekg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zmmgiplp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rwrfjcno.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3muqclntd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3cbwilyul.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ptjburbu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ppvresuf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3eckikvjw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zxxjxixj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3srnmfwvy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qibsfjif.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cluzofvn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwwpmgsp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ytheknwl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3expuvibg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kollhqku.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3blbdodlk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gzvmzqlz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3slsnxion.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jenrhzev.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3crceusql.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xnmovwpn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xifixcww.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tllsnrbz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xkavbmds.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ihmugnzx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qtbyyquh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3arnueglm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3poruxwqf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwegcmbw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3uaoxohyz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ztswbikf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hilmerhx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3thdaofyv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ajpzwakw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcuvdbsf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lzbaiijr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mxgilpbp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ewevhovp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3trjulkif.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gbigaxab.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sreerzad.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ysmpolji.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3mvqklhpi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3atjwhwrd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3aexdpxfx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3htpqwfzo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zqfiyvbd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bnvfkinv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tfsptmyi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zqwzgfek.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3sinmgeuf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sicfzxsh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3grtokvuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osfqcjrn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mmodaeoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iosmipkz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3anicmfdu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hhpekrxk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dbbohdau.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hqlofeka.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zsxzxuyk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wlpghifd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ykzdvjfv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3snkudclz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bjaldceg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vwpcldzl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3gqxiypch.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3wjhyzusd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gqfplsvk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hyvgzxzs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3iwjrolfz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gfwukriv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fkdgimkw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ejxfkpun.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3iwplmuls.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnukekrr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xvcpxfco.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xochrqfu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qgmbsdvj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cevspkpf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xfarwenc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zwrifzem.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaumxxma.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tmazegts.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ajzcxqlq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3nlxbdyil.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3omgqfmyo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyexwspd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jtzuokme.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3iigehkxv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3uoomibsg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3aavqiayk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rpohkovv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3izydmcld.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jhuievnt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ojrreurh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iqunqxgo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vjhemdzl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rsivsuel.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xyitvsto.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kgwyrtms.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zlvrbpfr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kciztsta.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3rimwflgm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lkljccal.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xcjwoaby.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3cxwqyqaa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zxasebko.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vyoxkcxd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jnyyhvci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htiiftcc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lhwotanp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3envuxgxc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ieuqhuse.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vtauewfr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zvmdblrz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hvfjdugq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3amljxvye.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xsymunlj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sfoamqec.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zeuaohls.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jntgsmgu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3bbserxou.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vfcalgea.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3flsydhdf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ldgfpcti.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ackbeboh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oxgpyddd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dpscidam.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ipdhffug.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3khjyrujo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jvxjojps.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kyqoqqna.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rjoaqpji.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rljdjopb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3chuvnxjs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ztdpykjb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wzjputkl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3onmzdhkg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gfhlvhhs.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ymcmbjam.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kpjkwwia.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xfdwwfqd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3apzhmpfc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ebmsvdkm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rtjzrcgd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bnapdsef.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rqhbgmfq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aaxffuqd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hsoqarxp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dwwixthp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3agwhdsju.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hvoksbsc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lnhxxibb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qahstuof.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3leikvibb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3crfkozha.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jagsqnfk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3clbiyxxn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bzckwkpn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3omvfyhkc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qqulymfl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nzbmxyng.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qqozfykh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3abewbxac.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3nnlzlcbq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibkpsbnz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lfdyxghq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nbzgkszi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jvjppolv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xmqcvsrj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wlrywhhk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlcocxhy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rtsxgekg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iuxjmdza.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jnwtwazd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3agolxefy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3yrqdypah.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3scmvuwmb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gavzrmqo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfwyjtoh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kmotusvn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3hkcybiqk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jnubwmwo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zulxfcrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuorffse.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3dbmedyvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjfbppgn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3dvxgenkv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lijueyad.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lxhxagsc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3slwcksjf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zrfxcrpi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ypyccnou.html

);
来源：http://www.52xcode.cn/Article/details/gt3kdihlguf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mnhiwkgb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hzzwhzat.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3eqgavjjj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3puqbtdbe.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mjnlwrfz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wfprtjhr.html

);
来源：http://www.52xcode.cn/Article/details/gt3dkngbvkb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3sfnilipf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3slhrbfxv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3posgucrs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qhsetcpr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yxnsucmu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3csvdqsbo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rbrmsycv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jhnukiqz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vgtcvpqv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jgtjkfgp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pmydwvam.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bepxikjs.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ddadnlon.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ahxpwjzq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3coidvtdn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3srlzsjpf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ljuquqjm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qbbspxui.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mbxrkpzq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wpvmalpq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lpzqijqc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xhttbytc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kxqxkzzs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3lhsfnwhx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3decnqfci.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3klpkwrpa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qktnnydj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3doslvsrd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3erlocrcr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mghdjgay.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3cxzpssfu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3cyfxvtxc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ncvgmnkt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hfttnqqt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ckuyhfio.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3flhvjgaf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nisjdvfx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cociavpk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dfjevmzp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ykugnqgk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wdyjbmkv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3lmelbtlk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tndnmbmi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yiwmfcls.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lwmcbchb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ofpbhdli.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lpbviqzn.html


<!-- 参考信息 -->