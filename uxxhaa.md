代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.quarkkingdee.top/gtyytcqmtb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuetiantiany.cn/gtcsnxumqb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigfzy.top/gtmphrluze.html

C#:   Process.Start("ls", "-l");
来源：http://hz.quarkkingdee.top/gtqnofkdgb.html

[M04] 获取当前工作目录
来源：http://hz.shangyingyoupin.top/gtwuawyhwr.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtoavmweem.html

PHP:  getcwd();
来源：http://hz.nanxinkj.top/gtmxybeqqe.html

JS:   process.cwd()
来源：http://hz.aizwys.cn/gtmtknstdu.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtvfivpftj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgufenzy.top/gtykjpgxvt.html

Go:   os.Getwd()
来源：http://hz.yanxiufei.cn/gtaahpmdiy.html

Ruby: Dir.pwd
来源：http://hz.yangfankeji.com/gtghbsozgh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.svipenyu.cn/gtoakzahmj.html

[M05] 设置退出码
来源：http://hz.meibo888.top/gtetjnrkpn.html

Py:   sys.exit(1)
来源：http://hz.shangyingyoupin.top/gtrfsjvtuu.html

PHP:  exit(1);
来源：http://hz.tian-w.cn/gtcfotowfd.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtduggpibk.html

TS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtrqsdbzsl.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtbxwklqjp.html

Go:   os.Exit(1)
来源：http://hz.ppjwa.cn/gtecakyghe.html

Ruby: exit 1
来源：http://hz.jlsjyb.cn/gttvetfmqo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cqqwz.cn/gtixgswfkb.html

[M06] 向标准错误输出
来源：http://hz.hnxiangtu.top/gtzfotwczx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtkfnbetmg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.quarkkingdee.top/gtmmcbifgb.html

JS:   console.error("err")
来源：http://hz.redwolf501.top/gtjzmobklz.html

TS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtcwxikbkf.html

Java: System.err.println("err")
来源：http://hz.snrcjt.cn/gtlufvbsjm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydzc1.top/gtjftqlidn.html

Ruby: warn "err"
来源：http://hz.nwbrower.top/gtubdivsio.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.c1oappe.top/gthquwyyij.html

[M07] 判断是否为主入口
来源：http://hz.xuetiantiany.cn/gtrclxlmnu.html

Py:   if __name__ == "__main__":
来源：http://hz.yvedp.cn/gtxzuwhkuz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pycfn.com/gtirttgbns.html

JS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtvqtnczrm.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gttrnbtrjd.html

Java: public static void main(String[] args)
来源：http://hz.jinqigfzy.top/gthhlmrjzm.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtnmpxclgs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jqgufenzy.top/gtzabzpiin.html

C#:   static void Main(string[] args)
来源：http://hz.zhiwuduotai.top/gtslklarsz.html

[M08] 获取系统与运行时信息
来源：http://hz.zhongyouzk.top/gtcbxtyaug.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258888.top/gtgpbpghms.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shanyushiyangkeji.top/gtjngyagkp.html

JS:   process.platform;  process.version
来源：http://hz.fzhhl.top/gtutbrizdw.html

TS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtmmbjbgmw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gaohongyu789.top/gtfcasnsac.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtduqbnmit.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.iojbl.cn/gtdxrouynq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gogol.net.cn/gthwlpbhnw.html

================================================================================
来源：http://hz.shuidangran.top/gtcqvidyks.html

N. 数据结构与算法
来源：http://hz.kuanghao11.cn/gtbakakhrs.html

================================================================================
来源：http://hz.0kj1m.cn/gtqjtkrjus.html

[N01] 二分查找（有序数组）
来源：http://hz.yueranfly.top/gtnedexzaw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangtech.top/gtsjsivonx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aibaodan.cn/gtpmslawva.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtlstyivts.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtbbgsarav.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.haohaochexian.top/gtifyriklr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sysykeji.top/gtzbrxjtdh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.9152youxi.cn/gtclzagxdt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gtzsrnejzl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtralvzbng.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtuwoxfltj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cucudq.cn/gtdwegprqd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtgdhihsdp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gtvcbvcimx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnqzz.top/gtdtvlhbsj.html

