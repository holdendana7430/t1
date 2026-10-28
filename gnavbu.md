代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.daria6918.cn/gtrtyinnvv.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtqhokkqys.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ehwqpu.com/gtsstfausq.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gtchsngxnu.html

Py:   if __name__ == "__main__":
来源：http://hz.yangfankeji.com/gtfuqmzzge.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yanxiufei.cn/gtksdukqfy.html

JS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtspadmlni.html

TS:   require.main === module
来源：http://hz.snrcjt.cn/gtjfwojgot.html

Java: public static void main(String[] args)
来源：http://hz.0kj1m.cn/gtovwcjxge.html

Go:   func main()
来源：http://hz.redwolf501.top/gtvaltpdqo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhongyouzk.top/gtxrfqpagf.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtqjvhcrih.html

[M08] 获取系统与运行时信息
来源：http://hz.wangdashe.top/gtsmzqbkiw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shangyingyoupin.top/gtvhdyhxbx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gtxqknqjam.html

JS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtvxyyigjv.html

TS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtyqwiutfi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pycfn.com/gtbigxddpc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xinyue.icu/gtakryswya.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigufen.top/gtoeljajsc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtiziyhtth.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwseertpv.html

N. 数据结构与算法
来源：http://hz.aibaodan.cn/gtxkgyfjko.html

================================================================================
来源：http://hz.hysaishi.cn/gtpflwdfit.html

[N01] 二分查找（有序数组）
来源：http://hz.zhaomingkeji.xyz/gtgvruvxcb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guannengcc.top/gtrtcykncy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhengqikj.top/gtgsxwcdyw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtnfvpyrim.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtrjjlptft.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gttvaoafyg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.0kj1m.cn/gtlvzcwcha.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtmblyqspr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtfytutnuw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangkeji.top/gtlbajfjyj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtodmalnqv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxuanxn.top/gtbkxuwbol.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtosccqohv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtossneirw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtntmtlvrz.html

Go:   slices.Sort(arr)
来源：http://hz.sweek.top/gtxwnnifus.html

Ruby: arr.sort
来源：http://hz.nwbrower.top/gtfbtmjsam.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtbeopzxtp.html

[N03] 快速排序（分治示例）
来源：http://hz.jlsjyb.cn/gtzdofyspc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yangfankeji.com/gtofufyxru.html

PHP:  // 递归实现，或用 usort
来源：http://hz.quarkkingdee.top/gtezdxfzsz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtcysgqgvs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtmzaebsra.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pycfn.com/gtunwxqzbe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yueranfly.top/gtotdvmeaz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.kuanghao11.cn/gtszjxzeqp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenlongwang.top/gtcqydaksw.html

[N04] 斐波那契数列
来源：http://hz.yj20258.top/gtbivimudc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtgqxoqwum.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gtndznnyxx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtwecdfupk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtbzhoighr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.mhx1999.top/gtllzdzsfl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cheryme.top/gtzoidhunm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtdpsjlxvf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtoxkbbwyf.html

[N05] 最大公约数
来源：http://hz.ydjk.org.cn/gtpvyhwisx.html

Py:   math.gcd(a, b)
来源：http://hz.52xcode.cn/gtpznjredt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.guowangkeji.top/gtqumdlxvb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gtxlbrwlox.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtpcaijfss.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtlapdvdvh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hongshengwenyu.top/gtxocjvyqj.html

Ruby: a.gcd(b)
来源：http://hz.kuanghao11.cn/gtilmlvxcy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhiwuduotai.top/gtkmvrombc.html

[N06] 判断回文字符串
来源：http://hz.nanxuanxn.top/gtzzfsicjn.html

Py:   s == s[::-1]
来源：http://hz.hysaishi.cn/gtitffdmcb.html

PHP:  $s === strrev($s);
来源：http://hz.c1oappe.top/gtgrblvbja.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtugzjstod.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gthhevnjpi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sysykeji.top/gtkmwopgma.html

Go:   // 双指针从两端比较
来源：http://hz.yangfankeji.com/gtmrulitqc.html

Ruby: s == s.reverse
来源：http://hz.jinqigfzy.top/gtfzgtkqtm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtoqdohgho.html

