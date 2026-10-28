代发 wailian999

TS:   process.cwd()
来源：http://hz.zhoulong.xyz/gttcxdupfa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ybcxt.top/gtkfvaskht.html

Go:   os.Getwd()
来源：http://hz.ybcxt.top/gtuzyrwlju.html

Ruby: Dir.pwd
来源：http://hz.gotoacloud.top/gtwbbcatte.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zycfv.cn/gtwrjzmoaq.html

[M05] 设置退出码
来源：http://hz.jyoumei.cn/gttrlprhaa.html

Py:   sys.exit(1)
来源：http://hz.xuanzx.com/gtimxmvwyx.html

PHP:  exit(1);
来源：http://hz.jinghuilouyu.cn/gtwhehxbrq.html

JS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtzrumyxbe.html

TS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtppmyaefc.html

Java: System.exit(1)
来源：http://hz.fzhhl.top/gtbazegjyx.html

Go:   os.Exit(1)
来源：http://hz.chenlongwang.top/gtciwtnhep.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtrazljsio.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenzaomai.com/gtrpdjpogd.html

[M06] 向标准错误输出
来源：http://hz.xziqi.cn/gtysnlngld.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhiwuduotai.top/gtiusloyei.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhixingplan.top/gtjraxwtbc.html

JS:   console.error("err")
来源：http://hz.yongpay.top/gtfwgruxyn.html

TS:   console.error("err")
来源：http://hz.yuxming.cn/gtbkdslpkp.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtuhhbtbhw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtouhyflwi.html

Ruby: warn "err"
来源：http://hz.wangshuangyany.cn/gtebejsbxr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yangfankeji.com/gtfswfuzfk.html

[M07] 判断是否为主入口
来源：http://hz.tianlin.xyz/gtrvfnmkho.html

Py:   if __name__ == "__main__":
来源：http://hz.aibaodan.cn/gtakfqnnpw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtrywipvmg.html

JS:   require.main === module
来源：http://hz.jyoumei.cn/gtaflvdhrx.html

TS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtscqlrgvw.html

Java: public static void main(String[] args)
来源：http://hz.ydzc1.top/gtuyartcak.html

Go:   func main()
来源：http://hz.vqdsnc.cn/gtmouwmrbd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj202588.top/gtttxwyxob.html

C#:   static void Main(string[] args)
来源：http://hz.pengpengdd.cyou/gthqrohckg.html

[M08] 获取系统与运行时信息
来源：http://hz.sweek.top/gtgrfccnqf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtxksjnpph.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jyoumei.cn/gtbxmrovoa.html

JS:   process.platform;  process.version
来源：http://hz.wangshuangyany.cn/gtyalvlsvy.html

TS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtckfwkcao.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.birdmap.top/gtfpzbdkyn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gtcsoufjna.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtqdzprzdn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtrxzlrbsc.html

================================================================================
来源：http://hz.daria6918.cn/gttjeajitl.html

N. 数据结构与算法
来源：http://hz.hywenlv.cn/gtjckcdygo.html

================================================================================
来源：http://hz.dashuyun.cn/gtriekkwoa.html

[N01] 二分查找（有序数组）
来源：http://hz.zhiwuduotai.top/gtqmtxhzsj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtmhisnoxi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pengpengdd.cyou/gtfkqcwvyo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gthiltdisb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gtaccidwui.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.mhx1999.top/gtalvticvm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aizwys.cn/gtakqcvcqp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtqnvvxbps.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtigmtksza.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pycfn.com/gtfyyeinuz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtfizcxgza.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gogol.net.cn/gtclmasqed.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtkxebyzdu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jianghu66.top/gtwgqiggvu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yuanzhike.top/gtyxxekzql.html

Go:   slices.Sort(arr)
来源：http://hz.yongpay.top/gtqdjhuykz.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtgbwfbfmi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.iojbl.cn/gtfpsakczz.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gtdoauuwzc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.316326.xyz/gtayqlngkb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ppjwa.cn/gtfmqmuosm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtmayqwolb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtqoyzyayn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hywenlv.cn/gtlochulvg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenjidiqi.icu/gtkixexlhe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenzaomai.com/gthzdnwsaf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sysykeji.top/gtbnoscoxc.html

