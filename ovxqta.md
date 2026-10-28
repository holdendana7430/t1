代发 wailian999

Ruby: ARGV
来源：http://hz.shangyingyoupin.top/gtanifoiwz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtrttvqkcx.html

[M02] 读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtpkydasol.html

Py:   os.environ.get("HOME")
来源：http://hz.yangfankeji.com/gtoualecrv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gtifjdtfcg.html

JS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtufuefcxo.html

TS:   process.env.HOME
来源：http://hz.sysykeji.top/gtmnavkquw.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtvholhzan.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenzaomai.com/gtvodycsvo.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtfnfdrviw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tian-w.cn/gtetlmktbb.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtysjtdssd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gogol.net.cn/gtzrzevgqd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.316326.xyz/gtdhzywaxi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtypvxyidd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cucudq.cn/gtjnjlyuuv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jiagoushi.top/gtiyfkzmmv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hnqzz.top/gtfbupglhp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydzc1.top/gtbcshjtgn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sufxvd.cn/gtvaixikgk.html

[M04] 获取当前工作目录
来源：http://hz.hfpthk.cn/gtztxwvkvk.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gtffaeeavo.html

PHP:  getcwd();
来源：http://hz.xingfuxueyuan.xyz/gttyuwhldu.html

JS:   process.cwd()
来源：http://hz.yj20258.top/gtaycmeukj.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtsfsowddm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gtvhbigscx.html

Go:   os.Getwd()
来源：http://hz.vqdsnc.cn/gthrpuqpbl.html

Ruby: Dir.pwd
来源：http://hz.ydjk.org.cn/gtkxkfbybg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.bjfxy.top/gtykijcpai.html

[M05] 设置退出码
来源：http://hz.zhengqikj.top/gtdbrhmfyx.html

Py:   sys.exit(1)
来源：http://hz.yanxiufei.cn/gtvcedikxp.html

PHP:  exit(1);
来源：http://hz.tanke756.top/gtqglmjtte.html

JS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtmhdyfbkc.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtnxpghuoq.html

Java: System.exit(1)
来源：http://hz.hongshengwenyu.top/gtdpoyusun.html

Go:   os.Exit(1)
来源：http://hz.yvedp.cn/gtloqebxbg.html

Ruby: exit 1
来源：http://hz.tian-w.cn/gtqrmoasip.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.mhx1999.top/gtlqybghnk.html

[M06] 向标准错误输出
来源：http://hz.smart0.xyz/gtkecyssuc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtmwvntgpf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daxiang520.top/gtsxudizzm.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtnwvmbupr.html

TS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtpmmoxxxt.html

Java: System.err.println("err")
来源：http://hz.zhoulong.xyz/gtmuiiviix.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gttbdxqshc.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtjdatkcli.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenjidiqi.icu/gtyizsmbvt.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gtcqzymuls.html

Py:   if __name__ == "__main__":
来源：http://hz.cqqwz.cn/gttpjuwuxb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgufenzy.top/gtgffvdybx.html

JS:   require.main === module
来源：http://hz.mhx1999.top/gtcbfxlhvg.html

TS:   require.main === module
来源：http://hz.xuanzx.com/gtwkwyksqq.html

Java: public static void main(String[] args)
来源：http://hz.wangshuangyany.cn/gtcgirbqsz.html

Go:   func main()
来源：http://hz.jiagoushi.top/gtpbihgscf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ehwqpu.com/gtcpanplow.html

C#:   static void Main(string[] args)
来源：http://hz.jqgufenzy.top/gtfxvuopvj.html

[M08] 获取系统与运行时信息
来源：http://hz.havefunace.top/gtrqdqjklo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zycfv.cn/gtygaxuuog.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hysaishi.cn/gtmcioexvb.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtilftuiht.html

TS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtoonvuxtq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gttnwecjih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.mhx1999.top/gtenxwvyww.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shangyingyoupin.top/gthyaaogen.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yvedp.cn/gtqmkfrsze.html

================================================================================
来源：http://hz.sxryk.cn/gtbzrbfwsq.html

N. 数据结构与算法
来源：http://hz.zdqjudy.top/gtfsfsknch.html