[N07] 两数之和（返回下标）
来源：http://hz.zhiwuduotai.top/gtumwgqvam.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangtech.top/gtbwvlhkqe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhiwuduotai.top/gtqzgumamo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.iojbl.cn/gtpfhyrpkd.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuxming.cn/gttsenhvct.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangkeji.top/gtrowohixn.html

Go:   // 手写 map[int]int
来源：http://hz.xziqi.cn/gtytskojhd.html

Ruby: // 手写 Hash
来源：http://hz.jinyuanbaomall.cn/gtqdmvrkmx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guannengcc.top/gtefztfong.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gthyppamjg.html

Py:   itertools.permutations(arr)
来源：http://hz.gaohongyu789.top/gtejbzxvbr.html

PHP:  // 手写递归交换
来源：http://hz.dashuyun.cn/gtvdkbmiar.html

JS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtarderljd.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtfnebnlxz.html

Java: // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtwtijjccx.html

Go:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtiydtfixy.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigufen.top/gtuzphzjlx.html

C#:   // 手写回溯递归
来源：http://hz.yongpay.top/gtmfyyzjgw.html

[N09] 栈与队列
来源：http://hz.zhaomingkeji.xyz/gtbozkifcl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xziqi.cn/gtxfupvnas.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.mhx1999.top/gtzowxnqlq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.c1oappe.top/gtkyekstdc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigfzy.top/gtzplndopx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinghuilouyu.cn/gtmeaczjjg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jiagoushi.top/gtjlsiwukw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.iojbl.cn/gtuhmzagfk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hnqzz.top/gtgvwwhjkz.html

[N10] 链表节点定义
来源：http://hz.ybcxt.top/gtzcaofdwr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shangyingyoupin.top/gtzugxgluo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cashguo.top/gtxzipcymd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ehwqpu.com/gtohykxxvp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.snrcjt.cn/gtwhqyjpia.html

Java: class Node { int v; Node next; }
来源：http://hz.jlsjyb.cn/gtzpbewbbk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangtech.top/gtdkzggfhl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zycfv.cn/gtqnkgjctz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.kuanghao11.cn/gtixvkzvkm.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtgejlxbzp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gtnehwlyzt.html

PHP:  // 手写递归函数
来源：http://hz.hammf.cn/gthflyseha.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtuxfxwrip.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtaodfpula.html

Java: // 手写递归
来源：http://hz.zhengqikj.top/gtuwwhzmuw.html

Go:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtdbgujosm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gtibjrsgdw.html

C#:   // 手写递归
来源：http://hz.sweek.top/gtpfdsxvxp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinghuilouyu.cn/gtbiqughqz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhaomingkeji.xyz/gtsumvsyjh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtplfpopbj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtevcjrmfe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gthshdigzj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.feifeiyinyue.top/gtvcjyyxac.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtjoxxaude.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.kuanghao11.cn/gtpdhrqhuw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtuzgxwcas.html

================================================================================
来源：http://hz.dashuyun.cn/gtvohdqkwy.html

O. 并发与异步
来源：http://hz.zhixingplan.top/gtgrbtiaip.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtucbnwuqz.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtihanefxw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nwbrower.top/gtlrlcwtdi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gthjtcwzrg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tianlin.xyz/gtqomabaqe.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtdrjchhwr.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gtzipkvrwk.html

Go:   go f()
来源：http://hz.bjfxy.top/gtbixlcgbk.html

Ruby: Thread.new { f }
来源：http://hz.chenjidiqi.icu/gtysaklpjv.html

C#:   Task.Run(() => F());
来源：http://hz.wangshuangyany.cn/gtglsfuifr.html

[O02] 使用线程池
来源：http://hz.ppjwa.cn/gtwufrarao.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gzhubu.top/gtedbgcwvm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yongpay.top/gtofotxpvt.html

JS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtriftnkqe.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gteflhqaai.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydzc1.top/gtnykknhld.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtozyyzzpf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pycfn.com/gtddlubmic.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnxiangtu.top/gttjyjgswu.html

[O03] 加锁保护共享数据
来源：http://hz.hfpthk.cn/gtnpppqwzm.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtwkaazrjz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ywan-chungtsiang.top/gtseuescyh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gtfiejpexd.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtvmhgrtrj.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenzaomai.com/gtcwdkwlvo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pycfn.com/gtpfphsmdo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtumpzxeem.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtyrurcasc.html

