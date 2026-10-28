代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gogol.net.cn/gtedmjbbnz.html

[M05] 设置退出码
来源：http://hz.chenlongwang.top/gtcotxenho.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtbekeqxch.html

PHP:  exit(1);
来源：http://hz.smart0.xyz/gtikrrdgee.html

JS:   process.exit(1)
来源：http://hz.guannengcc.top/gtjnkuetrc.html

TS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtzlehfzok.html

Java: System.exit(1)
来源：http://hz.ehwqpu.com/gtxkmcibaw.html

Go:   os.Exit(1)
来源：http://hz.yonumen.top/gtuzvxpgoe.html

Ruby: exit 1
来源：http://hz.chenlongwang.top/gtmmiajlov.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj202588.top/gtcjsjzujb.html

[M06] 向标准错误输出
来源：http://hz.pycfn.com/gtlvbpdbgf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtdqcguimm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.c1oappe.top/gtnjujwiqp.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtvhesxyep.html

TS:   console.error("err")
来源：http://hz.sweek.top/gtnehusyff.html

Java: System.err.println("err")
来源：http://hz.havefunace.top/gtqmximyjn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tian-w.cn/gtyoedjoxk.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtbhcqeoue.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ehwqpu.com/gtdemqbdgc.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtyoejkpuu.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gtsbhwjmyi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yueranfly.top/gtevjenaaa.html

JS:   require.main === module
来源：http://hz.quarkkingdee.top/gtuzlpnpbe.html

TS:   require.main === module
来源：http://hz.c1oappe.top/gtzipddtbc.html

Java: public static void main(String[] args)
来源：http://hz.sweek.top/gtrfseebdv.html

Go:   func main()
来源：http://hz.haohaochexian.top/gtlgrunkpk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.mhx1999.top/gtccwouqyh.html

C#:   static void Main(string[] args)
来源：http://hz.redwolf501.top/gtudkjnryr.html

[M08] 获取系统与运行时信息
来源：http://hz.aibaodan.cn/gtydpgckkd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shzxlz.cn/gtqccdowrp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zdqjudy.top/gtdfspfama.html

JS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtpsfdopfe.html

TS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtvomivffh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zdqjudy.top/gtcnclvxbz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.havefunace.top/gtsvkunzpv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtickcltdm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtjdpxhdvi.html

================================================================================
来源：http://hz.jianghu66.top/gtmwhyulll.html

N. 数据结构与算法
来源：http://hz.cucudq.cn/gtldackokx.html

================================================================================
来源：http://hz.gzhubu.top/gtnqkmftqj.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gtsthoypjq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigufen.top/gtlgfcudhl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenzaomai.com/gtnntdngkd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtraaveoaz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtkgpiygex.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtybtwbnpb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhengqikj.top/gtzpgeknjf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guowangkeji.top/gtjwfutcbm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cashguo.top/gtgprropgw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cashguo.top/gtziiewvsu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtnimbvemw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xylfe.cn/gtghjtealk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtpzqgaolb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtorfbpajx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gtchyfzitq.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtrpfwmcsc.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gttsappubv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj202588.top/gtowopqjup.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtgwtzvzlq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tianlin.xyz/gtxgcqntqi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigfzy.top/gttwawrpnh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gtdumfbvsv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtvikufdmz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shzxlz.cn/gtqmdhynqp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhoulong.xyz/gtdotrwgqa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangdashe.top/gtopllpunr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtoxichqgv.html

[N04] 斐波那契数列
来源：http://hz.pengpengdd.cyou/gtcjzvoxxl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtfmgszkqs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yvedp.cn/gtvzonnjjs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtixfmeahr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtywfvyqih.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhongyouzk.top/gtuqcmswwy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yueranfly.top/gtcymkfzqu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtzuvdwfon.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ppjwa.cn/gtamduurwx.html

[N05] 最大公约数
来源：http://hz.yueranfly.top/gtgquefsfp.html

Py:   math.gcd(a, b)
来源：http://hz.ydzc1.top/gtilmtgsxg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.andypj.xyz/gtruwklfte.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtyxioccku.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtnpwudmyq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtvrdhzwzf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zdqjudy.top/gtwniiqlak.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtueibzpgn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtsskkzzws.html

