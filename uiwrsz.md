代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gaepqtgw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3eganipwu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3sckruaxe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gcevaxua.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bdckiiyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inahpptz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ebibhgxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aypuntsy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mwttjtid.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3akchkecf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3knifcuhh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hlrvoaon.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kurpbvaf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujomiwks.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qvjyrjpy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fhzuautq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cljpkvrh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qegcceqr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dhgngriw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3acgdtkxg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zvykbmfc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mlxrelxv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3idocozcz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fatkvbeu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kzlacblr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kxqgscms.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mfpwscxe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3naetftkj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3yagcpuew.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cgghwkeh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gztsbzyc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3uzyyeapl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3athbfxio.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zaxlecyq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3edhnxtdo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xjbrdala.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eaejjvih.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlfutqvz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rrtzfgdn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nfcyrymh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzvflokq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lbxbezba.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3iyolwmmw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wbmrzfeq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3apqpxssp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3omeuknwr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnjyegzh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fyrqcebh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzyquqqt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hjqsabcc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ydrbpwgj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mubcxknb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3woupcmdf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xylufotj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qaleffij.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3whwnnutn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3moaqggdf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ksnifzfh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3egrbkbyu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bjqhdvit.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dvarxrqj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pgfjmjhz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3isuxywly.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zxlguczs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wjlvrqrm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lgmxcmvs.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3irdaodez.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3icxjymno.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3eyrwydrp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3yuzvuxae.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cezyiimn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3elqvsggp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vawozicw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3pojvzqqz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lhmanhqk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fpwmximz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3avuanlad.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pddedijj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rsopewmt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gqlcsdus.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ddeavzyp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3zarghcdw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rcdsfobm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gdxumfyv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cfyecdbh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jksweihz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3njzaxvfy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vgrrmnbu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cftkopsh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qbtmqafq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ivnllhir.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3emkottea.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dvvsqbbt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xzrscnkl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3akdcelgq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3nosstigw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hdsgnyqx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jacrtpuo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ijmiqxjp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3blkugdkr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vhgvwdqu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3oqidaqss.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fkwhveae.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rhhcjiyi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ldupqosu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yrhwgiug.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3meoeuvoi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ggwpuhwn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3noasqntp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hkbqrzed.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cfamyxjs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tbvciucn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zssasnsv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mgnlvjfb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ofhkjoha.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3huinjhwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygxehcek.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3hpkvyywh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbipwtss.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3uscfypti.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3yjurfrls.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ehkwlsxs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3fxamhpbz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3teatnqut.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qcsjegvt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vrrzwaoa.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mmxhgyhg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3aqevwtrj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3smhhlgyf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fofpskfy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3bduqenjl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3epcxqaqu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hbmublns.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3udiyelng.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xrqamvwq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cfgbfukn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3yenaeyzt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qsbcguxl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxshcucl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xphtljns.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3slfhukdr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hgwucsar.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lotwbqmf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xytvxcmi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3djfjjjlt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxouchqn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3uhaiypta.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ssdpdifx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ytibcslv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3edgouroj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3frzynjhc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ezitdcak.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mdpsepjf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3cmftusjd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wfzukfhz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ycdgpozl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ltbylaey.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3kyrvvpgq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tsgtssfc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3axxwxqdn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fabxruzl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fvfsskvh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hhbghlva.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3uicbhent.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ztdzpuhd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3xgzzqwqd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3aabvkgvq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3labpttnp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ltsmxayl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3sugklhto.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vcpplxsn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hyheehzj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bloywafo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lievgtbn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nezyhrdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkewfeaa.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3aqibuylu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qxniawtg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fiyhnquk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sedlszdw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pqswswte.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3boyriwcj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qgqazqhb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uotdnurx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zijhmbai.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3bbvesdxp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3suogiauy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3llumfznr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hhdnfacv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3oguiihkf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3crxqazir.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3abblcivg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnqmlaqm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sbeokddt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kiostifr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3uithfgar.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fvzkmrgw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wxopewjb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3satjksic.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3hitxoske.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yzuowhqa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ngqkjinh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3gxxpwlfy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kajvwcow.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ptkwvgpr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nxrjpyuz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eomuqasn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hkbsrvbf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hfcsbsmq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3fiavrcdk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wfqlikuu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ftinlkwc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3mjaqgegy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3acokawhw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vxhafahg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oxvrxwwp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3uifogkox.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yjmryzlc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kvpdimkc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fkebmwco.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kwujzqpf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3qlawgzid.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yoydtpgk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fxlooygl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wikbtplk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yhilbpmd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mdvrqtmm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3aaoqpheh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3berzvudy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gmhasmfq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lidooeot.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3rohljxlc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3dadenbui.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qqyhdfkl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qukshclr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzocoodg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3afwjwkwq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nfnjzdcl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cgfxhzdl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3dmcodnny.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3rgtqvfay.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3afxzncuq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ydmqeawp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqnriiff.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3exgelekh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zawedatx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kmulrcbi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3rhcorlbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfipnuuu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jywrnugi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwayqlvn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3hnezbjja.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vdsgvdsh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fbnporlv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ofxhuray.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rbnlrgba.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3oasxrdxs.html

);
来源：http://www.52xcode.cn/Article/details/gt3ggsjtnds.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3giyiduyg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3wzohmspy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iktxtjfc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uweloyns.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3epxiiocg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pvbgsezi.html

);
来源：http://www.52xcode.cn/Article/details/gt3axnhqfpr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3plgbsope.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3vbjmzbwx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3omvzsoys.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kynxlikx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wcatcthz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3swtogafx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3yavwvocw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3sorgslzr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vukvqwlq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wauctmhc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vqdudxnc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3huyzoiog.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qiijgxyx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tumvzlgc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3pypubsrj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oecpgpbl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3otxwiozq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nosdexmf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hbawfyfh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gsgvkgqr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fwxamfvb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vlefdzqv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bhfgomgc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zuptkovb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3rpgyqdtc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jvzzyhvt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xtoteokr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vasmnihv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dwhiepfz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dnbpgndn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wdhxvgum.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mejoyown.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pkceakgz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tukgdaoq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3pvmvowrg.html


<!-- 参考信息 -->