[O04] 定义异步函数并等待
来源：http://hz.shangyingyoupin.top/gtxlzhbrwd.html

Py:   async def f():⏎    await g()
来源：http://hz.svipenyu.cn/gtxktsmrdj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhijiandao.cn/gtircqafxx.html

JS:   async function f() { await g(); }
来源：http://hz.ehwqpu.com/gtjsqqfrge.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.kuanghao11.cn/gtfjlqtdjz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtnvcqfevs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hysaishi.cn/gtwcryypof.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.andypj.xyz/gtyyyjydwo.html

C#:   async Task F() { await G(); }
来源：http://hz.hammf.cn/gtgmyhxuje.html

[O05] 并发执行并等待全部完成
来源：http://hz.dianchejie.cn/gtblscdzer.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tanke756.top/gtbnatczmj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jianghu66.top/gttnokezui.html

JS:   await Promise.all(tasks)
来源：http://hz.ydjk.org.cn/gtmcukwrib.html

TS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtchhywjdu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ehwqpu.com/gtzxtsanqh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yongpay.top/gtyfemvvli.html

Ruby: threads.map(&:join)
来源：http://hz.9152youxi.cn/gtwerossgj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.svipenyu.cn/gtelbsbgmr.html

[O06] 使用进程池
来源：http://hz.hongshengwenyu.top/gtvlsnzghn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.birdmap.top/gtutyjgceb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.0kj1m.cn/gtwzcbrfmo.html

JS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtjzaguvvw.html

TS:   // child_process / cluster 模块
来源：http://hz.jinqigfzy.top/gtfavifwuh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daxiang520.top/gtgzgmyvgh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cdnleiting.top/gtfsundpeb.html

Ruby: // fork 块
来源：http://hz.ywan-chungtsiang.top/gtrntsslha.html

C#:   Parallel.For
来源：http://hz.hnqzz.top/gtrsrzxnxx.html

================================================================================
来源：http://hz.cashguo.top/gtebafywve.html

P. 常用工具函数
来源：http://hz.quarkkingdee.top/gtvqrcooaj.html

================================================================================
来源：http://hz.nwbrower.top/gtqmuukyek.html

[P01] 生成 UUID
来源：http://hz.shzxlz.cn/gtxegbfrmx.html

Py:   str(uuid.uuid4())
来源：http://hz.dianchejie.cn/gtxljhivob.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangkeji.top/gtvgfisfsz.html

JS:   crypto.randomUUID()
来源：http://hz.yongpay.top/gtskfxzyag.html

TS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gttjmzmkgz.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangdashe.top/gtulzhoiqg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yonumen.top/gtrfrqsvfl.html

Ruby: SecureRandom.uuid
来源：http://hz.smart0.xyz/gtloindtiz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.havefunace.top/gtwaypowmc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guowangkeji.top/gtrrzqfman.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydjk.org.cn/gtdqcbrots.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhixingplan.top/gtvpoisgdv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangtech.top/gtkfneiowb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fzhhl.top/gtrxydtxgv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenzaomai.com/gtinanmkge.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xylfe.cn/gtiapegoon.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxuanxn.top/gtdrddggzi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yangfankeji.com/gtezbrphqg.html

[P03] 生成短随机字符串
来源：http://hz.hfpthk.cn/gtlscmutsm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zycfv.cn/gtqsdcjzds.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cashguo.top/gtqyeluzim.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gteopzpinr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtxymnokki.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cucudq.cn/gtccvfzzjp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gogol.net.cn/gtqozkhrrp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.kuanghao11.cn/gtfmlwnqbm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangkeji.top/gtfibmgrch.html

[P04] 求长度
来源：http://hz.yongpay.top/gtpyozldmp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hongshengwenyu.top/gtveladjmv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtcofokqnp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gtxrrivzog.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtitahwevs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jlsjyb.cn/gttmsvvuld.html

Go:   len(arr);  len(m)
来源：http://hz.zhaomingkeji.xyz/gtyfirtlhm.html