Go:   slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtjnctqltd.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtyxvzrjle.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pengpengdd.cyou/gtlzdgrrbw.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtldrskizh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hywenlv.cn/gtsrxswymq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.316326.xyz/gtskcbwwvs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtjwenivvj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtcbutpwxv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jyoumei.cn/gtosrlvvon.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yueranfly.top/gtulywpfyl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gtvzmykzit.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtibkfnpvr.html

[N04] 斐波那契数列
来源：http://hz.andypj.xyz/gtgkatuupv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gthijipdrs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.vqdsnc.cn/gtyxenjxvw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtxboioiti.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtsjsbnhgo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtzvlahodj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.feifeiyinyue.top/gtjmyxmmqp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtnbgwuyhw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.52xcode.cn/gtqkwmuxeu.html

[N05] 最大公约数
来源：http://hz.zhaomingkeji.xyz/gtmtgobhfl.html

Py:   math.gcd(a, b)
来源：http://hz.ppjwa.cn/gtgugdtqwa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtzidchbtc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtinrbqihq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gtrotidzpt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gtgyrdvpos.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuetiantiany.cn/gtoijyqdsz.html

Ruby: a.gcd(b)
来源：http://hz.zhiwuduotai.top/gtmkiunbdg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtliizpemc.html

[N06] 判断回文字符串
来源：http://hz.0kj1m.cn/gtnwqtedmj.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gtduyurxph.html

PHP:  $s === strrev($s);
来源：http://hz.zhixingplan.top/gtwoewzkkg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtpzcdmneg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtoweajpdj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtovzeheba.html

Go:   // 双指针从两端比较
来源：http://hz.xinyue.icu/gtswrsivfn.html

Ruby: s == s.reverse
来源：http://hz.jinqigfzy.top/gtutjcxpjc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtfpvncnyf.html

[N07] 两数之和（返回下标）
来源：http://hz.316326.xyz/gtotmvlfno.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangtech.top/gtpgloabzf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtqgnojado.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.316326.xyz/gtxnlabdqg.html

TS:   // 手写 Map<string, number>
来源：http://hz.ybcxt.top/gtgyrcrkzv.html

Java: // 手写 HashMap
来源：http://hz.xinyue.icu/gtpjpnoqrv.html

Go:   // 手写 map[int]int
来源：http://hz.zhengqikj.top/gttkcjbwig.html

Ruby: // 手写 Hash
来源：http://hz.haohaochexian.top/gtmxiewtuq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pycfn.com/gtnjbhteqx.html

[N08] 生成全排列
来源：http://hz.zycfv.cn/gttlinvbus.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtexqiecby.html

PHP:  // 手写递归交换
来源：http://hz.daria6918.cn/gtqxlyisek.html

JS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtsxvazjsj.html

TS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtvrolcmdv.html

Java: // 手写回溯递归
来源：http://hz.gogol.net.cn/gthvdycmpu.html

Go:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtyalxeftg.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gtwfuzudjp.html

C#:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtsrhfjxwv.html

[N09] 栈与队列
来源：http://hz.smart0.xyz/gtfenzwiyn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xingfuxueyuan.xyz/gtjnnvatdn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guannengcc.top/gtjmkwdozx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yangfankeji.com/gtzticecms.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.0kj1m.cn/gtccwmkvqn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cdnleiting.top/gtvdjcjrfq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dianchejie.cn/gtuvdrbjay.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yueranfly.top/gthjagowrc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yueranfly.top/gtxkugdipu.html

[N10] 链表节点定义
来源：http://hz.ivvv.top/gtqypsfcin.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hysaishi.cn/gtyjhehzzd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shuidangran.top/gtqiuwqora.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gtklxmjfdu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.0kj1m.cn/gtbsyoxwyq.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtklmxektr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtsudsiafq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gaohongyu789.top/gtutomjhqr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yongpay.top/gtyamudkdy.html

[N11] 二叉树中序遍历
来源：http://hz.xingfuxueyuan.xyz/gtaudzdupm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.havefunace.top/gttvqizeag.html

PHP:  // 手写递归函数
来源：http://hz.nanxinkj.top/gtpmvmwqne.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.quarkkingdee.top/gtnqlwpbge.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.mhx1999.top/gtbfjmlndi.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtxbwqteag.html