================================================================================
来源：http://hz.yueranfly.top/gtrtmmiros.html

[N01] 二分查找（有序数组）
来源：http://hz.jinyuanbaomall.cn/gtefpdadwk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jiagoushi.top/gtjegvmvtp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gtbrjovmtn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtebyuzbhf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtafiywhfe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhixingplan.top/gthypdygtc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hongshengwenyu.top/gtinvxvzvj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.birdmap.top/gthoovmsjl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtwwzvbdof.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.meibo888.top/gtnqksrjrf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtvupdffub.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gthuudawwp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtgbpragkz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtdhxusmff.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daria6918.cn/gtzrnticxa.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtmngyedet.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtjmrzsgda.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuanzhike.top/gtehibckyb.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtmlkosdaj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtlyezblju.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shuidangran.top/gtdmwezntb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtecubjqnj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fzhhl.top/gtlnqohjal.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nwbrower.top/gtrustmzxr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuxming.cn/gtmmawspsq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.kuanghao11.cn/gtpqxpwyro.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sxryk.cn/gtqxlolcal.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtdzdhxpee.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtclnvrnzd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtwmiffaxz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtwtouqtgk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.quarkkingdee.top/gtdaivyogf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtoevuclkp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhaomingkeji.xyz/gtlmjkgqfy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtqpmsjulr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtahhpavbi.html

[N05] 最大公约数
来源：http://hz.ybcxt.top/gtzfdbcfda.html

Py:   math.gcd(a, b)
来源：http://hz.c1oappe.top/gtbefkkjxx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jqgufenzy.top/gtyvjlsvko.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtlsdegaff.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gtelvwdlwz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.meibo888.top/gtisqbrndp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhixingplan.top/gtyxljpqzn.html

Ruby: a.gcd(b)
来源：http://hz.jinqigfzy.top/gtwfygzmqb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hnqzz.top/gtumllutsx.html

[N06] 判断回文字符串
来源：http://hz.zycfv.cn/gtnrfsfkvu.html

Py:   s == s[::-1]
来源：http://hz.sxryk.cn/gtacymgzwu.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtjhtzpufb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtvqoidhbe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yongpay.top/gtvtbeocfq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cashguo.top/gtxlbnmzsg.html

Go:   // 双指针从两端比较
来源：http://hz.shuidangran.top/gtzxznzavm.html

Ruby: s == s.reverse
来源：http://hz.gotoacloud.top/gttpmkygeq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtatuexchk.html

[N07] 两数之和（返回下标）
来源：http://hz.cheryme.top/gtuhjragaj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuetiantiany.cn/gtxmktewgb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj202588.top/gtlhzpcfut.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.feifeiyinyue.top/gttnryavxo.html

TS:   // 手写 Map<string, number>
来源：http://hz.yongpay.top/gthygikmeq.html

Java: // 手写 HashMap
来源：http://hz.c1oappe.top/gtvuamsmmh.html

Go:   // 手写 map[int]int
来源：http://hz.jqgfzy.top/gtznjreanl.html

Ruby: // 手写 Hash
来源：http://hz.nwbrower.top/gtnuvplqya.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtxsgwjgmc.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtasuuizbe.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtgkcoeeon.html

PHP:  // 手写递归交换
来源：http://hz.xingfuxueyuan.xyz/gtnvznvfit.html

JS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtlczgurpp.html

TS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtleppzzwo.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtxgjhpsra.html

Go:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtiluxhlqu.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtotcvfaqx.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gttogfbuuq.html

[N09] 栈与队列
来源：http://hz.yuxming.cn/gtdgjtcydg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jyoumei.cn/gtynrfjhgv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnxiangtu.top/gtvasokrhn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aizwys.cn/gtjslroeit.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.andypj.xyz/gtkwuvqpda.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dianchejie.cn/gtrldctxnx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gteenupeku.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yongpay.top/gtnozmgeov.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jianghu66.top/gtmqzlthqx.html

[N10] 链表节点定义
来源：http://hz.yj20258888.top/gtzcyuliuw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtbzmtrqqa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gtwofyycfp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sweek.top/gtmtxlumal.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.snrcjt.cn/gtkivtizol.html