[N06] 判断回文字符串
来源：http://hz.aibaodan.cn/gtcbsjlosv.html

Py:   s == s[::-1]
来源：http://hz.fzhhl.top/gtyldsndqw.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gtpldlvqrf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtckdnitmm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtgolwordu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.fengsongda.top/gtfebvvvch.html

Go:   // 双指针从两端比较
来源：http://hz.yonumen.top/gtdxgmvyqq.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtjwimrsbh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtprfpxsvg.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258888.top/gtbvqypghm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.meibo888.top/gtbuoupczm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tian-w.cn/gtrvupxrpo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gtejxabvhm.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtlwluuemq.html

Java: // 手写 HashMap
来源：http://hz.zhengqikj.top/gthofuqapq.html

Go:   // 手写 map[int]int
来源：http://hz.cqqwz.cn/gtzzaxqqyw.html

Ruby: // 手写 Hash
来源：http://hz.aizwys.cn/gtvjdlajfd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shuidangran.top/gtspwvddlh.html

[N08] 生成全排列
来源：http://hz.zhixingplan.top/gtansvlblb.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtszqnflic.html

PHP:  // 手写递归交换
来源：http://hz.ivvv.top/gtpzwkguce.html

JS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtnmchvhdz.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtqrqzldhq.html

Java: // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtkrtwggbr.html

Go:   // 手写回溯递归
来源：http://hz.yonumen.top/gtpzfwanrg.html

Ruby: arr.permutation.to_a
来源：http://hz.yueranfly.top/gtvfsdhnuy.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtxahuclcx.html

[N09] 栈与队列
来源：http://hz.mhx1999.top/gtpiejprwg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.andypj.xyz/gtteghhodn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fzhhl.top/gtvcfqpqae.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenzaomai.com/gttfbptgfu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tianlin.xyz/gtnuasjzew.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guowangkeji.top/gtxjbntfoi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sxryk.cn/gtdlofvgjd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nwbrower.top/gthzfwdfks.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtckkkevkb.html

[N10] 链表节点定义
来源：http://hz.mhx1999.top/gtkpkgkhcc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhaomingkeji.xyz/gtfycmrpcz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dianchejie.cn/gtnkmbyotm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.bjfxy.top/gtnhfggjne.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yanxiufei.cn/gtwfnvpxvc.html

Java: class Node { int v; Node next; }
来源：http://hz.sufxvd.cn/gtkskxskiy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinyuanbaomall.cn/gtdbjpstkd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gtsqrzpjhh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.iojbl.cn/gtkiiiirre.html

[N11] 二叉树中序遍历
来源：http://hz.jinyuanbaomall.cn/gtwrhjdejy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuanzx.com/gtxbovsxdy.html

PHP:  // 手写递归函数
来源：http://hz.aibaodan.cn/gtpmffhjew.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtcenxarvm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtmxzluqmj.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gtwfjowhyd.html

Go:   // 手写递归
来源：http://hz.zhixingplan.top/gtasmhtatl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gotoacloud.top/gtyejkkihf.html

C#:   // 手写递归
来源：http://hz.jlsjyb.cn/gtiwfaztov.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cucudq.cn/gtrxmmizfe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gtwuirkdnq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gtzcyfxxbc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtazkyiagi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtasdlhgeu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtwnrayztr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xingfuxueyuan.xyz/gtvsrmmuqa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zycfv.cn/gtrvwkutjp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtwmxjdotx.html

================================================================================
来源：http://hz.fzhhl.top/gtjkyjkjrf.html

O. 并发与异步
来源：http://hz.zhixingplan.top/gtikenqrzv.html

================================================================================
来源：http://hz.pycfn.com/gtsuedmvhq.html

[O01] 启动一个线程
来源：http://hz.xuanzx.com/gtthbcaqcj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xingfuxueyuan.xyz/gtqpljjpbt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daxiang520.top/gtqfciliap.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gtgyzglcob.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtiquplsqg.html

