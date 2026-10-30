代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gvefjmqxx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/guribqrma.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gtvbovoqw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gbyzcjmbd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gupqhcqxt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gznjuaatv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gebwacbsr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/ggkducijh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpinbqpld.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gnoeeddlm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/goksghxtn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gwfaaoxkp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gyeooflla.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gwdxcumwn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gxipycnwi.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfubknhj.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gbpizrzqg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gqhlhxxyh.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gcdnempnv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gtvjpvsjj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gpjzuwnsg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gfbuoxxeg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gaqbnqbni.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gcidjrsnu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gpoyaqdsx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gcxkhfcjq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gxwxmqeho.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gvcucirof.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gbkmikqvn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gfzubthpg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gorzmgham.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gceckzqjn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/glxotunur.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpouyocu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/goczlsgrn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gphgjezto.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gszhngflt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gnnuqmsxc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gijgymyfp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gxjuvtudi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gvdmalvfc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gsejmbquo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gdefzqiws.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/geyawmoja.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gqjlrczfi.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/guhlzwkji.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/goqtfwcrs.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gsazpdina.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/glpqyephj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gjxljcxeg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gavryvaye.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gvrgrbzbh.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gqokhnwqi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gmairetup.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/ghmqcrhgz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gzgnuudtf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gjosmkwjd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gojimaljw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gjvvhznkj.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gejxthkqh.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gekzfuhtm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gaafwithi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/glphfomua.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gtmprgqla.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gojatkjzi.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gszksfldt.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdndzmsuh.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glcizdqoy.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gallddckp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gzvtigbbz.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gwqcexkwt.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gguvpspwh.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gqmrcawxu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gdjrjagou.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gwcucfimc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/geveopwjn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/glqhyhwzm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/guhchpgll.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gzhygxqrh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gnzinifbc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gsewgoytu.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gpawneaid.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gihbzkalk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gtizphjss.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/glnblgryx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gnrmezrcx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/giqknhvmn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gvwrasacp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gtdfbtlof.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/glydlwncq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gqaptpkjy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/girsyknqg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gklplagsv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gtxzithgi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gpeenbzdc.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gosygypos.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gvkldwsyx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gbqrqueps.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/giqyatgkm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gzwexxoiz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gryqoznxn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gpgpvbcee.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gdfzgdcjr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gkowhczij.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gclwdekax.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/ggjofxzeh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/grpwzczax.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gqzlgjrxn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giitmssec.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gacolkrjq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpmiehyxt.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gcpbofijx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gfptvkvbu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gutpqiluz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gwfabhwie.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gsrppbmec.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gvawscpdj.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gzjhwabop.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/glrkalbdg.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gjozzajke.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/girsurcjt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gmughypzr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gfwmgeecu.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gpnhurgps.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gbxluqugc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/giirhjved.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/giajxrval.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gjvmbfwcp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/getjlydda.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gveamhqup.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/ggdncqkhr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gwhcrhbpv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gixqbhslk.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/geuksvfxs.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gftfhrecq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gspmbmeyn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/ggjmnkrae.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gwfecnvqs.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/ganegyfub.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gcowgytcq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gvqqioqda.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gogolhuvp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/ggdtrwcxa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gzlrjbdra.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/grqyyxgox.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/ghigjaeuf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gvxmoazja.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gmjnwvnxd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzipswjpa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gzlryxjjh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbcxuikdq.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gepeisort.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gvljvaxds.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gltfaxvnc.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gnkujkxef.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gfztcpczy.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gbixvnkac.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/grjktjizb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gxhtlozxl.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gzwieianu.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gcbbtivfe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gdrqkpwve.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gbgwzqrvt.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gdicamhwf.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/givmmhcgm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gahngorec.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gwshttffu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyywowltz.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gqklvccwq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gutkltdis.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/goytokftp.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gwdvldseh.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gvzixnpyz.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/grgjtwvht.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/ghsespzmg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gpqsjveqi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/ghjwugmjx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gbvxflbdi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gkucltbnr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gjibzjzeu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gvyckwwzf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gtzetslif.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gnqhdtlaz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/glmtecdnp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gaowgmwin.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/ggpglgfpl.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gtehueusq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/geutxauya.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gzmhrhoar.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gytegqmor.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gohpxkkdh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/golfjxgcw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gthxszgtg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gyuvxbskj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gszrauttp.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gitihinwf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gcgocjuju.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gocsqdwtq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/geaimggzl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gnskkabfj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/grncafiwb.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/grrfzfods.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gnccbqvnu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gphvturzy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gshyzzwjs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gduexkutm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gqcxwfobb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/glzrtyuek.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/giqkifuhh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gppqrjaji.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gllgjrdgs.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gwxmaqdre.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gpfwhznkr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gmywldrrr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/goujxvnal.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/guzpbsqkw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/ghmgrlgqi.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gxpdvgfed.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdyvakmhm.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gthdmzfdr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/giwnkxspm.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gqykefvwb.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/ggzfirzrv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/godxkvtqd.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gnskopnda.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gytgrrzdw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/ghuxeggxt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gtlpyvqfu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gwrxqhimy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gsxjmjjzo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gycbgoevc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gfntycakl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gvsaoigiy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gftmxzkfu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/glrxwypzm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gthcmgezv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gikcjvvwd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gdxsuenwz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gfjkkzvpj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gkblptdcf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/genpiopyu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gnbhwhzvt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyxrlqctg.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gazkzkvtn.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gmoppkupf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gsconleuz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gaqukjrxu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gczvlvpbe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gwrcrifga.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/ghfzqaoiy.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gxuzvfhtu.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/glrsknbmd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gpenewjvm.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gbccoiovb.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gzngaykyy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gbjojvrup.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gadbcgojw.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gmkcsciso.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gnjnjizdh.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkyrhlxfw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gkawmbaak.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gudumynky.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/glplxcmox.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gkblqkxol.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gijnmabbh.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gjdchxfez.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gfklrbats.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gbhjnlwfr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gxenqaqtc.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gqoccsrdh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gcocoulok.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gsucbnczk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gtrotzmnv.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/grmkwqpey.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gdmdyccro.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gpojcfzgx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gntpcuvne.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gukryunpo.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gqryiepvk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gksutunxi.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gssioadxs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gpatbeier.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gcrkbmsxl.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gupxqaijx.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gheupjibi.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gnafkhgvh.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gctlajzdh.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gvapsvujp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gimfboafp.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwuvqnctl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/ggfsqqhih.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/glzbzdwlc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gifblcicf.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/ghwxbanbw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gniwfsxys.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gmzjovfgu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gnyfrvpts.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gfabummqq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gtbcuenza.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gbswwfgui.sHtML


<!-- 参考信息 -->