Java: class Node { int v; Node next; }
来源：http://hz.yueranfly.top/gtsxogctag.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhiwuduotai.top/gtqczgewhk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yongpay.top/gtuhrwuyud.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sxryk.cn/gtumedbytb.html

[N11] 二叉树中序遍历
来源：http://hz.0kj1m.cn/gtcvlnfevd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jlsjyb.cn/gthvjidpvk.html

PHP:  // 手写递归函数
来源：http://hz.yanxiufei.cn/gtgomjpphz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtqznlkpvw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yueranfly.top/gtkbeqalcp.html

Java: // 手写递归
来源：http://hz.xuetiantiany.cn/gtetrlxbpm.html

Go:   // 手写递归
来源：http://hz.pycfn.com/gtqhltmjwn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.havefunace.top/gtoqqgvhvf.html

C#:   // 手写递归
来源：http://hz.chenjidiqi.icu/gtlkvcmryx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtbkqqnrgi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenzaomai.com/gtaurpodjo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuxming.cn/gtludlyowb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtftwuwzwe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.mhx1999.top/gtjdjkxwev.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daxiang520.top/gtvlqsnfbx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yanxiufei.cn/gtdkyhnyss.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangkeji.top/gtmoxiuyfp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtylldiaev.html

================================================================================
来源：http://hz.hnqzz.top/gtxopgmhny.html

O. 并发与异步
来源：http://hz.andypj.xyz/gtwlndkrhz.html

================================================================================
来源：http://hz.cucudq.cn/gtoqanitop.html

[O01] 启动一个线程
来源：http://hz.ydjk.org.cn/gtyjilqmgk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ivvv.top/gtfnwecehl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.feifeiyinyue.top/gtcoiklhcw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gttfdsfbbb.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtiiptfcgo.html

Java: new Thread(() -> f()).start()
来源：http://hz.meibo888.top/gtqbrwsfld.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gtmynkudzz.html

Ruby: Thread.new { f }
来源：http://hz.yj20258.top/gtsdtwjuet.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtrinuotlp.html

[O02] 使用线程池
来源：http://hz.quarkkingdee.top/gtrylddfzy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.meibo888.top/gtinfpvcum.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pycfn.com/gtvzcomayd.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gtgltzqfym.html

TS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtfrzoorvi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.haohaochexian.top/gtrzcsohos.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtysgjsdue.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gtjjswkxjs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtbwsciqet.html

[O03] 加锁保护共享数据
来源：http://hz.guannengcc.top/gtxtblrwzf.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gtkebmcbfl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinyuanbaomall.cn/gttuutnjty.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.snrcjt.cn/gtbtnwuvlh.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtfbupspfk.html

Java: synchronized (this) { shared++; }
来源：http://hz.andypj.xyz/gtvccopwyl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jianghu66.top/gthppfbhfa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yongpay.top/gtumdllnhr.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenjidiqi.icu/gtwphtvnsc.html

[O04] 定义异步函数并等待
来源：http://hz.hfpthk.cn/gtgftqjton.html

Py:   async def f():⏎    await g()
来源：http://hz.gogol.net.cn/gtgmemrxsa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuxming.cn/gtsupkuknv.html

JS:   async function f() { await g(); }
来源：http://hz.chenlongwang.top/gtboswqehn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.0kj1m.cn/gtyhqmymcv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhijiandao.cn/gtduxnbhqe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xinyue.icu/gtwvcofsjm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhaomingkeji.xyz/gtqqgjwkch.html

C#:   async Task F() { await G(); }
来源：http://hz.zdqjudy.top/gtezrwagqr.html

[O05] 并发执行并等待全部完成
来源：http://hz.pengpengdd.cyou/gtmcaolhma.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aizwys.cn/gtlrzihgaj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cucudq.cn/gtfdltofsc.html

JS:   await Promise.all(tasks)
来源：http://hz.andypj.xyz/gtdqfemlyb.html

TS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtwcaoswdu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cdnleiting.top/gtizztptpp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.wangdashe.top/gtamgezrwt.html

