代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuxming.cn/gtcwgqmkyh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daxiang520.top/gtldmtidex.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shzxlz.cn/gtgnkfuhqt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tanke756.top/gtkwcpdnlm.html

[M04] 获取当前工作目录
来源：http://hz.cqqwz.cn/gtexjdzrmr.html

Py:   os.getcwd()
来源：http://hz.hnxiangtu.top/gthvyqneta.html

PHP:  getcwd();
来源：http://hz.guowangkeji.top/gtuyjbrplv.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtqupbpdrq.html

TS:   process.cwd()
来源：http://hz.yangfankeji.com/gtadhdptey.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gzhubu.top/gtlozvshmg.html

Go:   os.Getwd()
来源：http://hz.ydjk.org.cn/gtkhktgwwd.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gtjfbelzcy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ivvv.top/gtwkycimyh.html

[M05] 设置退出码
来源：http://hz.hfpthk.cn/gtyfvgwspq.html

Py:   sys.exit(1)
来源：http://hz.xuetiantiany.cn/gtkwllgzdh.html

PHP:  exit(1);
来源：http://hz.zdqjudy.top/gtluzqxefw.html

JS:   process.exit(1)
来源：http://hz.yueranfly.top/gtsyxuxgxf.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtcfdsnotd.html

Java: System.exit(1)
来源：http://hz.xuanzx.com/gtkfphjiev.html

Go:   os.Exit(1)
来源：http://hz.c1oappe.top/gtvnzerdhw.html

Ruby: exit 1
来源：http://hz.jqgfzy.top/gtjjfomqnj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgfzy.top/gtcqiylooj.html

[M06] 向标准错误输出
来源：http://hz.yj20258888.top/gtyudmxqnb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gthiyhfooo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.9152youxi.cn/gtrumlodlq.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtrquozpkv.html

TS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtxeldhzsx.html

Java: System.err.println("err")
来源：http://hz.shzxlz.cn/gtowqexjny.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.haohaochexian.top/gtshsmxqkb.html

Ruby: warn "err"
来源：http://hz.yj202588.top/gthpqaljib.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.birdmap.top/gtramqqxyi.html

[M07] 判断是否为主入口
来源：http://hz.birdmap.top/gtcwvbrazm.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtkrrddpey.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ivvv.top/gtrdlbxxpa.html

JS:   require.main === module
来源：http://hz.jianghu66.top/gtuoghlygg.html

TS:   require.main === module
来源：http://hz.ybcxt.top/gtjyeofhal.html

Java: public static void main(String[] args)
来源：http://hz.meibo888.top/gtkbdvzjfs.html

Go:   func main()
来源：http://hz.hammf.cn/gtsndizfwc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhoulong.xyz/gtsfwkposu.html

C#:   static void Main(string[] args)
来源：http://hz.jinghuilouyu.cn/gtlgzxdmrr.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gtvsfmyqgi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yueranfly.top/gtvccosqyd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jianghu66.top/gtrpirqqwu.html

JS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gttazcxuro.html

TS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtgfaivhae.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhixingplan.top/gtxjzvhizd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pycfn.com/gtjivuivvh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtrukieivk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.quarkkingdee.top/gtdziwdylv.html

================================================================================
来源：http://hz.svipenyu.cn/gteeddeser.html

N. 数据结构与算法
来源：http://hz.meibo888.top/gtqwuzbyet.html

================================================================================
来源：http://hz.ppjwa.cn/gtpnvgdipq.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gtszvzuqej.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tian-w.cn/gtiiliregp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gtqfvpmaqb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtlpdkppgm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj202588.top/gtjdyaovzd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zdqjudy.top/gtmjdkllbz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jianghu66.top/gtqivjqlmr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yueranfly.top/gtglyycewc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cheryme.top/gtsetnqvgb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtlubtgioe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtwcqqswgn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgufenzy.top/gtqxcpfhua.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtwlzfhdba.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gteuokyyjl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xziqi.cn/gtutetjkbe.html

Go:   slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtkgxqtikj.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtbuqflebc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.quarkkingdee.top/gtuclgnpuw.html