Ruby: x.length;  x.size
来源：http://hz.feifeiyinyue.top/gtagmasxra.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xylfe.cn/gtxdywghtb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gtlisqrcfx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgufenzy.top/gtmsbbkmkw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.kuanghao11.cn/gtujkamygd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.c1oappe.top/gtjxertudn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hysaishi.cn/gtnisfhpfk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhixingplan.top/gtszrjvfec.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tanke756.top/gtgcrjwbzq.html

Ruby: a == b
来源：http://hz.ybcxt.top/gtjxaodhve.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ppjwa.cn/gtqpmlxrji.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigfzy.top/gtznyzpntx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnxiangtu.top/gtvopvuaey.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtlfwitusd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tian-w.cn/gtpofkjfdm.html

TS:   if (x == null) {}
来源：http://hz.mhx1999.top/gtmoinsgpc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtxqfkfsdm.html

Go:   if x == nil {}
来源：http://hz.jlsjyb.cn/gtrnefnhyf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258.top/gthhxhozms.html

C#:   if (x is null) {}
来源：http://hz.zhixingplan.top/gtxyukhwrx.html

[P07] 防抖与节流
来源：http://hz.gaohongyu789.top/gtdltyuidv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dianchejie.cn/gtogzfdive.html

PHP:  // 手写时间戳比较
来源：http://hz.c1oappe.top/gtdcpxrbkz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtospxyqfv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtqmvtvbxc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.feifeiyinyue.top/gtlhbjzwsa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.feifeiyinyue.top/gtfpgftnyx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nanxinkj.top/gtfkjavtct.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ywan-chungtsiang.top/gteorgegib.html

[P08] 处理浮点精度问题
来源：http://hz.chenzaomai.com/gtaykkrzvi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gtixbnfbsj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cqqwz.cn/gtijbloajr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gtkckbimjo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhengqikj.top/gthmdmzmbd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.fengsongda.top/gthgygwqjy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gtebysiied.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangkeji.top/gtlzkajklf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.feifeiyinyue.top/gtsjanohqb.html

================================================================================
来源：http://hz.cashguo.top/gtceqwtjsz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jqgfzy.top/gthxvygjry.html

================================================================================
来源：http://hz.c1oappe.top/gtpbbfkrcs.html

[Q01] 创建表
来源：http://hz.yj20258.top/gtopzxdqqz.html

CREATE TABLE users (
来源：http://hz.tianlin.xyz/gtkajdnikr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtlcipfape.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aizwys.cn/gtcnxibkls.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ehwqpu.com/gtqzymispp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangshuangyany.cn/gtzwivcaxm.html

);
来源：http://hz.ydzc1.top/gtjiltkptu.html

[Q02] 创建带外键的表
来源：http://hz.bjfxy.top/gtjxbstudh.html

CREATE TABLE orders (
来源：http://hz.xuanzx.com/gtztoduaxb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtdonfxjkx.html

user_id INT NOT NULL,
来源：http://hz.smart0.xyz/gtdnxwjkxg.html

amount DECIMAL(10, 2),
来源：http://hz.yvedp.cn/gtnaalybpn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tanke756.top/gtrhbkbeai.html

);
来源：http://hz.daxiang520.top/gtifdtnfsc.html

[Q03] 增加列
来源：http://hz.316326.xyz/gtssmpqzcf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shzxlz.cn/gtmyyoeabn.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtdxusletb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.smart0.xyz/gtvkiqncch.html

[Q05] 重命名列
来源：http://hz.yvedp.cn/gtkihcmxfm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhongyouzk.top/gtxtejcygd.html

[Q06] 删除列
来源：http://hz.shzxlz.cn/gtmlehezll.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fengsongda.top/gtrzvniycf.html

[Q07] 删除表
来源：http://hz.yangfankeji.com/gtsyabtjkx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ivvv.top/gtlyuaosdj.html

[Q08] 创建普通索引
来源：http://hz.meibo888.top/gtqpgwffaa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhaomingkeji.xyz/gtmzuirtqr.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtlsdpoetn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtaljhaajx.html

[Q10] 插入单行
来源：http://hz.dianchejie.cn/gtvypwvokj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgufenzy.top/gtankszqug.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gtkhmspsfr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.andypj.xyz/gtrkxrczeq.html

[Q12] 插入后取自增 ID
来源：http://hz.cheryme.top/gtvzrpwugq.html


<!-- 参考信息 -->