[N04] 斐波那契数列
来源：http://hz.pengpengdd.cyou/gtmsufmzzp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtaxizvgav.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xingfuxueyuan.xyz/gtlhlejxto.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtwkqjjbtz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtqmeuueww.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258888.top/gtekibtkeg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gttymxheyy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtnloruokk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxinkj.top/gtokdnnkrl.html

[N05] 最大公约数
来源：http://hz.jiagoushi.top/gtgubeagdl.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangkeji.top/gtkzgvcjlk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenzaomai.com/gtjpobcten.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gthyrhxfvv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtojlhimvq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhengqikj.top/gtajkcylqh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guannengcc.top/gtuyhxxfyv.html

Ruby: a.gcd(b)
来源：http://hz.guowangkeji.top/gtsdebgndo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hammf.cn/gtncetqnre.html

[N06] 判断回文字符串
来源：http://hz.fengsongda.top/gtnilftpzc.html

Py:   s == s[::-1]
来源：http://hz.shangyingyoupin.top/gtqdgwexij.html

PHP:  $s === strrev($s);
来源：http://hz.hnxiangtu.top/gthziefhlm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtsawvbdjn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtetgxonws.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtxzdsqukz.html

Go:   // 双指针从两端比较
来源：http://hz.daxiang520.top/gtqfvadyfh.html

Ruby: s == s.reverse
来源：http://hz.hfpthk.cn/gtjxlusyeq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sysykeji.top/gtagzhteur.html

[N07] 两数之和（返回下标）
来源：http://hz.sxryk.cn/gtyalbutfn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhoulong.xyz/gtxfotkurq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuxming.cn/gtjwofqkgi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ivvv.top/gtbnjmarkh.html

TS:   // 手写 Map<string, number>
来源：http://hz.dianchejie.cn/gtcipydtcg.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtbbqzppbe.html

Go:   // 手写 map[int]int
来源：http://hz.zhoulong.xyz/gtcxbhswgy.html

Ruby: // 手写 Hash
来源：http://hz.tianlin.xyz/gtnoewwqbs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gotoacloud.top/gtxjzmlglr.html

[N08] 生成全排列
来源：http://hz.yanxiufei.cn/gtudohosyv.html

Py:   itertools.permutations(arr)
来源：http://hz.yangfankeji.com/gtbvogadhm.html

PHP:  // 手写递归交换
来源：http://hz.zhengqikj.top/gtehrqpmnb.html

JS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtkskzinct.html

TS:   // 手写回溯递归
来源：http://hz.pycfn.com/gthcvgxrmy.html

Java: // 手写回溯递归
来源：http://hz.hnqzz.top/gtnzpydqfg.html

Go:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtmxyamsuh.html

Ruby: arr.permutation.to_a
来源：http://hz.tianlin.xyz/gtjcobfkju.html

C#:   // 手写回溯递归
来源：http://hz.ivvv.top/gttgkgorxu.html

[N09] 栈与队列
来源：http://hz.hammf.cn/gteetvpfbm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigufen.top/gtvuhrvduv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangdashe.top/gtrkclmrxp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cdnleiting.top/gthgbrrbsi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.9152youxi.cn/gtjlgorbqq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinghuilouyu.cn/gtpljwxhah.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtolqwaswn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.havefunace.top/gtucaivsse.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gogol.net.cn/gtgddcipns.html

[N10] 链表节点定义
来源：http://hz.0kj1m.cn/gtikswdnch.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.316326.xyz/gtfrtvtjrn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fzhhl.top/gtvapaowgu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jlsjyb.cn/gtuwlcxrja.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.haohaochexian.top/gtwkceysyu.html

Java: class Node { int v; Node next; }
来源：http://hz.pycfn.com/gtgngjpehr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gteoexspba.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tian-w.cn/gteeglfffl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtomzohtyy.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258.top/gtsrqsfggi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yangfankeji.com/gtbtpruhxd.html

PHP:  // 手写递归函数
来源：http://hz.hammf.cn/gtfycbhoyg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtfksrwdru.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtnhlpkutu.html

Java: // 手写递归
来源：http://hz.chenzaomai.com/gtuuvebsvl.html

Go:   // 手写递归
来源：http://hz.cqqwz.cn/gtntmyoecs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shangyingyoupin.top/gtbffqkfwa.html

