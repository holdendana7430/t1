代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtkfossklj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daxiang520.top/gtllzvthee.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ivvv.top/gtdhloyjmb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pycfn.com/gtxqsqozha.html

[M04] 获取当前工作目录
来源：http://hz.fzhhl.top/gtsehnkzfs.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtcmntzgjy.html

PHP:  getcwd();
来源：http://hz.yangfankeji.com/gtpjfgaciv.html

JS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtslteyhyc.html

TS:   process.cwd()
来源：http://hz.snrcjt.cn/gtafjjffgk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hongshengwenyu.top/gtwpzvydms.html

Go:   os.Getwd()
来源：http://hz.ivvv.top/gtrpnfgepd.html

Ruby: Dir.pwd
来源：http://hz.hammf.cn/gtfpzrzgis.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtrvfxyoko.html

[M05] 设置退出码
来源：http://hz.mhx1999.top/gtqbkbmnic.html

Py:   sys.exit(1)
来源：http://hz.sysykeji.top/gtkntkpdta.html

PHP:  exit(1);
来源：http://hz.daria6918.cn/gtmnvojvgr.html

JS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtmkbhdzuq.html

TS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gtoxvlukik.html

Java: System.exit(1)
来源：http://hz.yj202588.top/gtzyzhzfhg.html

Go:   os.Exit(1)
来源：http://hz.birdmap.top/gtvkmzplun.html

Ruby: exit 1
来源：http://hz.guannengcc.top/gtylmfccwf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.9152youxi.cn/gteksclrbc.html

[M06] 向标准错误输出
来源：http://hz.gzhubu.top/gtfmkshkex.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtyjqcqezh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hammf.cn/gtyqquankk.html

JS:   console.error("err")
来源：http://hz.ydjk.org.cn/gteqmhbews.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtwtgyuexy.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gtkjlvjyzn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.wangshuangyany.cn/gtcvezkvnj.html

Ruby: warn "err"
来源：http://hz.fzhhl.top/gtluchlfsp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ehwqpu.com/gtzajpwddw.html

[M07] 判断是否为主入口
来源：http://hz.c1oappe.top/gtycsuocbg.html

Py:   if __name__ == "__main__":
来源：http://hz.fzhhl.top/gthfnymefi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yongpay.top/gtlswkydjf.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gtlytohdux.html

TS:   require.main === module
来源：http://hz.hysaishi.cn/gtpxdkijry.html

Java: public static void main(String[] args)
来源：http://hz.chenlongwang.top/gtnxksokhv.html

Go:   func main()
来源：http://hz.xziqi.cn/gtelyqkbnu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258888.top/gttnmhxygw.html

C#:   static void Main(string[] args)
来源：http://hz.hammf.cn/gtdyurgvmn.html

[M08] 获取系统与运行时信息
来源：http://hz.quarkkingdee.top/gtmwinlbse.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtvgotlklv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hfpthk.cn/gtjqlmeppm.html

JS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtnhuwwuoe.html

TS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gthxkewfdz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgufenzy.top/gtroyrvxqs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shangyingyoupin.top/gtwipuzlbc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hongshengwenyu.top/gtalquucsw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gtzbaemyiy.html

================================================================================
来源：http://hz.birdmap.top/gtaesjogxp.html

N. 数据结构与算法
来源：http://hz.dianchejie.cn/gtggtdahho.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfzosmqan.html

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtchshzbpa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.52xcode.cn/gtzqdkggcc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fzhhl.top/gtcwjoiylg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtezsshtez.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtrshjugrc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sxryk.cn/gtisazrbsj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhongyouzk.top/gthnrhelgt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj20258.top/gtbjbaslzk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daria6918.cn/gtvvkcyxgk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxuanxn.top/gtiudrpblx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtsuwrnlcn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.52xcode.cn/gtmbaunapu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtyqiidnce.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtkxyznkzk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hysaishi.cn/gtdrtdpgsl.html

Go:   slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtfqpkhtmv.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtwghuhwys.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtqgkiwsfj.html

