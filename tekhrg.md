代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjhfywxp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fihazqfs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ubsmevid.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2icapkkhd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nixvhsck.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qvwydlnm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lexxysor.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gdlbzuaq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ohzoamcn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2pmbhnxap.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2clexogms.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vuiyyylf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wuorqzhm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hasurhgx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ytjznxjp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2exlaeqna.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tivpzobf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ewwbzbfv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bxmtxjyu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mpkvxstg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jxhrdvwe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2swbgqxzx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ndztvvtd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xmmdnpzz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ictmcgdx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kjqquggo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fpuwikko.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xmizxebh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ndriooje.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2okiwtmgl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvfuvymn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhginscu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgqpnvoq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jlxcbiba.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ouuywaiv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gikzfvcx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbyfnzmo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2verxfenk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iqybvdyg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gsfovzyz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qknmlwli.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qgssvalo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2dmxprygz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2htewsfiv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2puldbxva.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2epyikhef.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2pvecpfvv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yanrgvjh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2bzpywzye.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cxraclmm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jizomgtp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pktpqflp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dhysjreh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2kmyzthrq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hlbjaehp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tuzumbzl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ovbzmebz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kxfyzbin.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qkzqfzrj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xbfqwcxk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2npxontug.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cakydhlx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gsshykic.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ckyfmhbu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2phxrrqlt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wrfxtpot.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fepadbne.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gmgtkmdl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2niisyhha.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2evgmmqgw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cxrpakbk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2teppgzqm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jrqtrxuu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xzgirmov.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dkenwhvm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lfipkhqk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ijkpzqqn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qadvnhks.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2doquyxli.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ocftqqdq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2amugbtcu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sitixsmm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iyoyhcsu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2bguctsya.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kpwpkvxx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cylkhmxi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xsdsfzpx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gymhfdxe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2puhjghwf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ifnawppc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vwkowids.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ruxlvmuk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xoppqadg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2motjceet.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cvmzwzcw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mnrembcv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lkpnvaom.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gkyeobja.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pguzetzg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vvolxswj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfedbxop.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2eiydrqkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htimofkh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2bogyoxbb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2aggldflu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ayvppkol.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ruptnsgs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2avucqfci.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wtbveyri.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cspzkzog.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2byzvklea.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2kvuiimby.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2inycrula.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rznnrmly.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2blotojgr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zuocqxmd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2twixales.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2mzuzqcfp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2eqegqxke.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tmhfcecz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jrcjgyjk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vozktkyz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cgkrjgjn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gemtnjiz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2wsvtyzqj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wuhkihin.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lwgkfzes.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bkckqpha.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2hcejnxtv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubtvikov.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qfgwozev.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2aarerbqq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bgvmjksl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2adyipsol.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2betmklrb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2phgrstmu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bqoewrbw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ieidpuag.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jpeqtkvl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dictecxi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kwhaiwxc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wcyjsbge.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dnaxwmiy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kbcccwtk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2nrgjcwbt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vsbixbym.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2auullqzb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ogblzmop.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2cnqqpuqa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uuxeouoq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ivtnlfll.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2debvbjdd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ymilzwfa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2siuqzlno.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fyxfvltb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mufmelik.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yvktuywg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlbndmpz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ldpjhzjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikwgumze.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2anvmqcgp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pscbqncv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2lzfeuhvk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2suwoppve.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2frqrddgi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lfsxabnz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tctjwyhc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xnylpwnk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ucjqqssl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2iurtgycs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ytzihvtm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zilywmja.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jqmtrckp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qvedrcem.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2igqlsamj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2mgtokhpp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgstahkh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2juaxcbin.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tgffvrfz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2exhnmjww.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2egfabano.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qpeyfvyn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2moluykng.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2fedyolmj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ozwooiyy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qllsyuoj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mglwwtor.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pvtbcscz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2raaszpbo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2krhpdbkc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yenxijyx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2chjabccv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2iuuangvm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wagiqmni.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qnkcxkre.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qynvhyqt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2dovpjebx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2qppvcmtl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rourikqm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2pkaffanw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vzmuwwrm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mcikispc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bkvaqify.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zygpdxpc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jluhhdxr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ckymskoz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gbrwcflw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rilfgsar.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2afuemeca.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxihppro.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiscvudp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ennjcqnq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2htmkhhjk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljnafzfo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ixqlnlfh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gvxfsbqw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lptifcjc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ddzrruaj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jpqmjiaq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjpuxhzv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uesecuit.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xxnppdfz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qyhlqcuw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qddklqlo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vrsnfzji.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nobozkmo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wxfjryzc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2caeyprji.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gthvtndj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2crfvipex.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2yoopdehg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jrunbkna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uicvkmaq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2qwjrgqlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vntkuobw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2udsqdkgu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pbmpsumy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wrqkzkfg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dwwkxmrk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kthkrjvy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gypuzeur.html

);
来源：http://www.52xcode.cn/Article/details/gt2ngpvmvop.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2csjiznkn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nryqewyt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2goiqruut.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lgzskcpq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2exqyfeta.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zzvhavjd.html

);
来源：http://www.52xcode.cn/Article/details/gt2aehgtjka.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xhiysrwa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jiolnbwf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2psqlomro.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bdzguuxn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2khynzdos.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ovieyzhu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wmntcxwv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jqrnpdqq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2cknoxvwi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yrzlbabh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ikxeinje.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hltcnnyh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2esuahfgk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2owvogpnx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xllzdwqv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2imagcywv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kbxsjvdg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xuqoezfm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fsvtemsd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2cahtkbpw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hmdyftit.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2pklpauza.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2crhsnotb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2srkwvnfq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lzzgpaea.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ncebaalc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qshyuqvr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dqpklraa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ajkymgin.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bsiianep.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2eyqqadhh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2iqgzrlwt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jjndkumt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2usbpleqd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tiesmrmj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2lomdgxyv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qmwzqjeb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cyxiavct.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vzzdbewb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dplirsjo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yogycfvw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dyrhjpax.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vfnbogiy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ljtvsjtj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lhfaeeke.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vgosulib.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2iklekyin.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2bwvyjteq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nwlxquae.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eabmepdk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2leapolsc.html


<!-- 参考信息 -->