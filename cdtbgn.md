代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cdnleiting.top/gtgwyelkot.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daxiang520.top/gtgaqblxqz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gtigyekjsj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtjjpvrzgz.html

[M04] 获取当前工作目录
来源：http://hz.jlsjyb.cn/gtjxvmqrly.html

Py:   os.getcwd()
来源：http://hz.xziqi.cn/gtlrbslsxt.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gtkokrlizg.html

JS:   process.cwd()
来源：http://hz.fzhhl.top/gtjzyyqbmr.html

TS:   process.cwd()
来源：http://hz.cqqwz.cn/gtrgtbmwko.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenzaomai.com/gtwhhqefdq.html

Go:   os.Getwd()
来源：http://hz.sysykeji.top/gtpdiivnra.html

Ruby: Dir.pwd
来源：http://hz.hfpthk.cn/gtxtskztyd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gthvggqoxi.html

[M05] 设置退出码
来源：http://hz.zhongyouzk.top/gtafezretm.html

Py:   sys.exit(1)
来源：http://hz.gotoacloud.top/gtbhsbtabx.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtkfwvduhb.html

JS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtqzjrzrta.html

TS:   process.exit(1)
来源：http://hz.birdmap.top/gtvqeddpsf.html

Java: System.exit(1)
来源：http://hz.dashuyun.cn/gtrsxbwqug.html

Go:   os.Exit(1)
来源：http://hz.gogol.net.cn/gtdbywyoyi.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtqwqjgsln.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tian-w.cn/gthowjrtyn.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gtkolfmvax.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtajoxznso.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jianghu66.top/gtxppplqve.html

JS:   console.error("err")
来源：http://hz.yvedp.cn/gtqhgrhfvv.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtazqryfrr.html

Java: System.err.println("err")
来源：http://hz.yj20258888.top/gtxnvfgjao.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shzxlz.cn/gtckytocnx.html

Ruby: warn "err"
来源：http://hz.iojbl.cn/gtfaqynldb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnxiangtu.top/gtzzclamlu.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtgmvtyjig.html

Py:   if __name__ == "__main__":
来源：http://hz.fzhhl.top/gtjhffkxve.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtnlrndfng.html

JS:   require.main === module
来源：http://hz.xuanzx.com/gtxuavzabd.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtupqsxjaa.html

Java: public static void main(String[] args)
来源：http://hz.snrcjt.cn/gtkuortbjd.html

Go:   func main()
来源：http://hz.yj20258.top/gtcsfmssur.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ywan-chungtsiang.top/gtwkrfrhek.html

C#:   static void Main(string[] args)
来源：http://hz.shuidangran.top/gtlcckzabd.html

[M08] 获取系统与运行时信息
来源：http://hz.hnqzz.top/gtwyqlftyd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtwbqevhqk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fengsongda.top/gtzofbsait.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gturhrwlva.html

TS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtwtvlibim.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gtfilmgtzw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.vqdsnc.cn/gtprojcqgt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gotoacloud.top/gtvfyozfpe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhijiandao.cn/gtmqmunddd.html

================================================================================
来源：http://hz.svipenyu.cn/gtznkjdqqr.html

N. 数据结构与算法
来源：http://hz.birdmap.top/gtzmzqvuoj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmdncfirk.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxinkj.top/gtgebghpnu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.aibaodan.cn/gthemywyyx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.c1oappe.top/gtziwcmsna.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtdsdzswwz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtjliuxacx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtgojcwkxg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fengsongda.top/gthfetfrpq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtvqnmjdih.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xziqi.cn/gtftensitq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangshuangyany.cn/gtfwlubjxv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guannengcc.top/gtztyikenj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.feifeiyinyue.top/gtxmgpqudg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtltmrxdkd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtvuoapqdz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pycfn.com/gtiusvhbhc.html

Go:   slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtqtgnrbmu.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtijnzkkls.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sxryk.cn/gtmpdwrnsd.html