Java: new Thread(() -> f()).start()
来源：http://hz.tianlin.xyz/gtktfopnyo.html

Go:   go f()
来源：http://hz.yangfankeji.com/gtoddvmlae.html

Ruby: Thread.new { f }
来源：http://hz.cashguo.top/gtokgytnhc.html

C#:   Task.Run(() => F());
来源：http://hz.birdmap.top/gtgizxiopq.html

[O02] 使用线程池
来源：http://hz.zhiwuduotai.top/gtviyxzkhe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenlongwang.top/gtjqwpvnqg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtjptlypyn.html

JS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gtqowtxxuf.html

TS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtfiksoxdq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.havefunace.top/gtmgmdrfrw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.aizwys.cn/gthjzwpdww.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhongyouzk.top/gtdszjufzu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sweek.top/gtgidjgaga.html

[O03] 加锁保护共享数据
来源：http://hz.vqdsnc.cn/gtbmotgdag.html

Py:   with lock: shared += 1
来源：http://hz.gotoacloud.top/gtgeaymxwl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtvnybrule.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tianlin.xyz/gtdbrjywcf.html

TS:   // 同 JS
来源：http://hz.iojbl.cn/gtnnhhbipk.html

Java: synchronized (this) { shared++; }
来源：http://hz.yvedp.cn/gtlkisopvb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuetiantiany.cn/gtkizeyape.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuanzhike.top/gtgkrewvwg.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtjwjzmlmw.html

[O04] 定义异步函数并等待
来源：http://hz.gaohongyu789.top/gtqqavjaqj.html

Py:   async def f():⏎    await g()
来源：http://hz.ybcxt.top/gtqjvbavgv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhiwuduotai.top/gtbbvensrr.html

JS:   async function f() { await g(); }
来源：http://hz.jqgufenzy.top/gtrnnwoiyv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sufxvd.cn/gtglffnoit.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gtuaxsbuhr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.dianchejie.cn/gtbkyvzffs.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xziqi.cn/gtipwltgrr.html

C#:   async Task F() { await G(); }
来源：http://hz.sxryk.cn/gtmewoyeyp.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtiuwzljdo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtiyeabfvs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.daxiang520.top/gtsmfhcjkx.html

JS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gttptqgtkj.html

TS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtwhebdxxq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenlongwang.top/gtnhyxngmp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aizwys.cn/gtxosrczyq.html

Ruby: threads.map(&:join)
来源：http://hz.tianlin.xyz/gtdypcxwjj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aizwys.cn/gtyigkxvut.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtphehnmfe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.aizwys.cn/gtljezfzfj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pycfn.com/gtltuplsyp.html

JS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gtzekuhauj.html

TS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gthhmvhxuo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigfzy.top/gtsiyslitr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jiagoushi.top/gtiicbwhtg.html

Ruby: // fork 块
来源：http://hz.xinyue.icu/gtitzaaqij.html

C#:   Parallel.For
来源：http://hz.zhoulong.xyz/gtnxzyywwv.html

================================================================================
来源：http://hz.zhengqikj.top/gtxffncoao.html

P. 常用工具函数
来源：http://hz.tanke756.top/gtgqyumudt.html

================================================================================
来源：http://hz.havefunace.top/gtlybirwte.html

[P01] 生成 UUID
来源：http://hz.yuxming.cn/gtclrtaoor.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gtflmunltw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinyuanbaomall.cn/gthxetklwo.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtdxdnvcpw.html

TS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtkywifltf.html

Java: UUID.randomUUID().toString()
来源：http://hz.hysaishi.cn/gtkxiirpqh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.vqdsnc.cn/gtrsncfosk.html

Ruby: SecureRandom.uuid
来源：http://hz.sweek.top/gthkcihzuc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtxfbqtijy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daxiang520.top/gtrbvtjarm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydjk.org.cn/gtibztctmq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.vqdsnc.cn/gtthupffnp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sysykeji.top/gtammshpxg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gogol.net.cn/gtztcxlpmq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ybcxt.top/gtjluxbxsq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtmoxfikph.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangkeji.top/gtnzvngeyj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhoulong.xyz/gtouaowqzq.html