C#:   // 手写递归
来源：http://hz.nwbrower.top/gtqgzzthia.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhiwuduotai.top/gtujvodopw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yuanzhike.top/gtxphqbndk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guannengcc.top/gtjrenifnt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtuieawbqx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtkkggscrr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.9152youxi.cn/gtkxgkmbia.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj20258888.top/gtottpuwoi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.snrcjt.cn/gtbfzipbpq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtvyktutmb.html

================================================================================
来源：http://hz.pycfn.com/gtswisokdq.html

O. 并发与异步
来源：http://hz.iojbl.cn/gtlecjrhte.html

================================================================================
来源：http://hz.cheryme.top/gtigaxztmx.html

[O01] 启动一个线程
来源：http://hz.zhongyouzk.top/gtmbpjgbwu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daxiang520.top/gtsywmxktm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenlongwang.top/gtkwfumiae.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jiagoushi.top/gtecnvwixr.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gtqsnunzfr.html

Java: new Thread(() -> f()).start()
来源：http://hz.c1oappe.top/gtbbrbutbt.html

Go:   go f()
来源：http://hz.chenjidiqi.icu/gtxptfmspi.html

Ruby: Thread.new { f }
来源：http://hz.aizwys.cn/gtekkrywpr.html

C#:   Task.Run(() => F());
来源：http://hz.sufxvd.cn/gtokimzoyq.html

[O02] 使用线程池
来源：http://hz.jianghu66.top/gtmrbnngdk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gaohongyu789.top/gtbrlfujcr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.andypj.xyz/gtdzhhwdgi.html

JS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtalzgwvxg.html

TS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtlhinjapx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhiwuduotai.top/gtlhqugfqo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.aibaodan.cn/gtxldccjrj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tian-w.cn/gtcghkyhxb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gttkrgbscc.html

[O03] 加锁保护共享数据
来源：http://hz.cqqwz.cn/gtrqzbtwns.html

Py:   with lock: shared += 1
来源：http://hz.ivvv.top/gtzxvelrjg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aibaodan.cn/gtbrdhoscy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.vqdsnc.cn/gtwyrhrhxg.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtchcmqiow.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtboeatsvf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hfpthk.cn/gtdfwvlyas.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hywenlv.cn/gthzzjgzuu.html

C#:   lock (gate) { shared++; }
来源：http://hz.cdnleiting.top/gtjolwdayx.html

[O04] 定义异步函数并等待
来源：http://hz.fengsongda.top/gtoeaqxknr.html

Py:   async def f():⏎    await g()
来源：http://hz.yuxming.cn/gtoieqeyku.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuxming.cn/gtwcptokye.html

JS:   async function f() { await g(); }
来源：http://hz.nanxinkj.top/gtrqfmllvj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jqgfzy.top/gtiakuxsjq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.redwolf501.top/gtdnhncior.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtepxoqvxo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.0kj1m.cn/gtbolgsktc.html

C#:   async Task F() { await G(); }
来源：http://hz.smart0.xyz/gtaenotgaz.html

[O05] 并发执行并等待全部完成
来源：http://hz.aibaodan.cn/gtosnqjrxy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinyuanbaomall.cn/gtulrzgnbm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jlsjyb.cn/gtxpcwtunj.html

JS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtxuvcsnmr.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtcycceopf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hongshengwenyu.top/gtwnsqjhxk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.wangdashe.top/gthyovezfk.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtwrjwyudb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nwbrower.top/gtsvazdidp.html

[O06] 使用进程池
来源：http://hz.gzhubu.top/gtsuyxkptu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sysykeji.top/gtcbbcubsp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtfvrhigxw.html

JS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtzjgcgdun.html

TS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtwziczxhv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guannengcc.top/gtclmfjnvl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gzhubu.top/gtenyglnhc.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtfpltjrvn.html

C#:   Parallel.For
来源：http://hz.chenjidiqi.icu/gtvxxutgzi.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgnwgmskl.html

P. 常用工具函数
来源：http://hz.sweek.top/gttdzabhlt.html

================================================================================
来源：http://hz.yuxming.cn/gtiwrofvjz.html

[P01] 生成 UUID
来源：http://hz.haohaochexian.top/gtdoyxjkpp.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangtech.top/gtazodofdu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.birdmap.top/gtxgcxhnth.html

JS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtnxkvvkop.html

TS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtbfeoatei.html

Java: UUID.randomUUID().toString()
来源：http://hz.chenzaomai.com/gttrhwcqqf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtqmnvhnve.html

