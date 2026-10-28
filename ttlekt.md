代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hz.jyoumei.cn/gtrwrvefie.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtsaqgytdq.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtqrzzzahw.html

TS:   require.main === module
来源：http://hz.yangfankeji.com/gtuvjjqwvt.html

Java: public static void main(String[] args)
来源：http://hz.gotoacloud.top/gtrsipktle.html

Go:   func main()
来源：http://hz.havefunace.top/gtybjxrvjo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xinyue.icu/gtiwxizsvl.html

C#:   static void Main(string[] args)
来源：http://hz.shuidangran.top/gtazafeljo.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtqluowlch.html

Py:   platform.system();  platform.python_version()
来源：http://hz.svipenyu.cn/gtpehgjpbe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258888.top/gtwlzjesvh.html

JS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtzqchlupk.html

TS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gtnkstrjwg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gttweearnq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhoulong.xyz/gtboepbdga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangshuangyany.cn/gtbbnxwhje.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xylfe.cn/gtrecccrev.html

================================================================================
来源：http://hz.jinqigfzy.top/gtntsznqep.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gteviwsvud.html

================================================================================
来源：http://hz.zdqjudy.top/gtrcwwhdef.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgfzy.top/gtdqqruido.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hammf.cn/gthvfmsqps.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yueranfly.top/gtiulffshi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtmcjxtmfz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtlaabojzp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gthwgbmglj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yueranfly.top/gtdswfrujx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtukcxbmkk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtwtsboleu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hfpthk.cn/gtpaehxnti.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtpoivdexn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtnoiuxoek.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtehniagdp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtspdbgihn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.meibo888.top/gtszzizoih.html

Go:   slices.Sort(arr)
来源：http://hz.bjfxy.top/gtkryinhgh.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gteqlaidbp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dianchejie.cn/gtyooxvpjm.html

[N03] 快速排序（分治示例）
来源：http://hz.guannengcc.top/gtcbhvnybd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sufxvd.cn/gtxohgqpuk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhiwuduotai.top/gtqjujjwee.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtnfrbktew.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtnqiytcwp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jianghu66.top/gtxlqxqxkw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gtropjafkf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.redwolf501.top/gtmcdsvnnj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtxizvddzj.html

[N04] 斐波那契数列
来源：http://hz.chenlongwang.top/gtlhwaosea.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtwckxxygl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangtech.top/gtomjyeibp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtlsesktkp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtpobftgfk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigfzy.top/gtzedjjpss.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhixingplan.top/gtwagqequz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtznhvealq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnxiangtu.top/gtlvztxaun.html

[N05] 最大公约数
来源：http://hz.yj20258.top/gtwasshgcf.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangtech.top/gtcgwxgkjs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sufxvd.cn/gtqxymcspj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtsyiimsio.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtgxqncwmz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.feifeiyinyue.top/gtiumhkklm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yonumen.top/gttzdomfil.html

Ruby: a.gcd(b)
来源：http://hz.iojbl.cn/gtaatceomh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhoulong.xyz/gtycyxbomt.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtxbrxiuhq.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtmlpagtvz.html

PHP:  $s === strrev($s);
来源：http://hz.hongshengwenyu.top/gtjnrpaccg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtizoxvnwq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtchzwopud.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jyoumei.cn/gtwmyteftn.html

Go:   // 双指针从两端比较
来源：http://hz.zycfv.cn/gtivhpvxrv.html

Ruby: s == s.reverse
来源：http://hz.ywan-chungtsiang.top/gtvmdbtmwe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtlgfxwapv.html

[N07] 两数之和（返回下标）
来源：http://hz.smart0.xyz/gtwghehbje.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zycfv.cn/gtxylujwbi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtslwxvnwi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gtrkwawzlt.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydjk.org.cn/gtwmstjnpj.html

Java: // 手写 HashMap
来源：http://hz.redwolf501.top/gtgfzjkhsm.html

Go:   // 手写 map[int]int
来源：http://hz.aizwys.cn/gtbtfqqytr.html

Ruby: // 手写 Hash
来源：http://hz.jinqigufen.top/gtqvjstfno.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cashguo.top/gtarlkinay.html