[P03] 生成短随机字符串
来源：http://hz.chenjidiqi.icu/gtvvwdidsb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.andypj.xyz/gtlzbmglhd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinghuilouyu.cn/gtrxhabikv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.snrcjt.cn/gturbxtwmh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenzaomai.com/gtywwjskwe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shzxlz.cn/gtobzuutez.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tianlin.xyz/gturifsgop.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cucudq.cn/gtzfqeqinu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258888.top/gtiaodvgxc.html

[P04] 求长度
来源：http://hz.wangdashe.top/gtsvaviowr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgufenzy.top/gtxnigihdx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gthmfvmyyj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gteqjvjsmj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhoulong.xyz/gtzniwtcnj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zycfv.cn/gtfdrdtjsb.html

Go:   len(arr);  len(m)
来源：http://hz.bjfxy.top/gtoxppfzjq.html

Ruby: x.length;  x.size
来源：http://hz.chenlongwang.top/gtdbmvcaju.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ppjwa.cn/gtoamgufxb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nwbrower.top/gtuptfbqcb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.bjfxy.top/gtmdktczov.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhixingplan.top/gtzekdpybb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yanxiufei.cn/gtygswlgbb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guannengcc.top/gtqgokrulf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hysaishi.cn/gtctgdkhxd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ywan-chungtsiang.top/gtehcymqlh.html

Ruby: a == b
来源：http://hz.pycfn.com/gtbtkblxpa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shangyingyoupin.top/gtlfnjyccd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhengqikj.top/gtgfqvoait.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gtpefwncid.html

PHP:  if (empty($x)) {}
来源：http://hz.yuxming.cn/gtplapizzy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xuetiantiany.cn/gtfcixxxuh.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtbhxqbqkf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtboftooou.html

Go:   if x == nil {}
来源：http://hz.nanxuanxn.top/gtyzpxdnit.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sweek.top/gtylgupzkv.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangkeji.top/gtgjabbtzy.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gtaefzfapt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tianlin.xyz/gthqhwkjam.html

PHP:  // 手写时间戳比较
来源：http://hz.tianlin.xyz/gtusngwwsq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhixingplan.top/gttjmksrdr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtfewzkbeo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fengsongda.top/gtvfeppqke.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtdzreitck.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.0kj1m.cn/gtmfhkitwn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtshxhuaey.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gtcychpjxy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yvedp.cn/gtsjdrjaxa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gtfsgdogrz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sxryk.cn/gtrjmomvoe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenzaomai.com/gtbydumugu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nwbrower.top/gtilxacsux.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gtjrdwpmov.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.redwolf501.top/gtmwbunrqo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.vqdsnc.cn/gtbdpcbxxs.html

================================================================================
来源：http://hz.yangfankeji.com/gtkvbodpuf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.svipenyu.cn/gtvibyccef.html

================================================================================
来源：http://hz.daxiang520.top/gtmxljmrum.html

[Q01] 创建表
来源：http://hz.52xcode.cn/gtcbmjepea.html

CREATE TABLE users (
来源：http://hz.chenjidiqi.icu/gtefhovatw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gthiugnjeq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cdnleiting.top/gtidadkuyp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuanzx.com/gtpvjnyhba.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhongyouzk.top/gtefewqtah.html

);
来源：http://hz.jinqigfzy.top/gtpwgxifmu.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gtezovlufv.html

CREATE TABLE orders (
来源：http://hz.dianchejie.cn/gtkjcjftgh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtygqanzwc.html

user_id INT NOT NULL,
来源：http://hz.tanke756.top/gtscpyigfc.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gteagtfqiz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtsardvqob.html

);
来源：http://hz.pengpengdd.cyou/gtxdjmldsl.html

[Q03] 增加列
来源：http://hz.andypj.xyz/gtwexqijfm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.iojbl.cn/gteluavzet.html

[Q04] 修改列类型
来源：http://hz.zhengqikj.top/gtwpnoytwn.html


<!-- 参考信息 -->