[N03] 快速排序（分治示例）
来源：http://hz.shangyingyoupin.top/gtofqitpud.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.smart0.xyz/gtzmpkelkb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj202588.top/gthzlvpyng.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtxcbkcdyu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtqlesafdf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.snrcjt.cn/gthmcckkva.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shzxlz.cn/gtniiliwug.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.mhx1999.top/gtdnufaefq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.nanxuanxn.top/gtfialyegs.html

[N04] 斐波那契数列
来源：http://hz.xziqi.cn/gtmsxnzpmw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtkvxohnga.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xinyue.icu/gtthqgmuzq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtxafhriig.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.mhx1999.top/gtrcalcyhj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangtech.top/gtlnyjvmjo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hammf.cn/gthqofqdoy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtmbiorgad.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtnkhfcfxc.html

[N05] 最大公约数
来源：http://hz.aizwys.cn/gtyzytqotq.html

Py:   math.gcd(a, b)
来源：http://hz.svipenyu.cn/gtwrmfxwsr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangdashe.top/gtjrtiaqiv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtcounatjh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gthtkxtgia.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuxming.cn/gtwabiolah.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sysykeji.top/gtaamtvxoq.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gtvprdbhyz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhixingplan.top/gtpwrmjmuy.html

[N06] 判断回文字符串
来源：http://hz.jlsjyb.cn/gtszzioljz.html

Py:   s == s[::-1]
来源：http://hz.chenlongwang.top/gtyphnjwgi.html

PHP:  $s === strrev($s);
来源：http://hz.zhengqikj.top/gtdmorugvx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtypqwtpik.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtfcfwcazu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangshuangyany.cn/gtojezrwct.html

Go:   // 双指针从两端比较
来源：http://hz.cucudq.cn/gtqrkyffmc.html

Ruby: s == s.reverse
来源：http://hz.svipenyu.cn/gtpcecsxvx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtxupinrht.html

[N07] 两数之和（返回下标）
来源：http://hz.zhongyouzk.top/gtibvulyyh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtujtzivth.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aizwys.cn/gtsypwgofy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgfzy.top/gtjwfegzfv.html

TS:   // 手写 Map<string, number>
来源：http://hz.gaohongyu789.top/gtpayatiny.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtpgvotyac.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258888.top/gtnrsfqnhq.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtbybtvqjt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cheryme.top/gtldvvqnei.html

[N08] 生成全排列
来源：http://hz.hnqzz.top/gtizqfxssd.html

Py:   itertools.permutations(arr)
来源：http://hz.xuanzx.com/gtustefyba.html

PHP:  // 手写递归交换
来源：http://hz.aizwys.cn/gtgqaqvqqu.html

JS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtrbysvifi.html

TS:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtsuvtacak.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtjafjiwdi.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtqihncgcv.html

Ruby: arr.permutation.to_a
来源：http://hz.dianchejie.cn/gtoibbkqgj.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtvpdxfpwv.html

[N09] 栈与队列
来源：http://hz.ybcxt.top/gtwmlqlnqw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xylfe.cn/gtgpgkdbnv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daria6918.cn/gtvsdumnjm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtgjjgjlbi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sweek.top/gtwkkovntr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtclsoeuln.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gzhubu.top/gtpcbtqoxn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gtfdbdjssa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.fzhhl.top/gtaqreiezf.html

[N10] 链表节点定义
来源：http://hz.jinyuanbaomall.cn/gtzaitmpjc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xylfe.cn/gtlprltwff.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jyoumei.cn/gtvutgoqyp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yangfankeji.com/gtlpleraqx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtimejmgzu.html

Java: class Node { int v; Node next; }
来源：http://hz.yongpay.top/gtkouitlch.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxinkj.top/gtvcwtpbol.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jianghu66.top/gtmirmqoil.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgufenzy.top/gtqypeihbp.html

[N11] 二叉树中序遍历
来源：http://hz.birdmap.top/gtfegmdfsw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhongyouzk.top/gtmgwixcpy.html

PHP:  // 手写递归函数
来源：http://hz.cashguo.top/gtwtfmfrzk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtyasazwwh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daxiang520.top/gtmunjdour.html

Java: // 手写递归
来源：http://hz.jinghuilouyu.cn/gtxxwdmgca.html