[N03] 快速排序（分治示例）
来源：http://hz.zhiwuduotai.top/gtvpjthfdb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenjidiqi.icu/gtfgwaumwm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ydjk.org.cn/gtswnvlzoa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fengsongda.top/gtpfgfwstg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtagydzsph.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ppjwa.cn/gtqvfsllkp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ehwqpu.com/gtmiwqvjrv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.9152youxi.cn/gtqcetmvys.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgufenzy.top/gtcikljvek.html

[N04] 斐波那契数列
来源：http://hz.vqdsnc.cn/gttzstfsls.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtijxnqolu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gthkeyuncj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtwhellfrq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtjofpuryt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtqtxrzboo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtwuodxfgh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtvwahcnwt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtvbcqzciy.html

[N05] 最大公约数
来源：http://hz.zhongyouzk.top/gtmykscaaj.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gthvetdvlh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jyoumei.cn/gtkuezsdbh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gtmhqhstyu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtvivpsdhl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guowangkeji.top/gtwkpvryuj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jiagoushi.top/gtttojwjrs.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gthqptumed.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hongshengwenyu.top/gtgilzpvvc.html

[N06] 判断回文字符串
来源：http://hz.xylfe.cn/gtbqrxaing.html

Py:   s == s[::-1]
来源：http://hz.smart0.xyz/gtbayeisyf.html

PHP:  $s === strrev($s);
来源：http://hz.andypj.xyz/gtqypllqhv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtryblkepz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtqvkdjlcl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj202588.top/gtvtmpyfzx.html

Go:   // 双指针从两端比较
来源：http://hz.316326.xyz/gtuwlvbtmj.html

Ruby: s == s.reverse
来源：http://hz.jlsjyb.cn/gtidzwcoef.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtapcngbgb.html

[N07] 两数之和（返回下标）
来源：http://hz.yvedp.cn/gtlzzzobtj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.9152youxi.cn/gteogojivb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydjk.org.cn/gtqmdckttw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.birdmap.top/gttzrgygix.html

TS:   // 手写 Map<string, number>
来源：http://hz.sweek.top/gtcbutrvlk.html

Java: // 手写 HashMap
来源：http://hz.jiagoushi.top/gtmoyybrgw.html

Go:   // 手写 map[int]int
来源：http://hz.zhiwuduotai.top/gtcjxgndmf.html

Ruby: // 手写 Hash
来源：http://hz.xziqi.cn/gthlgqnlst.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hysaishi.cn/gtwwnmacsk.html

[N08] 生成全排列
来源：http://hz.jinghuilouyu.cn/gtakvqtkqy.html

Py:   itertools.permutations(arr)
来源：http://hz.yangfankeji.com/gtbhmmwnjm.html

PHP:  // 手写递归交换
来源：http://hz.meibo888.top/gtfxeqrmwx.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtrblkdlqd.html

TS:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtxikxhlfu.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gtfuseswlx.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtbrtvhgfx.html

Ruby: arr.permutation.to_a
来源：http://hz.ivvv.top/gtbyyocegd.html

C#:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtehibsyzg.html

[N09] 栈与队列
来源：http://hz.sysykeji.top/gttlozxlbf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shuidangran.top/gtdzqfmgwz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cdnleiting.top/gtizjdlxwi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.bjfxy.top/gtuzvdgecj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cqqwz.cn/gtuxqnybxy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtfjyqtpiq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gtpyuqorys.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtfwwignxk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daxiang520.top/gtxjghgfar.html

[N10] 链表节点定义
来源：http://hz.guowangkeji.top/gtbrxsstwc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258888.top/gtcgmwdlqq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangkeji.top/gtirtbfeln.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gtrttrmxaw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.aizwys.cn/gtvllnytws.html

Java: class Node { int v; Node next; }
来源：http://hz.jinghuilouyu.cn/gtchrcxqcn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj202588.top/gteklnpptn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sweek.top/gtjjldxxhu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.iojbl.cn/gtkstvffsr.html

[N11] 二叉树中序遍历
来源：http://hz.gzhubu.top/gtyhocnkla.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuetiantiany.cn/gtimauffsm.html

PHP:  // 手写递归函数
来源：http://hz.xziqi.cn/gtppdycydh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtjsqxmxem.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtehgkddcl.html