Go:   // 手写递归
来源：http://hz.zycfv.cn/gtekigiylu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenzaomai.com/gtdwhqqxul.html

C#:   // 手写递归
来源：http://hz.birdmap.top/gtrjsdaesr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yueranfly.top/gtziyvjgag.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gtyjvjeorc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gttlpjyoss.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtbzwuscpi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtdkogblon.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtbjzimitu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.birdmap.top/gtaexryhxh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.meibo888.top/gtmkcdxrio.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtgxuvuxhf.html

================================================================================
来源：http://hz.yj202588.top/gtyiwqcrgr.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gtikugqfth.html

================================================================================
来源：http://hz.jianghu66.top/gtunizjsvy.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtjmunondf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jqgfzy.top/gtajecafxi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tianlin.xyz/gtrxxgodag.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtudrgpfoi.html

TS:   // 同 JS
来源：http://hz.ydjk.org.cn/gtlandrglj.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangshuangyany.cn/gtejfyfvxd.html

Go:   go f()
来源：http://hz.hywenlv.cn/gtyltauhem.html

Ruby: Thread.new { f }
来源：http://hz.jinqigfzy.top/gtkyifoxlx.html

C#:   Task.Run(() => F());
来源：http://hz.zycfv.cn/gtlmzenigu.html

[O02] 使用线程池
来源：http://hz.xingfuxueyuan.xyz/gtmsqlxriy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ywan-chungtsiang.top/gtshzdjrvp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shuidangran.top/gtudrwhsqt.html

JS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtcbmcelep.html

TS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtakbdqseh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.0kj1m.cn/gtmrzcpmrq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ivvv.top/gtlwwnhsnq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gtbmlngelc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.52xcode.cn/gtnfmscovz.html

[O03] 加锁保护共享数据
来源：http://hz.hfpthk.cn/gtdcusbpvu.html

Py:   with lock: shared += 1
来源：http://hz.yuxming.cn/gtqrksiklt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ybcxt.top/gtirkpgbnb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhongyouzk.top/gtxjdanmvs.html

TS:   // 同 JS
来源：http://hz.jqgfzy.top/gtlmihtxhj.html

Java: synchronized (this) { shared++; }
来源：http://hz.birdmap.top/gtwjatbmta.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gtumorpjim.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pycfn.com/gttrfsrttj.html

C#:   lock (gate) { shared++; }
来源：http://hz.gogol.net.cn/gtaumowybd.html

[O04] 定义异步函数并等待
来源：http://hz.pengpengdd.cyou/gtdkbuotvk.html

Py:   async def f():⏎    await g()
来源：http://hz.svipenyu.cn/gtppwbtzvx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jianghu66.top/gtgwenlffd.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gtncotxvay.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.redwolf501.top/gtcbizqbst.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yvedp.cn/gtocynavge.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sysykeji.top/gtcxufpubn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sufxvd.cn/gtviwvhbez.html

C#:   async Task F() { await G(); }
来源：http://hz.yvedp.cn/gtpfkcjhiq.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gtsodfhnur.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yongpay.top/gtqymoumlb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangshuangyany.cn/gtdythnblz.html

JS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtfrqckasn.html

TS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtjdxhzech.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gtjkwroljb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gotoacloud.top/gtyqtfoqtq.html

Ruby: threads.map(&:join)
来源：http://hz.c1oappe.top/gtsheqfuzq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtyplvwaxb.html

[O06] 使用进程池
来源：http://hz.yj20258888.top/gtuehojwvn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtdamilxgk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sweek.top/gtcljrvivx.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtpuvdbajg.html

TS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtxyqbuatb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ehwqpu.com/gtwsoxsagm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinqigufen.top/gtibxkqsti.html

Ruby: // fork 块
来源：http://hz.zhijiandao.cn/gthwptnbog.html

C#:   Parallel.For
来源：http://hz.vqdsnc.cn/gtpwgvuioa.html

================================================================================
来源：http://hz.haohaochexian.top/gtvmyunplj.html

P. 常用工具函数
来源：http://hz.aizwys.cn/gtgpdezydd.html

================================================================================
来源：http://hz.shzxlz.cn/gtxpxwzlek.html