Ruby: threads.map(&:join)
来源：http://hz.zhiwuduotai.top/gtvfxkczgy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cdnleiting.top/gtwpoahxbw.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gtzxelxsun.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guowangkeji.top/gtjjsohigd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cucudq.cn/gtlguyfmnx.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gteixnpilv.html

TS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gtdaesrrul.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.mhx1999.top/gtymyqzryp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gotoacloud.top/gtlnjcrieu.html

Ruby: // fork 块
来源：http://hz.yj202588.top/gtkgivdvap.html

C#:   Parallel.For
来源：http://hz.jiagoushi.top/gtfqemloji.html

================================================================================
来源：http://hz.pycfn.com/gtbovmkrnp.html

P. 常用工具函数
来源：http://hz.sysykeji.top/gtpkqzjrtf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gteortrurc.html

[P01] 生成 UUID
来源：http://hz.hammf.cn/gtdwebqojz.html

Py:   str(uuid.uuid4())
来源：http://hz.yvedp.cn/gtxpucspol.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtojzwqusq.html

JS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtxpdezkjn.html

TS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gtlxkvqayv.html

Java: UUID.randomUUID().toString()
来源：http://hz.xziqi.cn/gtfbjxgdkg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtcvfcqrel.html

Ruby: SecureRandom.uuid
来源：http://hz.chenzaomai.com/gtevdzndth.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jlsjyb.cn/gtesnfhvvi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gtukyixkvd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.snrcjt.cn/gtbladggrb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guowangkeji.top/gtsucfazaz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.vqdsnc.cn/gtdvtrgmyd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.bjfxy.top/gtrfaaoxco.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tian-w.cn/gtfjgbnwwb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gtxgnqmcit.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gtwvyfnoci.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenjidiqi.icu/gtqqnwlnle.html

[P03] 生成短随机字符串
来源：http://hz.yongpay.top/gttvsvmlyh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangdashe.top/gtcqwmjyvc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hywenlv.cn/gthedfnzxh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtndorvfpe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtawlsycba.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.daxiang520.top/gtszzhthqa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aibaodan.cn/gtdtkmhetb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xziqi.cn/gtsovpzhgz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.c1oappe.top/gtjdvcelbm.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtgeotqupt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhoulong.xyz/gtwoeqiebp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtrcvisays.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtkmcchoep.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.haohaochexian.top/gtiinissfs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gzhubu.top/gtbdurazed.html

Go:   len(arr);  len(m)
来源：http://hz.jlsjyb.cn/gtjrumtujm.html

Ruby: x.length;  x.size
来源：http://hz.iojbl.cn/gtnqvknxkg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zycfv.cn/gtbilezsxk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hywenlv.cn/gtwhccllsa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xziqi.cn/gtescjsesm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtfkdgpfav.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuanzx.com/gtradoefjp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtotpjeokh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fzhhl.top/gtpnbnkeva.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shzxlz.cn/gtmvmptcjy.html

Ruby: a == b
来源：http://hz.nanxuanxn.top/gtuukazjhs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yueranfly.top/gtfqhpzhaq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gtrcsciyxw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnqzz.top/gtqnbezpnx.html

PHP:  if (empty($x)) {}
来源：http://hz.yanxiufei.cn/gtfqwehwpi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydjk.org.cn/gthosbghpz.html

TS:   if (x == null) {}
来源：http://hz.zhengqikj.top/gtajpntpnu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtzyezavll.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtknepngkl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yongpay.top/gtblomzvwr.html

C#:   if (x is null) {}
来源：http://hz.nanxinkj.top/gtatphxeca.html

[P07] 防抖与节流
来源：http://hz.zhongyouzk.top/gtkzixvbem.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtwfgutorp.html

PHP:  // 手写时间戳比较
来源：http://hz.zhengqikj.top/gtjxccnvcr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ppjwa.cn/gtyrzxqvpi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtwvfszvan.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuanzhike.top/gtopolihml.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtpsprzauz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.vqdsnc.cn/gtpkubynrc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ydzc1.top/gtclpfwyni.html

[P08] 处理浮点精度问题
来源：http://hz.havefunace.top/gtvnlqisar.html


<!-- 参考信息 -->