Java: // 手写递归
来源：http://hz.gzhubu.top/gtyltafjpx.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gtpdbnbpeb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ppjwa.cn/gtsvpptbls.html

C#:   // 手写递归
来源：http://hz.aibaodan.cn/gtowtjgjfw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gtudpjedlq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hfpthk.cn/gtcigfhycw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xingfuxueyuan.xyz/gtpjapbkmo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtzypejlaq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtjzmcmbij.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtsgwqxoye.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xziqi.cn/gtjspdrcqc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gtxyycppcq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtiulueuqk.html

================================================================================
来源：http://hz.nanxinkj.top/gtbrxivbqa.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtbojneicw.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtyqojxolb.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtffkwqhbf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ivvv.top/gtnkfkvnlj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xziqi.cn/gteifspben.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ydjk.org.cn/gtisqxszmc.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtbmvgtrgc.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gthbipbhsm.html

Go:   go f()
来源：http://hz.aibaodan.cn/gtqrfaevhl.html

Ruby: Thread.new { f }
来源：http://hz.aibaodan.cn/gtusjomkrv.html

C#:   Task.Run(() => F());
来源：http://hz.gaohongyu789.top/gtjjhdutcj.html

[O02] 使用线程池
来源：http://hz.yj20258.top/gtwbllmktf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xziqi.cn/gtemdkjaer.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sufxvd.cn/gtsohadhfb.html

JS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtongrbhfv.html

TS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtycrxzlec.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnxiangtu.top/gttduysxyk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fengsongda.top/gtudgmuxie.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gtpzabfbit.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxuanxn.top/gtewwfmycn.html

[O03] 加锁保护共享数据
来源：http://hz.mhx1999.top/gtldclbxcp.html

Py:   with lock: shared += 1
来源：http://hz.shzxlz.cn/gtwxlmlseb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhixingplan.top/gtszmeljwq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yanxiufei.cn/gtxmtymzlm.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gteemlqmlm.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydjk.org.cn/gtutiagzae.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.redwolf501.top/gtsxseghhj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hywenlv.cn/gtdbszlwaf.html

C#:   lock (gate) { shared++; }
来源：http://hz.ppjwa.cn/gtwopmfnrl.html

[O04] 定义异步函数并等待
来源：http://hz.sweek.top/gthkmkwjwp.html

Py:   async def f():⏎    await g()
来源：http://hz.aizwys.cn/gtgoctmrtj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gtktlduonn.html

JS:   async function f() { await g(); }
来源：http://hz.wangdashe.top/gtemqptlcx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtbjfzanak.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuanzhike.top/gtbjelzupx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cucudq.cn/gtrpjxukgr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenzaomai.com/gteneruwva.html

C#:   async Task F() { await G(); }
来源：http://hz.yanxiufei.cn/gtsbrsqlpe.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenzaomai.com/gtngsrbmiy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.dashuyun.cn/gtsqepjdxz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenlongwang.top/gtdxmdxpon.html

JS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtunbdyzub.html

TS:   await Promise.all(tasks)
来源：http://hz.chenzaomai.com/gtfdzggcxh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.vqdsnc.cn/gtrethnmoj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.havefunace.top/gtrhyvtdip.html

Ruby: threads.map(&:join)
来源：http://hz.xziqi.cn/gtcarpgdbn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258888.top/gtlnihqqpj.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gtayrukgrg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangshuangyany.cn/gthxcrgzhv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gthvihzjgl.html

JS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtcviwyuqg.html

TS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtvnvpwalj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gteypwcmwo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pengpengdd.cyou/gtuygkdtnb.html

Ruby: // fork 块
来源：http://hz.jinqigfzy.top/gtufzbyndo.html

C#:   Parallel.For
来源：http://hz.dashuyun.cn/gtgwomoaik.html

================================================================================
来源：http://hz.zycfv.cn/gtmydjcuaa.html

P. 常用工具函数
来源：http://hz.jinqigfzy.top/gtmkihhuti.html

================================================================================
来源：http://hz.9152youxi.cn/gtkbzzlifl.html

[P01] 生成 UUID
来源：http://hz.birdmap.top/gtumnfcfsv.html