Go:   // 手写递归
来源：http://hz.chenlongwang.top/gtbtmgzczc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtncqkierh.html

C#:   // 手写递归
来源：http://hz.hnxiangtu.top/gtfoswziug.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gtwsgtwmka.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gteslgtorq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtzxguvwix.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtfwsvahom.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtyscmcdql.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtvlaecqtr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangtech.top/gtwrtqaihx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhongyouzk.top/gtacjjibqi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtbmqpgbnp.html

================================================================================
来源：http://hz.cdnleiting.top/gteqbzxanj.html

O. 并发与异步
来源：http://hz.zhengqikj.top/gtfcitoszs.html

================================================================================
来源：http://hz.snrcjt.cn/gtyjyqubso.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gtalsdbuyl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sweek.top/gtiwegdcza.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tianlin.xyz/gtyprtgsjb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhixingplan.top/gtidtoekwf.html

TS:   // 同 JS
来源：http://hz.aizwys.cn/gtmjhfwaqv.html

Java: new Thread(() -> f()).start()
来源：http://hz.daxiang520.top/gtlumvmnqz.html

Go:   go f()
来源：http://hz.yangfankeji.com/gtkncasqqh.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtmeqgdnzl.html

C#:   Task.Run(() => F());
来源：http://hz.yueranfly.top/gtxdxxhoyo.html

[O02] 使用线程池
来源：http://hz.hysaishi.cn/gtcdvvoeot.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhengqikj.top/gtrzycmyup.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shuidangran.top/gtldddogyw.html

JS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtvcrbubji.html

TS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtzsxgzbmd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.quarkkingdee.top/gtorhrmuqk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yueranfly.top/gtkidiqffx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.bjfxy.top/gtkhqkvlai.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhiwuduotai.top/gtcmdjtnjm.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtiurjnfop.html

Py:   with lock: shared += 1
来源：http://hz.snrcjt.cn/gtzojkimdr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yueranfly.top/gtkvaxziuh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhongyouzk.top/gttrgjxkmj.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtkwtqufnj.html

Java: synchronized (this) { shared++; }
来源：http://hz.meibo888.top/gtkrioafbo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ivvv.top/gtynpwyjow.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuanzx.com/gtactntdyi.html

C#:   lock (gate) { shared++; }
来源：http://hz.zycfv.cn/gtxblevrzh.html

[O04] 定义异步函数并等待
来源：http://hz.jinqigfzy.top/gtrhlfxirn.html

Py:   async def f():⏎    await g()
来源：http://hz.tian-w.cn/gtxnluhxbn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cdnleiting.top/gtfcezkxum.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtcoohibhu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yvedp.cn/gtnatgoiwj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.smart0.xyz/gtalfosyre.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.c1oappe.top/gtwdnqezfa.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtkziiddxl.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gtkiiblkxo.html

[O05] 并发执行并等待全部完成
来源：http://hz.hnqzz.top/gtmxhsgsnt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gtowybfaup.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yonumen.top/gtjuzzvqgg.html

JS:   await Promise.all(tasks)
来源：http://hz.vqdsnc.cn/gtcubenevy.html

TS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtgneizybk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dashuyun.cn/gtutnpwqio.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jlsjyb.cn/gtetzrfwoq.html

Ruby: threads.map(&:join)
来源：http://hz.snrcjt.cn/gtzwhrqkat.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zdqjudy.top/gtsujkjnfw.html

[O06] 使用进程池
来源：http://hz.pengpengdd.cyou/gtyqaopvmq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jianghu66.top/gtqzudjcme.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shzxlz.cn/gtpofdpcxv.html

JS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtfjzaxgbc.html

TS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtjdkavmvf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gzhubu.top/gtqdtyzfjk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhaomingkeji.xyz/gtclqukgue.html

Ruby: // fork 块
来源：http://hz.gaohongyu789.top/gtdcciwmiq.html

C#:   Parallel.For
来源：http://hz.dashuyun.cn/gtfhggftkz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdcfbezrr.html

P. 常用工具函数
来源：http://hz.yvedp.cn/gtmwusqnrh.html

================================================================================
来源：http://hz.snrcjt.cn/gtjwtopzat.html