Ruby: SecureRandom.uuid
来源：http://hz.chenzaomai.com/gtyarmfual.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jianghu66.top/gtbdiwyrdi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xingfuxueyuan.xyz/gtqdnwqanv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fzhhl.top/gteexwercs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigfzy.top/gtitayfyqp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydjk.org.cn/gtiazvlrxr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.mhx1999.top/gtejdpaado.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ehwqpu.com/gtfpizbnlu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cucudq.cn/gtjcumnwxl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.kuanghao11.cn/gtxozjymmo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gtugnffcjw.html

[P03] 生成短随机字符串
来源：http://hz.pengpengdd.cyou/gthfrhbkty.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yanxiufei.cn/gthqojphcu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuanzhike.top/gtethgapsn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtvyapbsql.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtumxyvrzz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtxkkodefo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.iojbl.cn/gtkjwfmmje.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.mhx1999.top/gthvifltxz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigufen.top/gtqkblqlly.html

[P04] 求长度
来源：http://hz.tian-w.cn/gtplrgeyie.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.feifeiyinyue.top/gtjnondvgu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ehwqpu.com/gtvhqxikmr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtgshwamoa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gttxdqghbz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gaohongyu789.top/gtpyggxito.html

Go:   len(arr);  len(m)
来源：http://hz.tianlin.xyz/gtdwbvxqci.html

Ruby: x.length;  x.size
来源：http://hz.zhijiandao.cn/gtkhdyizxp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.daxiang520.top/gtfsygplmc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.snrcjt.cn/gtvirfylcc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.haohaochexian.top/gtsolxynwg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtscfxdrbd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.haohaochexian.top/gtvrzwfklk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yangfankeji.com/gtriqwuweh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cashguo.top/gtxhvogoxa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.0kj1m.cn/gtilftiums.html

Ruby: a == b
来源：http://hz.jiagoushi.top/gtmsejfjsk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hysaishi.cn/gtfnvtvaqc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gtnakavklj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhengqikj.top/gtxihxhohp.html

PHP:  if (empty($x)) {}
来源：http://hz.xuanzx.com/gthhxmzlwu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gaohongyu789.top/gtnserlqmh.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gtlmbluwcn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.smart0.xyz/gtihznrloy.html

Go:   if x == nil {}
来源：http://hz.mhx1999.top/gtiunrnduh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daxiang520.top/gtkxyxeqxz.html

C#:   if (x is null) {}
来源：http://hz.zhiwuduotai.top/gtbtcivneh.html

[P07] 防抖与节流
来源：http://hz.sysykeji.top/gtrnayxgtm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gogol.net.cn/gtadsaouot.html

PHP:  // 手写时间戳比较
来源：http://hz.yangfankeji.com/gtvapaajkr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtwposjcgo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gtyfcsudhk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ivvv.top/gtnjjtzbsh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.9152youxi.cn/gttrvrulmw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sufxvd.cn/gtacydaiit.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sxryk.cn/gtcgfmjlet.html

[P08] 处理浮点精度问题
来源：http://hz.yvedp.cn/gtkpsfciyw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtwbbcjciw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhaomingkeji.xyz/gtdsntmzzw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhongyouzk.top/gtxqzijmtr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.kuanghao11.cn/gtnxeklmfp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhengqikj.top/gtlnkwmacz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.havefunace.top/gtwfogyqkb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangdashe.top/gtwgenwtov.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ehwqpu.com/gttwfdbptg.html

================================================================================
来源：http://hz.meibo888.top/gtamnhuerc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dashuyun.cn/gtuzpmjmsp.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqgjuiicx.html

[Q01] 创建表
来源：http://hz.yj20258888.top/gtlacapxlq.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gthfczizan.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gttoaniuhk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258888.top/gtgitgqbgg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yvedp.cn/gteuqygseo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sysykeji.top/gtcwvqsjzc.html

);
来源：http://hz.cqqwz.cn/gtcuhpzgdr.html

[Q02] 创建带外键的表
来源：http://hz.hnqzz.top/gtqniooebw.html

CREATE TABLE orders (
来源：http://hz.sufxvd.cn/gtufrwrbbn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gtemaokrim.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtrxfuempp.html

amount DECIMAL(10, 2),
来源：http://hz.fengsongda.top/gtoayhiryf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtrweqgpye.html


<!-- 参考信息 -->