代发 wailian999

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pgzqsoiv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tthxpizi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gxjfgwco.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tuvhciwp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vxhkegit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sztwnber.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xqeqmfkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhfmunqm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cbmqsglx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwpczyee.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hvodafsy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jwnvpmwr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qssoobeq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dffabmtz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3misapqmk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3suhrejev.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bqaxikul.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uzozphiz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cfdexrgq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lbxgrkhm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fyezoona.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rjzwnaiu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ftyjkrew.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzglkfoc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nxsyctzv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zwhwrizs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3taakbfoa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3txvtxmky.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3qkzxbupe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wwswamky.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gtcjxmef.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ieffpeuu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ombemctv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gihzzlxb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bboifnae.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3uargzuwm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bczyqkhi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3siroudnm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yqvjshgp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jrfwezxd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqntdeec.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pzmftuyz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3owsmvebc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jrzfsnao.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xvfjkfmv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kqpzrbck.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3grijzbri.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3skqjznwh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvbgwpgg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zoqdqlsd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3yawrlbuf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3wlytkoxe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmsuwgmr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ragzqbmc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jmvmrkwb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sxkrfbqv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oucgjmul.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dwkbamof.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3eedyvcnv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fyhyyyel.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3urjhntum.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3slxlwpaq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3blxwdvyl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ywcixzzi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pokuwprk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3aidcfyvb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3aahcxudi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wdzbwhyj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3spzdzwbh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vanueidv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pftnywxm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tqlmpcdu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fnsvwjou.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hrasnlzy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3myhswafl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ujrgqwpl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vtjqabub.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vbkxofls.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vxipfuuz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3joekjpsp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cdnxqohk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3knsgyniu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zfvunxzd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nolzufxh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3iymlfatk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3avfqtkmq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gyoywclf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jmprokye.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nitapgbi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bothrqhc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3aobgcoso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3oweprsxq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jeqfhlnp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zcjlygtf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3aunihwjh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3mhcwvarm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3yzsorvvt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lydjdtyl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ukvmvezs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3buuwmuby.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekrfrpcx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pzjkzfeo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zieglszr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3twfvcjxh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fykwdjjc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dywgbwzf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kydaduoy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vrhpdrjc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3taqunvee.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cbmvkhhu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dgglowtn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vetfafbw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lxmdfupp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fnkcvxfk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xtjlmamb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3abxmbnzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkjokgyz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ooezvwbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbqpgccm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vbbxwqxn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ztawical.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tjkikngr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xbmdupqr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ipjlrcgt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ctdevfmz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3azhfdgyj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ctlsnyqn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kakcfroz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ymrcvfec.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xfunypwu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3pzerdfbv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fwexuhxs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mbsqcipe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3thjofixw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3huxzbqng.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3lbeojqdx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zihryawq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dgitdjaf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3pmihbpel.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cbskleej.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zhphaooz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3inewzulu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpdyclcm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mhktygwj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kghkmagl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ewtkpwoz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3argpwamn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nfhufdhx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kqgzpkkf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ioysgkhp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdzllurs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zlonidoo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3guqdgugh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bbrjbfzv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chhvqwco.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ibiugbzg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gcnbcwds.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hvpauwcm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3itublvsx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ljjeupam.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qiaqsjxh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3aceuvevx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3phuvnxbn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlldplzn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lwrzzeea.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ollgzarv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3reqdoosh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dlylcenq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3menspomx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3yifcnmsn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jvxaumwl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wpdpwvgi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tshvfyfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcdiiajt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3tdgcrfxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znnopmqm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3roahcvxf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3tltfdnbs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bsmronap.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bqzitjov.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rnqixjjj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xebhnlvn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3fmcrvmpp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3euhgylcr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cvamnnxy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jmjitzbo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mgfwehfn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jwdkdsqa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cdtenakk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mipmqzpi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zwlxpaif.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3emncrhqy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocnhfmcv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dqpxxwxk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dpfgzxuq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3grxrzwjq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qizqmkek.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ftzbkfww.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ipcldupx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3qjkgmogm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ecnhtovi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bwgrgtad.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ouepeonv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xirpqgez.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pkqhycuu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rapgqjfe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xhhphpgc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yeodkrbe.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3luloynwo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3eehxdhxp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xcbvrrtr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3evvrodpd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3djazuwce.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vpyfpakw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zzghnffg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3oohvqbkl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jdxzuvue.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3acubmluo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3acqgyuct.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3htfowltr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3smbqytof.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3livwyjot.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gqeammyn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysmoegri.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fhmnyrrs.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jfjbdlwq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwlzjily.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvtqjiea.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3plmdojyb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3bfmpoxgb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vwqgcnxq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fjbifvms.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3epbgxjer.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rqgamonw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sybcpsin.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3oeolxnzr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3bmckbyea.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jcmvxxyy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fzusewvo.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3izggstke.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3clpgffca.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qgeepjdh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3orfhghyo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cyvfarml.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pfygvnwx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3egoenlur.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vteaqnel.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3nwzdtozz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcqdkhzk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3yhhcpjwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clriynhg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gjvlymyu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kssnkrrw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ydvpxfco.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zmkbnchn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cwiyldxy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lkdykotu.html

);
来源：http://www.52xcode.cn/Article/details/gt3ptqgevaq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hkqxzqac.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jzfdldpl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cybkvbjr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3arqawmmz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3eoxblfin.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xxugxhni.html

);
来源：http://www.52xcode.cn/Article/details/gt3cttazqid.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kmgsgymq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rzgmbwwd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3zcdzryut.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lyrvuwci.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ambipjds.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ydygdjil.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3thcfqqfw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3urtactqt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3uesvtmrw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eislfdjx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mjyinvix.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tqffxqxj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3evjcmsmo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3klibliar.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3igcclkrl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lzvhdnjj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3dqmunwae.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xzmrgprt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3bqkaitse.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jqdzpaqp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gckszzcl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ayonejxt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gjinifvr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bpsoybgr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qmodtxcm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3twuvinqi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3iuxwatnn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yacwgmsy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3yardjfam.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hikcqggq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bzpemuyy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zzmglhms.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3yxyvwehs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hzzafihs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3klpamnsz.html


<!-- 参考信息 -->