[N03] 快速排序（分治示例）
来源：http://hz.wangshuangyany.cn/gtntljtyxy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.smart0.xyz/gtcpkkqcsa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtxkcfajse.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtdbufqyts.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtmwrktaga.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtjbfaudyg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhengqikj.top/gtxiwwejim.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydjk.org.cn/gtjfmtckos.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.vqdsnc.cn/gtdcopuepv.html

[N04] 斐波那契数列
来源：http://hz.52xcode.cn/gtisxgqufs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtnvgnnifh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cqqwz.cn/gtgrfzbhgv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtoecfkrox.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtcapyikgj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cdnleiting.top/gtshqieatk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zdqjudy.top/gtcsuuqczb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtfermealn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtcjitjehn.html

[N05] 最大公约数
来源：http://hz.ivvv.top/gtvvntislw.html

Py:   math.gcd(a, b)
来源：http://hz.zhixingplan.top/gtygyckxld.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gtsrlwzucy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtcqnkmvjc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xingfuxueyuan.xyz/gtkynntkfg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.dianchejie.cn/gtgbifhvfa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gotoacloud.top/gtrwtfjddr.html

Ruby: a.gcd(b)
来源：http://hz.tianlin.xyz/gtvtljjwek.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.wangshuangyany.cn/gtxkjdlvpp.html

[N06] 判断回文字符串
来源：http://hz.havefunace.top/gtznsfevkn.html

Py:   s == s[::-1]
来源：http://hz.pycfn.com/gtcfjuaaml.html

PHP:  $s === strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtrgrnbovj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtloasfqgq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtpfnshbzo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtqbbzzkkz.html

Go:   // 双指针从两端比较
来源：http://hz.cucudq.cn/gtptwvaesc.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gtvfqnpdxm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.0kj1m.cn/gtenegupfv.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258888.top/gtqqzlhgtm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shzxlz.cn/gtmhpovrgz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hywenlv.cn/gtdmqfcvzd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jianghu66.top/gtzysqsghw.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtnxzsujmr.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gttbcfcvjd.html

Go:   // 手写 map[int]int
来源：http://hz.haohaochexian.top/gteibtfuye.html

Ruby: // 手写 Hash
来源：http://hz.cqqwz.cn/gtqxajqjjb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sysykeji.top/gtlyjsvimz.html

[N08] 生成全排列
来源：http://hz.fengsongda.top/gtyzjnoaik.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gtggadrxph.html

PHP:  // 手写递归交换
来源：http://hz.hnqzz.top/gtdactfsku.html

JS:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtxlujlilj.html

TS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtgnasvplh.html

Java: // 手写回溯递归
来源：http://hz.ybcxt.top/gtcrwxfudk.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtscliqluz.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtdzsotqkm.html

C#:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtuskcsuwc.html

[N09] 栈与队列
来源：http://hz.zhixingplan.top/gtygwuiagb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.fzhhl.top/gtrbshlpet.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgufenzy.top/gtouwzcgwi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtncbljram.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yanxiufei.cn/gtrbgxsepj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tianlin.xyz/gtlobtnmii.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xingfuxueyuan.xyz/gtlqcszvjs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dianchejie.cn/gtwnnaxiae.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gthtvhmnbc.html

[N10] 链表节点定义
来源：http://hz.dianchejie.cn/gtdgzbenst.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ywan-chungtsiang.top/gtpaarhppw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gtedrhxgvn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shzxlz.cn/gtlssrhvjw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxinkj.top/gtaihncemf.html

Java: class Node { int v; Node next; }
来源：http://hz.shangyingyoupin.top/gtvdmyigdd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gtyzwlecvn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.bjfxy.top/gtihddclnw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.iojbl.cn/gtvnfyoero.html

[N11] 二叉树中序遍历
来源：http://hz.hnxiangtu.top/gtuwjpupdo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ywan-chungtsiang.top/gteukwfyyq.html

PHP:  // 手写递归函数
来源：http://hz.shuidangran.top/gtyrelooxk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nwbrower.top/gtktxjakcz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtbxzwnlmr.html

Java: // 手写递归
来源：http://hz.mhx1999.top/gtlvkunqhz.html

Go:   // 手写递归
来源：http://hz.guowangkeji.top/gticjftpak.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuxming.cn/gtgtxiownm.html