[N08] 生成全排列
来源：http://hz.yuanzhike.top/gtmzvrqidu.html

Py:   itertools.permutations(arr)
来源：http://hz.daria6918.cn/gtwxizarda.html

PHP:  // 手写递归交换
来源：http://hz.xinyue.icu/gthjjpassg.html

JS:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gthovdenwk.html

TS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtzsjmauur.html

Java: // 手写回溯递归
来源：http://hz.52xcode.cn/gtpbttdoyx.html

Go:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtplculzbp.html

Ruby: arr.permutation.to_a
来源：http://hz.shangyingyoupin.top/gtaxrqmidi.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gteqhunwgd.html

[N09] 栈与队列
来源：http://hz.jinghuilouyu.cn/gtmzkzslkp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daxiang520.top/gtddyoceom.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgfzy.top/gtyhrwdgvm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtewcmhlfx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.52xcode.cn/gtccpbcmyl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuanzx.com/gtrmhjaqhh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aizwys.cn/gtpsqwgobr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.0kj1m.cn/gtizfkaauv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydzc1.top/gtvqwnwtow.html

[N10] 链表节点定义
来源：http://hz.zhengqikj.top/gtnuuqzjjm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tian-w.cn/gtztcystdm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtvavrsgtj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhijiandao.cn/gtwtuxmrrz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hysaishi.cn/gtucmthgcc.html

Java: class Node { int v; Node next; }
来源：http://hz.yuxming.cn/gtufpqrnau.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xziqi.cn/gtnxtpszch.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gtkgvioyfd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuanzx.com/gtvttovcbh.html

[N11] 二叉树中序遍历
来源：http://hz.cashguo.top/gtxdxosuhk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.feifeiyinyue.top/gtywvwfpsy.html

PHP:  // 手写递归函数
来源：http://hz.shangyingyoupin.top/gtrdwxiqee.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtqxzpxdbs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtmrsxkyxi.html

Java: // 手写递归
来源：http://hz.jinqigfzy.top/gtmvgsaqay.html

Go:   // 手写递归
来源：http://hz.andypj.xyz/gtigihftwv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zdqjudy.top/gtppjjfrok.html

C#:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtmhctuaov.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cheryme.top/gtqjsvtgih.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigufen.top/gtbmkqlnvd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ppjwa.cn/gtaeytsqmz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtpqhbkajf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gtmglmtapg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtjwrppipl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuanzx.com/gtqifenxvo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangshuangyany.cn/gtreowxidn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtxvlednhu.html

================================================================================
来源：http://hz.kuanghao11.cn/gtbcujjyvs.html

O. 并发与异步
来源：http://hz.daxiang520.top/gtjileenrt.html

================================================================================
来源：http://hz.gogol.net.cn/gtgikptmvr.html

[O01] 启动一个线程
来源：http://hz.xziqi.cn/gtopudndao.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.iojbl.cn/gtqmoqoxua.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pengpengdd.cyou/gtarofdeer.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hammf.cn/gtiaqonqbv.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtwqoohdsx.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhiwuduotai.top/gtfxucttzo.html

Go:   go f()
来源：http://hz.yuanzhike.top/gtcermbbhk.html

Ruby: Thread.new { f }
来源：http://hz.sweek.top/gtrxndhptl.html

C#:   Task.Run(() => F());
来源：http://hz.ehwqpu.com/gtsjklulng.html

[O02] 使用线程池
来源：http://hz.shanyushiyangtech.top/gtusylysjl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuanzhike.top/gtrbdmfhja.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cheryme.top/gtriuhodmq.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtxnfleqer.html

TS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtpjafrxym.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yvedp.cn/gtkplzaaaq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xziqi.cn/gtakiwtrcv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gtjazryacm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuxming.cn/gttddrwvsj.html

[O03] 加锁保护共享数据
来源：http://hz.zhixingplan.top/gtdsuxeien.html

Py:   with lock: shared += 1
来源：http://hz.feifeiyinyue.top/gtslxflmnp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinyuanbaomall.cn/gtdcqnnyui.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guannengcc.top/gtmbftujdq.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtggfuvfsq.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtrccexorj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hfpthk.cn/gtvfpjwqpp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.birdmap.top/gtztimctps.html