Py:   str(uuid.uuid4())
来源：http://hz.shangyingyoupin.top/gteccgxzvi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xingfuxueyuan.xyz/gtynjcaqzu.html

JS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gthbiqhckk.html

TS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtzvsumdwa.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnqzz.top/gtcwucigla.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shuidangran.top/gtlbjtvqxg.html

Ruby: SecureRandom.uuid
来源：http://hz.zhaomingkeji.xyz/gtiozwbsum.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhaomingkeji.xyz/gtelenxwjj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xziqi.cn/gtgdkruvbl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xingfuxueyuan.xyz/gtrvrejwke.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.kuanghao11.cn/gtrmgygscq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangtech.top/gtqwboquyp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ywan-chungtsiang.top/gtqytlpvkd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.meibo888.top/gtrftxlmjl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydjk.org.cn/gtzaumodin.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gtainffvbi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.bjfxy.top/gtsxrzzyra.html

[P03] 生成短随机字符串
来源：http://hz.316326.xyz/gtsnglawjs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gtqljhptym.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuetiantiany.cn/gtiwnbzdkl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtsevygrfn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtgjrawaho.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtpgylfpth.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuetiantiany.cn/gtmpajxytz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yvedp.cn/gtnzykcsog.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangkeji.top/gtkqyuxezh.html

[P04] 求长度
来源：http://hz.xingfuxueyuan.xyz/gtmgkulwxx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ywan-chungtsiang.top/gtayagoynu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cucudq.cn/gtvbioezuw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtaegzpnkk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtpmlgowgi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ehwqpu.com/gttjkoopqu.html

Go:   len(arr);  len(m)
来源：http://hz.pycfn.com/gtiohzzvfk.html

Ruby: x.length;  x.size
来源：http://hz.meibo888.top/gthncasqwb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.havefunace.top/gtiblmsqqi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hnqzz.top/gtyfwufkdy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xylfe.cn/gtmmwiyiaa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cheryme.top/gtiqlqohag.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.vqdsnc.cn/gtenvmnuqc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtnulejiad.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.kuanghao11.cn/gtaoibmmbx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ywan-chungtsiang.top/gtwejfbahd.html

Ruby: a == b
来源：http://hz.hnqzz.top/gtojclcevr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jianghu66.top/gtfdferhop.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxinkj.top/gtiyyssbkn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuxming.cn/gtqpvycnzs.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtzckhccif.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.birdmap.top/gtbrwotjnk.html

TS:   if (x == null) {}
来源：http://hz.hywenlv.cn/gtwmoynyqh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gtsohqnskv.html

Go:   if x == nil {}
来源：http://hz.smart0.xyz/gtescraitb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtpbmdknky.html

C#:   if (x is null) {}
来源：http://hz.yj20258.top/gthnntjwjb.html

[P07] 防抖与节流
来源：http://hz.hfpthk.cn/gtamqyxhrl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.daria6918.cn/gtsphghqms.html

PHP:  // 手写时间戳比较
来源：http://hz.snrcjt.cn/gtvhzpemci.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtjwobcsjl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtmraiejyd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtldhfboth.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgfzy.top/gtyfqkofpb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gtpxuswcym.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuxming.cn/gtxfnwlnww.html

[P08] 处理浮点精度问题
来源：http://hz.chenzaomai.com/gtohhtjcfb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sweek.top/gtfoqzorbn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daria6918.cn/gtckaxuoxv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhaomingkeji.xyz/gtpworvytc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xziqi.cn/gtsianxlqm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cheryme.top/gtghrukufo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hysaishi.cn/gtmxdyowfg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhongyouzk.top/gttrluyymo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shangyingyoupin.top/gtnvoljaun.html

================================================================================
来源：http://hz.daria6918.cn/gttistlmtg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gthblduktj.html

================================================================================
来源：http://hz.jianghu66.top/gtqxrukacd.html

[Q01] 创建表
来源：http://hz.zhiwuduotai.top/gtrtnbctjj.html

CREATE TABLE users (
来源：http://hz.nanxinkj.top/gtyjjrrnus.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gtjhhhnggz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gttdlpmjee.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dianchejie.cn/gtmxoivzzq.html


<!-- 参考信息 -->