C#:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtztpczygc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jianghu66.top/gtvmqulkud.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fzhhl.top/gtdenyvaju.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydjk.org.cn/gtepskexcv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtnqycgyzp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gtaxcrzpzf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtarsiojmg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gogol.net.cn/gtedkjrujm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xylfe.cn/gtzpxvbpps.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtornvyvlv.html

================================================================================
来源：http://hz.yuanzhike.top/gttsusirtj.html

O. 并发与异步
来源：http://hz.nwbrower.top/gtpyqtjxty.html

================================================================================
来源：http://hz.jinqigufen.top/gtlsdzgnhr.html

[O01] 启动一个线程
来源：http://hz.daria6918.cn/gtmjozzxtm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.andypj.xyz/gtmrxwblwj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jlsjyb.cn/gtffpygwrx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xuetiantiany.cn/gtooxepnfx.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtmqaajywa.html

Java: new Thread(() -> f()).start()
来源：http://hz.yonumen.top/gtcimnqywr.html

Go:   go f()
来源：http://hz.0kj1m.cn/gtdmfsrysw.html

Ruby: Thread.new { f }
来源：http://hz.jyoumei.cn/gtwtntqglu.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtvwvvfujr.html

[O02] 使用线程池
来源：http://hz.zhaomingkeji.xyz/gtidqpxqqb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.dianchejie.cn/gtfpshxduz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aibaodan.cn/gtmdigbgmg.html

JS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtaajkuyjn.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtdvcgnugj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtfzkpkgzr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.9152youxi.cn/gtfijvpefl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxuanxn.top/gtxhunqeep.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.birdmap.top/gtngznnalk.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gtjdwzgcht.html

Py:   with lock: shared += 1
来源：http://hz.redwolf501.top/gtsmwloppo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuxming.cn/gtltyabxcn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gaohongyu789.top/gtdkjjitrs.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gttzxewbrc.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxuanxn.top/gtfkyczpri.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gtwupeuckx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.snrcjt.cn/gtpqyphpyu.html

C#:   lock (gate) { shared++; }
来源：http://hz.sufxvd.cn/gtnqcxsxci.html

[O04] 定义异步函数并等待
来源：http://hz.hfpthk.cn/gtfopgsukk.html

Py:   async def f():⏎    await g()
来源：http://hz.aizwys.cn/gttflutkcg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuxming.cn/gtctoknool.html

JS:   async function f() { await g(); }
来源：http://hz.hywenlv.cn/gtldajpkbl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tianlin.xyz/gtagyrddau.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hfpthk.cn/gtqyfjpygd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gotoacloud.top/gtbzlhqter.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtxsavbtei.html

C#:   async Task F() { await G(); }
来源：http://hz.ppjwa.cn/gtialbnxyp.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuanzx.com/gtsbrvhlxt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinghuilouyu.cn/gtdxzyasxj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ywan-chungtsiang.top/gtxknziijf.html

JS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtnmwpuokf.html

TS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtinhidalx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.meibo888.top/gtmpzeyyas.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sysykeji.top/gtccdjwktq.html

Ruby: threads.map(&:join)
来源：http://hz.smart0.xyz/gtmqicnmry.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jyoumei.cn/gtuokhmkvh.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtkronysfj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtmcafofhd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuxming.cn/gtbpytuydh.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtwnjgtwwk.html

TS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtesmudxcy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xinyue.icu/gtgtpantad.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aizwys.cn/gtrksjldjj.html

Ruby: // fork 块
来源：http://hz.guowangkeji.top/gtajhpkova.html

C#:   Parallel.For
来源：http://hz.xziqi.cn/gtxiqktvfu.html

================================================================================
来源：http://hz.svipenyu.cn/gtyjqqfrea.html

P. 常用工具函数
来源：http://hz.yueranfly.top/gtmcuarhzq.html

================================================================================
来源：http://hz.ehwqpu.com/gtempvdglh.html

[P01] 生成 UUID
来源：http://hz.gaohongyu789.top/gtdhpzfxnm.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gtlxxvjgab.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.c1oappe.top/gtokpwyajn.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gthwpoynja.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtmdjzcciu.html