C#:   lock (gate) { shared++; }
来源：http://hz.daxiang520.top/gtzrogrpxk.html

[O04] 定义异步函数并等待
来源：http://hz.jlsjyb.cn/gtbgtwcahy.html

Py:   async def f():⏎    await g()
来源：http://hz.smart0.xyz/gttgmzpcdg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gtakzwosqe.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gtfsvftbqi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cheryme.top/gtlviywtei.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.wangdashe.top/gtmowfxrbv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cheryme.top/gtduzwucvh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxinkj.top/gtvublzbog.html

C#:   async Task F() { await G(); }
来源：http://hz.yj20258.top/gtbhvrwajf.html

[O05] 并发执行并等待全部完成
来源：http://hz.andypj.xyz/gtlnjmvoiy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhixingplan.top/gtoqbqcezd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cheryme.top/gtbahtvchf.html

JS:   await Promise.all(tasks)
来源：http://hz.aibaodan.cn/gtjqsokafv.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtqlzqnqoe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sufxvd.cn/gttbqbuany.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuetiantiany.cn/gtjknbdtac.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtvfttkbab.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guowangkeji.top/gtxaevooks.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtugwluinr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.bjfxy.top/gtbgddudjv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guowangkeji.top/gtvqhxeqwx.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtwszaipso.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtriqohkof.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.mhx1999.top/gtbnvutozy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ybcxt.top/gtykppbrhr.html

Ruby: // fork 块
来源：http://hz.snrcjt.cn/gtctvmiwwm.html

C#:   Parallel.For
来源：http://hz.andypj.xyz/gtqjwghwyv.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpmthtwhi.html

P. 常用工具函数
来源：http://hz.zhiwuduotai.top/gtmuedmfsm.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtelpolunr.html

[P01] 生成 UUID
来源：http://hz.316326.xyz/gtrhzxcmcr.html

Py:   str(uuid.uuid4())
来源：http://hz.yuanzhike.top/gtppbbwwqo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.wangdashe.top/gtwuqxqwjc.html

JS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gtcxejmvxo.html

TS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gtyhhttjgt.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigfzy.top/gtjdoyqhtv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gaohongyu789.top/gtuopoglkb.html

Ruby: SecureRandom.uuid
来源：http://hz.sxryk.cn/gtthuhggeh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.bjfxy.top/gtiamzacqu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gttpurzvdu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ybcxt.top/gtmccwxnkk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnqzz.top/gtdghynyru.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnxiangtu.top/gtachjwkly.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cucudq.cn/gtidpkcxxj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gtyhkyxqvc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.9152youxi.cn/gtuzukcihw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.snrcjt.cn/gtkjbfusyu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhongyouzk.top/gtifrxdzbe.html

[P03] 生成短随机字符串
来源：http://hz.fengsongda.top/gtyjendmfk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hongshengwenyu.top/gtvzvtimpq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gaohongyu789.top/gtwknevshd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtxyfzimfb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gttendqaln.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuanzhike.top/gtxcjinvcy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtbuburism.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xziqi.cn/gtvuhrpikc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jiagoushi.top/gteyjdpjjh.html

[P04] 求长度
来源：http://hz.0kj1m.cn/gtqgmevago.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gtbruvooxm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gttaqchdgm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtdqimwwee.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangkeji.top/gtebznmrzj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gtbglgufvr.html

Go:   len(arr);  len(m)
来源：http://hz.xuanzx.com/gtyqisrzfg.html

Ruby: x.length;  x.size
来源：http://hz.vqdsnc.cn/gtqpnoocbt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.fzhhl.top/gtmotojuem.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hnqzz.top/gtynfbgesc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuanzhike.top/gtuvhsaqcq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hongshengwenyu.top/gtjiuwbhvy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yueranfly.top/gtjajieulg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtfpfsdnqw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zdqjudy.top/gtrtvdyaek.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.feifeiyinyue.top/gtvhgdstul.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gtzfkxudvj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenjidiqi.icu/gtulitpysz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgfzy.top/gtfavwmsky.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xingfuxueyuan.xyz/gtzsepptwf.html

