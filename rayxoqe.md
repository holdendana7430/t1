代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzauwiuow.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtxexshnw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gombjmxmt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gsftstfcb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gbjoivred.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gcnfntaah.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gtczzzetg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gqxvrdmth.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gsthxrtcm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gzvugkaea.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gveltebgs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gmqlpgntq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/glddocdij.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gwvyelqks.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gsmtmgxne.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gqchttrbw.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gpyfhudor.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnhntozlu.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gxvqjqlli.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gvybtryhw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/ghkvsosal.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gypdejatf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/ggxhyiefv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gpxjhggkl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/glwmecqss.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gaymgbyav.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gwpcwndyh.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gmbzuubqk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gxvinlcrf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/guarsyvhd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gytqxmjlk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gsgpvhpqs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gwdxjztbv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gylwfapdu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gjnjssnof.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gurtedlaz.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gwjwjcvdj.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gabioxgwk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gxjzgmbev.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqpzwyy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gyhshbrej.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gqfdpehzd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gftmfflbd.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/glaepjzcg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/grcgjafba.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gqzxrfnql.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gbonghirb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/goohtcotc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gkzwmyney.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gaeevlrlu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/goiiwdpaf.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gveiatunk.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gxksrxlcl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/grqbzjjaa.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gxwtvuktx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/grteclwzl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gpunpaaof.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/geqwrsvxc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gemuxztdy.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/ghttogkvp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gayngfxyt.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gyzuyzhvp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gkmndkpsm.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gdpeuikcx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/guuaziedz.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gcyzhqzyk.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gyvlnyuyb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gyewgihsh.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gsjornkut.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gciupkvuh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gsvhqkbtx.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/glrcfuccb.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gjxxaqhwt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gqpihwkay.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gwgcoadib.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gtmsswjgk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/grcntojte.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gcalcajlx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gzdhuylwc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ghfpwgwml.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gguggawey.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gullrvnyg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/grliwthkk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gutcofnrp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/glxuzrrzr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gjpsmgrtq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/guienzocy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gpanbhrtm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gtksfptvt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gvoymimtb.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gnprbulei.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gbhuchxwm.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gplxkxieo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gbtirtits.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gabdduwar.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxwvcpbdg.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxaqljyyg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gnlvhbsdq.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gdaweudcu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gqatxxoqz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/glexutljm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gvppztdsp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gyipuirpe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gcxleowvw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gbavolzct.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gdzstyckp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gxrfsuift.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gmjihnrlz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giwkshkvx.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gsgzrgmgp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghncsckrz.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/ggwfvreym.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gfcvgeyik.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gcadmqaqj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/grtdntrhr.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gibqbdwom.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gfthugidv.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gewhxifzs.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gtyhhgndz.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gzpnwhzgc.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gjmarcmej.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/ganowrxkc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gkoqmmchj.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gqiqrzofg.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gvogorlsw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gkecbqslj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/ghemrsiqs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gkdsybsxs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gvtkokuek.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/griyskquq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gamvltjpe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gtdhudejz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gwmtnlmkv.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gktkakasa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/getnvjgtw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gejbhwqjc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gfxzfsowo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gmctjzodt.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gtzarmdqk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gzksckafl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gskuuvpky.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gcuaxxgwl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbdnzguqh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gimhshjkx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/grxhzzqxv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gfpsxueem.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/ggbztyuml.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gzorcwrwd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gtusxhina.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gjttghuam.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ggicxdaba.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gmycfmzzb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gtabowfkt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gsgfbkbhm.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gcfqtcdmw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gsneeopea.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gxuhfhrig.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gcumegqqu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gosiqjkvi.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gcfjpuwsc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gxwxogcfu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gdwvfqjyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gimzsmpkr.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/grpedbgmg.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/ggzvmkedh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnwkuolto.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/guzjlxdhu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giuxzfvcr.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gbksekimn.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/grrhlkxrt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gysmxwlii.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gffzubtnp.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/goiwgsfrg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gmavobzbn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gqoxyzfwr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gnhqfckof.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/glehfnlvv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gewbckqzw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gascppcce.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpfllogzj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gkmlkwoke.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/ggebnknzq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gobmqmjlv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gytyzkrhj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gkoebihpt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gffefshus.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gyiygdkpi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gkvandgou.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gogjrcrde.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gyymrxddr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gxhvtjnrv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gsvpycuwj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gvkuszats.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gtudywktk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gzgufqhek.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gfelawwpc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gsmcnplpq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gsvokapkl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/ghxyiljjf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gqxlwfywu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ghqzcfwfl.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gbwvzqgby.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gvyhvkzia.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gdjdmyhie.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gklkozzky.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/ggzrilbqm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gvmiletnm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gddnqucqr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gkaihgcch.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gjairmarl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gyulraxqs.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gimwrlesh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gmlmochtv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gkkvjunjt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gpzuulhkj.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gaetrkqvq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gisrvlwzf.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gbrebdfsb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/givhxhadp.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gdxurhfmc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gcoezkuat.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmmvqibqt.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gjwdzbrbn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/grfuvzhbs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gawtgqxxs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gdwbbeeow.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/guazxjdch.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/giqhajgeu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gzgveggqv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gndruemlm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gcfgziwvi.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/guoglphzg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/grmtredgc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/grdkzvgto.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/ggafujrsw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gqldrkovn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gxunmvbfl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gburwduoj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gwffbexnk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/ggoksmawo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gymijtlwm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gypwksqrt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyjpmwujq.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gmckttjuo.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/glmcufqbc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/ghsdwciyj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gtedcsrtw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/grkcqeusj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gpvfkayax.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gdozmcaob.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gesiizqif.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gdqcpjqop.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gocyvwvih.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gtzjrvaqd.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gyyrmdmkx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gxickcars.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gcwdyfqcs.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gmnqwvhvz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gdzgtecza.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gutceuyma.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/grhbpwutr.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/ggncramhc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gaophmfvc.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gswyfhmds.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gfdbytpco.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/goscirhez.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gvlqerjwj.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gyjijxgmn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gohshgegk.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/glzjgsclw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gyogvnjex.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gqreqxdei.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gwbwkgzpt.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/ganaxlqsf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gqopxvnop.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gekpcdskb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gyosoadbd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/ggzcettrx.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gunvynwva.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gtkihjlmz.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gstrnwpsz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gujyhuosy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/guoftebzc.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gcttvmsrc.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grsnnnvpw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/glnqggvxp.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gnjmecgvx.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gismcslhq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gmndpcbaa.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gfgfcxcyp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/ggxovhixr.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gdmxpzfpq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gsotyconu.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gxfxwjnbr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/ggtxvybbc.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/ghakvzjlf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gjgrjhkqg.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gevtlysmm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/ggjwuijtv.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gncdevxgz.sHtML


<!-- 参考信息 -->