[P01] 生成 UUID
来源：http://hz.dashuyun.cn/gtdxbloefn.html

Py:   str(uuid.uuid4())
来源：http://hz.316326.xyz/gtlihwhhla.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigufen.top/gtqruavljn.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258888.top/gtgjigpcaa.html

TS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtauzmqprz.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhoulong.xyz/gtpuykdkzk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.andypj.xyz/gtcwjebirn.html

Ruby: SecureRandom.uuid
来源：http://hz.xingfuxueyuan.xyz/gtzrxwxnjq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sweek.top/gtdfhrbhrx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ybcxt.top/gtlhwaarlf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.smart0.xyz/gthichrjdr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dianchejie.cn/gtagebboop.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hongshengwenyu.top/gtoimcgjtz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.kuanghao11.cn/gtjmrobjku.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhiwuduotai.top/gtjvztyijr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xinyue.icu/gtmznmpfib.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gteisidsuv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinqigfzy.top/gtbnxsjzqr.html

[P03] 生成短随机字符串
来源：http://hz.zhixingplan.top/gttdejaorv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pycfn.com/gtinbvpena.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zdqjudy.top/gtcqdedavf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtqpkdnyjf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtqkbkaquv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ywan-chungtsiang.top/gtiuoffzhd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tanke756.top/gtgrbaklqw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hongshengwenyu.top/gtfzcsuauh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.bjfxy.top/gtjgkfjtyj.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtvarctpxz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhongyouzk.top/gtuijryxvg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtysivtxpr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtarwiizqv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.redwolf501.top/gtphdyhubj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtcyuktzzt.html

Go:   len(arr);  len(m)
来源：http://hz.ybcxt.top/gtiuzbmehp.html

Ruby: x.length;  x.size
来源：http://hz.nanxinkj.top/gtfvfulffw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guannengcc.top/gtybmufxfc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinqigufen.top/gtkufqghnc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gtiyfluakc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gotoacloud.top/gtuuecehkn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zycfv.cn/gtuujxwatb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtmzihijzb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gtlmorrpgm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnxiangtu.top/gtzkdwdtdp.html

Ruby: a == b
来源：http://hz.vqdsnc.cn/gtcrpiowvp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinyuanbaomall.cn/gtbosbvhfa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daxiang520.top/gtdrwhwyuv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenlongwang.top/gtafznoczu.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtmfkqxzsz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pycfn.com/gtvathgchr.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtvxprhqyk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.havefunace.top/gtgngfoqzz.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtlpbdkcjh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jiagoushi.top/gtkspgehdq.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gtaxqhomam.html

[P07] 防抖与节流
来源：http://hz.nanxuanxn.top/gtcnclqgtb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hongshengwenyu.top/gtuvrbpmma.html

PHP:  // 手写时间戳比较
来源：http://hz.wangshuangyany.cn/gtklrpubpo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtitlzoglm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtukwrxcsc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cashguo.top/gtntntpizt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhijiandao.cn/gtcwduwxud.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ehwqpu.com/gthnzaexke.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tian-w.cn/gtlsrgkhqu.html

[P08] 处理浮点精度问题
来源：http://hz.zhoulong.xyz/gtdatwkyxj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.9152youxi.cn/gtkfciharv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tian-w.cn/gtvbwpebyn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guannengcc.top/gtsoyqdqcz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xinyue.icu/gthlkbjtdo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shangyingyoupin.top/gtdbtactua.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hammf.cn/gtvgrngjfn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yvedp.cn/gtsetlmoua.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zycfv.cn/gthhtfjfqp.html

================================================================================
来源：http://hz.daria6918.cn/gthlsvlvlg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cheryme.top/gtmcxlgwwc.html

================================================================================
来源：http://hz.gogol.net.cn/gtelnnbkog.html

[Q01] 创建表
来源：http://hz.zhengqikj.top/gtglwsjzhf.html

CREATE TABLE users (
来源：http://hz.smart0.xyz/gtvlfuwbmz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtmvdqjofb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yangfankeji.com/gtemdcnpux.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hywenlv.cn/gtjhvugxie.html


<!-- 参考信息 -->