PHP:  if (empty($x)) {}
来源：http://hz.shuidangran.top/gtkontyzlc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yangfankeji.com/gtkltmsmjq.html

TS:   if (x == null) {}
来源：http://hz.hnqzz.top/gtcbchkfau.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtvqiiqwll.html

Go:   if x == nil {}
来源：http://hz.nanxinkj.top/gtjpoftsvn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xingfuxueyuan.xyz/gtstbpuifi.html

C#:   if (x is null) {}
来源：http://hz.pengpengdd.cyou/gtfgoeepwk.html

[P07] 防抖与节流
来源：http://hz.chenjidiqi.icu/gtqyewrovn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258.top/gtbqveraij.html

PHP:  // 手写时间戳比较
来源：http://hz.snrcjt.cn/gtyalhfqfq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtswadsskw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtiixhylnf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yvedp.cn/gtouxgjwjk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.meibo888.top/gtzofrsfbo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuanzhike.top/gtkdcyrtpa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtvquchjjn.html

[P08] 处理浮点精度问题
来源：http://hz.zhixingplan.top/gtvqcdnbhq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangshuangyany.cn/gthdrcovmb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtrhurmzmz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shangyingyoupin.top/gtnycjzwch.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.bjfxy.top/gtgharxkzk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenzaomai.com/gtnceuqlia.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sysykeji.top/gtxljkziot.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gotoacloud.top/gtomxtcurr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtupnvbruh.html

================================================================================
来源：http://hz.svipenyu.cn/gtdboofkrk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pengpengdd.cyou/gtzasnnlit.html

================================================================================
来源：http://hz.xziqi.cn/gtnwejyqhb.html

[Q01] 创建表
来源：http://hz.sweek.top/gtgiatzshm.html

CREATE TABLE users (
来源：http://hz.zhixingplan.top/gtwqvrrepx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtskxullcr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.316326.xyz/gtgyigpybx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.snrcjt.cn/gtzakrdbxb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yangfankeji.com/gtrdgqhkai.html

);
来源：http://hz.kuanghao11.cn/gthkkafvya.html

[Q02] 创建带外键的表
来源：http://hz.daria6918.cn/gtzrhjuqpc.html

CREATE TABLE orders (
来源：http://hz.cqqwz.cn/gthymyojji.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtimflpoml.html

user_id INT NOT NULL,
来源：http://hz.tanke756.top/gttrydindw.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258888.top/gtnjjyimob.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangshuangyany.cn/gtisthugsv.html

);
来源：http://hz.wangdashe.top/gtaxvrvstl.html

[Q03] 增加列
来源：http://hz.316326.xyz/gtfsuttxxn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangshuangyany.cn/gtycxryuvd.html

[Q04] 修改列类型
来源：http://hz.sufxvd.cn/gtivlmfnxp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cucudq.cn/gtncrqyurq.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtoacvbfjp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtgtxtsfil.html

[Q06] 删除列
来源：http://hz.xuetiantiany.cn/gtgjfnubod.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hysaishi.cn/gtssnmxyem.html

[Q07] 删除表
来源：http://hz.xylfe.cn/gtqmzoggkk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigufen.top/gtpanxdrsl.html

[Q08] 创建普通索引
来源：http://hz.yueranfly.top/gtbyolcdzt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guowangkeji.top/gtpwnobywc.html

[Q09] 创建唯一索引
来源：http://hz.gogol.net.cn/gtbubwmdhb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.smart0.xyz/gtvlssjbkc.html

[Q10] 插入单行
来源：http://hz.yj20258888.top/gtxkjxndpz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zycfv.cn/gtuuadqhpx.html

[Q11] 一次插入多行
来源：http://hz.ybcxt.top/gtxbjsmnxl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.mhx1999.top/gtkvllisqf.html

[Q12] 插入后取自增 ID
来源：http://hz.andypj.xyz/gtbdhmgdpe.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.316326.xyz/gtpwatreav.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gthowowlgy.html

[Q13] 忽略重复插入
来源：http://hz.zhengqikj.top/gtbcgyxqcg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.9152youxi.cn/gtxuirgfgx.html


<!-- 参考信息 -->