[P01] 生成 UUID
来源：http://hz.gzhubu.top/gthmoogfmf.html

Py:   str(uuid.uuid4())
来源：http://hz.cdnleiting.top/gtglxbzoze.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hnqzz.top/gtkksjfoyu.html

JS:   crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtvcarivbk.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtrqnzrnin.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgufenzy.top/gtsyitfvhj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sxryk.cn/gtzdfxufgj.html

Ruby: SecureRandom.uuid
来源：http://hz.xuetiantiany.cn/gtvyszttoq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.redwolf501.top/gtnzsafnjz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.smart0.xyz/gtuomxbtde.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.iojbl.cn/gtxuluzqkq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinghuilouyu.cn/gtuenpvfnj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxuanxn.top/gtsrwbafsz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hammf.cn/gtugfperga.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shanyushiyangkeji.top/gtuemwjoqd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.bjfxy.top/gtslvdhdoy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yonumen.top/gtkbyysfuc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.iojbl.cn/gtlvqlbkex.html

[P03] 生成短随机字符串
来源：http://hz.xylfe.cn/gteluyphsu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cheryme.top/gtixzcmxbj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuxming.cn/gtvcqeukgr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtbqydgblf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtjbmgwvgd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zdqjudy.top/gtxfhogrxy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.feifeiyinyue.top/gtwqivcvci.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shangyingyoupin.top/gtoxhvdyyp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yongpay.top/gtnezooykm.html

[P04] 求长度
来源：http://hz.gzhubu.top/gtoikmkedd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258.top/gtqpollbea.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtkhfuuoti.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtlityzpfy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtwcrgtjfw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jyoumei.cn/gtnjuoalpj.html

Go:   len(arr);  len(m)
来源：http://hz.xuetiantiany.cn/gtynfbabsc.html

Ruby: x.length;  x.size
来源：http://hz.zhiwuduotai.top/gttsrdtpxl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtkgakucsy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.iojbl.cn/gtvjujzaoa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinqigufen.top/gtuvdmsfrd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuxming.cn/gtrcdiispv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtxhlowxic.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhixingplan.top/gtwitohalp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.svipenyu.cn/gtmumlmcvi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shzxlz.cn/gtctptlars.html

Ruby: a == b
来源：http://hz.hywenlv.cn/gtmtaxxuge.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jianghu66.top/gthbwvlprx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.feifeiyinyue.top/gtdqgdudxp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtjiddwzzj.html

PHP:  if (empty($x)) {}
来源：http://hz.chenjidiqi.icu/gtubsdowzr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yueranfly.top/gtzmkogdto.html

TS:   if (x == null) {}
来源：http://hz.xylfe.cn/gtrnbqgevs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.haohaochexian.top/gtfkiuljkk.html

Go:   if x == nil {}
来源：http://hz.yj20258888.top/gtukniysmd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtztwxdcsp.html

C#:   if (x is null) {}
来源：http://hz.hnqzz.top/gtpmsletoa.html

[P07] 防抖与节流
来源：http://hz.gaohongyu789.top/gtlmoightq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sxryk.cn/gtouymaaka.html

PHP:  // 手写时间戳比较
来源：http://hz.chenlongwang.top/gtgdarrswt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gttofamdut.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtmnhgggex.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.316326.xyz/gtaiaschpi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.bjfxy.top/gtxyveqmqb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dashuyun.cn/gtprehepds.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.havefunace.top/gtmqbfrbyf.html

[P08] 处理浮点精度问题
来源：http://hz.316326.xyz/gtsgbgtrbb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtmeztnkcu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtlajhhdne.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ivvv.top/gtthvkxkxw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydjk.org.cn/gtbwggnwca.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtugdesnug.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gtrofsbfjk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangdashe.top/gtzvgwgmqa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.smart0.xyz/gtozkoqmww.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtkulahzqe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xuetiantiany.cn/gtnipibkyn.html

================================================================================
来源：http://hz.dashuyun.cn/gthgwrenif.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gtwgjzvvyn.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gteeybjist.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtdjmtdjis.html

name VARCHAR(50) NOT NULL,
来源：http://hz.0kj1m.cn/gtplcdteev.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhixingplan.top/gtockthgrl.html


<!-- 参考信息 -->