Java: UUID.randomUUID().toString()
来源：http://hz.daria6918.cn/gtrdwadafs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.vqdsnc.cn/gtzumwfhcl.html

Ruby: SecureRandom.uuid
来源：http://hz.tanke756.top/gtxasqizwb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sysykeji.top/gtitmqmhds.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zdqjudy.top/gtvhkxlfbt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtamacnnms.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cucudq.cn/gtxhjwxtpl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuxming.cn/gtvjdbjhbk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtwpozmzoz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgfzy.top/gtwcjicpex.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tianlin.xyz/gterhqmmxa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinyuanbaomall.cn/gtwlhffzux.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cheryme.top/gtswgzrrwu.html

[P03] 生成短随机字符串
来源：http://hz.52xcode.cn/gtujlgkbzn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pengpengdd.cyou/gtlqochnvz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aizwys.cn/gttbvmicel.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtnfvfktuh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtmyzhhjku.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnxiangtu.top/gtpqyfiajd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daria6918.cn/gttqwfbtye.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gtrqeobvkk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jiagoushi.top/gtqspsvbdp.html

[P04] 求长度
来源：http://hz.xuetiantiany.cn/gtvtkvxiww.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xinyue.icu/gtsxxlbyst.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtnllajmcj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtytgevckn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cdnleiting.top/gtclsejonx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhongyouzk.top/gtguechswe.html

Go:   len(arr);  len(m)
来源：http://hz.zhoulong.xyz/gthctougpo.html

Ruby: x.length;  x.size
来源：http://hz.jinghuilouyu.cn/gtybpjnght.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gogol.net.cn/gtnsqylytr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhixingplan.top/gtctpfkipi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.andypj.xyz/gtnahobwzo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cheryme.top/gtibpbnqcx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxinkj.top/gtwxkkgbpz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtriipspep.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgfzy.top/gtluhubkhy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinghuilouyu.cn/gttcnknoaz.html

Ruby: a == b
来源：http://hz.chenjidiqi.icu/gtfovynsgg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtovuuvios.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sysykeji.top/gtbhkrxjnw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yongpay.top/gtmljalaas.html

PHP:  if (empty($x)) {}
来源：http://hz.9152youxi.cn/gtollcrarq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnxiangtu.top/gtbzujlvxk.html

TS:   if (x == null) {}
来源：http://hz.tian-w.cn/gtuffsakfq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daria6918.cn/gtvtqvmkuq.html

Go:   if x == nil {}
来源：http://hz.cheryme.top/gtqgbfcsop.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shzxlz.cn/gtcxzpefee.html

C#:   if (x is null) {}
来源：http://hz.yj20258888.top/gtlhbtymiy.html

[P07] 防抖与节流
来源：http://hz.zhoulong.xyz/gtzzhrtvrb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aizwys.cn/gtdoohvmdc.html

PHP:  // 手写时间戳比较
来源：http://hz.yonumen.top/gtgvtiofun.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtxsdojpgr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtnyqzehhz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.snrcjt.cn/gtnuxtjrco.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxinkj.top/gtupdbwjlc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gtzpqqdqoh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gaohongyu789.top/gtwhihlhso.html

[P08] 处理浮点精度问题
来源：http://hz.xziqi.cn/gtylqilijy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenlongwang.top/gtbgxobrsn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shangyingyoupin.top/gtkpihgirl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.c1oappe.top/gtwieowfga.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jianghu66.top/gtkknkafzf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tanke756.top/gtcikjuaao.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.smart0.xyz/gtuzcrnaie.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ydzc1.top/gtwxmlrfkm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhaomingkeji.xyz/gtbpesrkrx.html

================================================================================
来源：http://hz.gotoacloud.top/gtahiiljdk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydjk.org.cn/gttwnauotj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbrunaswb.html

[Q01] 创建表
来源：http://hz.vqdsnc.cn/gtkbunkmtx.html

CREATE TABLE users (
来源：http://hz.hysaishi.cn/gtvouyccha.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gtwzifshnb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtbpxzqdbl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jiagoushi.top/gtklultudg.html


<!-- 参考信息 -->