代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybpmdtxu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kiyjdivf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pztqsnst.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oesvhtxt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bvwfojgh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ncgcnuqd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2isdrynmd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obpwmhmr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gdbavbzl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hqsbzshb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2okotwisu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xcbciywj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2svauapvt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ejoqpytf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hzsvbsgp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ymblbsfd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vgmgodov.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qmdmwkoc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2akhlrlzg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2irnjhesc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2googwdij.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2znaljsaj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jvkaixil.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bducgzcn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2spiavwgz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mcdjloxa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mvsjarrb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tjgjdwxm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ryzvymjn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lmstcfzy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozwvwbhv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyrtyoxn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2acjlhrlm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rlzifeoy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vekljjpp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fomhqysl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2yhsblwte.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zhuuoefa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vvmkihdj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gzinxkmp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gjycpvqo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ihoupihe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2khgreoww.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2himouwyh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rcisiqyy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bzqsozne.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2atlqvorc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vguoctkq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zsojuruy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pwdwzifi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ivqeuzhx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2eukrqbnu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ohoxygqt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2erxnmcll.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bldvdeui.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2spokphbv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pcyllpwu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2iuicnrve.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2swphmzxd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lnpirdqa.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqjuxbcm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uhhdaifu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ifoquhfz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aeootkxg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dmgisozl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wjlwbnew.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fkmpjosg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rblmgbsu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ujcrqkjr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mzgfaqst.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qniscouv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gxggsbni.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vqqkfkzn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rggyytkh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jyzkvgyj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dtbljkzi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ghkmnlcz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hgzeysme.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2trtfblhx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2woocwwvl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mihzjszx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qbnsnrcu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ffpdkvgw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ojbttprw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ylvphiwc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gyeymkov.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zbimfqls.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hytkfevm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ihgkngcx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xpssmgui.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jjtjclmg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2geokhwxu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vkhalitn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2sgyxjixy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tsxoemfj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bnruiqxk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bziyonfa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gurlksfj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rbmpgfib.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nfknmkqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjgjeafw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fawcsbvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jslbifkh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2odkdtznk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ntsaiamy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vjarpefh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fudynwjr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2warqawrq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vopeguze.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nqecnjah.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2cvfrrzck.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pfwsafqx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pgvklsyy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2erwfaaqn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jtgpjxzh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nzncopgj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wyjeiupq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2luywethg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jsptpzpf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ivdgxpet.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2saclymlo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zxelfekl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vnlkltit.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qgitifvn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ndngvyet.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eqqduewl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cystkqbt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2irxukwbg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uqpmmxmt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eywrwzgw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2unkdlezk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gayjlqwv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dvwhwpla.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfuifcos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmyrxuud.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2doztzbay.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gutrkwsu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xrjqxgyk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rshjrkrw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gaxeslia.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dqvvtrje.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rjoyhtih.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cdrntmeo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ojeskzzv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2izmgfxkw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2aqiqjtkk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kgpoewbe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2clwqbhei.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qnpgamdi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2gytdrqax.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wehdwkgz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2shvpsgaa.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2svfaameo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rfftslxl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2orestsph.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wbywmilb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xacoyuxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgiorxca.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cshzqage.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgwhuozl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2twjkpfzd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dkgidkop.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hbisamuh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ybnkrhpi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2olheuegv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2urreikax.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2sijhcmca.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ptohjakd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tbqybyqt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xzyaqofv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2lzmmwwhf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2hiobvrte.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2azfiwosw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bvuozmki.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wyauhdiq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gaueplng.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqscvzwq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ctrqhiyh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nvsjdfnj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2efkmtjxl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ndptepfa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zyvfrzcj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jbushgvc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pjgdlyiv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fgnnbcle.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvkezue.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2kpbgffdj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zrecmogz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ebfzgwxn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fivnibiw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2obkicuwz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qpbwiimg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2usqwioef.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rctzyney.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hahvhtah.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qvtqybgo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2bnlnujeg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2iphryyqg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2oermmpnl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zaomjvkm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jxfyegfu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2uebthsaz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jxxbphsa.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dhrsfqxy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2sqpoqjfu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pftnhrbp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nfajdioz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgbpgden.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qlkgkhvg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wscmcynd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kxrzgogy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2byhnvois.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gljgybaj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnxrezzg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nqwzyqed.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2eouphvyx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2oqwujbex.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eqpwurfy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kujsofhx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2owujwrrw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uannazvt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2fzunhyyo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2xmlnjpyh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2dhbcabka.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ifcjofzx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mpeywkzw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bshowpsp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yotzhteu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qmvoijuw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2wavkqrgq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2fywsjong.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ceetydot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipesdpow.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2liyxrnxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hesdbhue.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2iujphhca.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jigwiyzm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vurfrulj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rkwidglv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2vvenboso.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tpydrudp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lhppbecb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nukqvnfs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zzbksves.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iscirzyi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hdlrnpib.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nbbxnshu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ucgmvbxo.html

);
来源：http://www.52xcode.cn/Article/details/gt2gatjnftu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rxkznpau.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2vicbwxwz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ptrejemw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nzjhgfki.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qmiuzmly.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2nynhyodb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hvpcjgpv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2goynidhc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mxfkjcxd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ijnzyxoj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2jcwapkpl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fffjabah.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uphacckn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2valtufun.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mzzlmfyw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yqnjsijh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2guaxgfay.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dfoceigv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2uaachwrg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qwcsptbs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gripfyvc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2egxnaxae.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aucacyda.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gmpakzkg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zqmniouc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ptzawjao.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wruviojf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nerpgjrh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wbcawong.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bkdzkhck.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tukmuync.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2scmeolqf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qakvfkne.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rtbhglli.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2pttzstfl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dscjdzkd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qtrkslfx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bxuqnrxy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hmlzqidq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2luywuduo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jpbcofzn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zixtdivg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qgvmywjs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ybmwsxln.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2amusztdf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2akmchckz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rswxojwf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wrwpymgw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sclymfcg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hnagtsqf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2adgepuyq.html


<!-- 参考信息 -->