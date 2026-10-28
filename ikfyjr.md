代发 wailian999

Ruby: ARGV
来源：http://hz.c1oappe.top/gtxtgipclm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenzaomai.com/gtorsipcki.html

[M02] 读取环境变量
来源：http://hz.zhoulong.xyz/gtkexowcbi.html

Py:   os.environ.get("HOME")
来源：http://hz.zhoulong.xyz/gtfrwjbgoc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gtuultwcgl.html

JS:   process.env.HOME
来源：http://hz.fzhhl.top/gtpsguecvh.html

TS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtfpekpcyy.html

Java: System.getenv("HOME")
来源：http://hz.zhoulong.xyz/gtfsiijdoo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shanyushiyangtech.top/gtubhbpzyz.html

Ruby: ENV["HOME"]
来源：http://hz.guowangkeji.top/gtiutlolqs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtdogefmop.html

[M03] 执行外部命令
来源：http://hz.bjfxy.top/gtasulducg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtfapnaajs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinghuilouyu.cn/gtjtkcspup.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtkuzbgzbu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtesyfddwu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuanzhike.top/gttefjwplr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhiwuduotai.top/gtxewzjled.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shangyingyoupin.top/gtcbvijgnc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yongpay.top/gtomwzabqm.html

[M04] 获取当前工作目录
来源：http://hz.kuanghao11.cn/gtnxzcsjmw.html

Py:   os.getcwd()
来源：http://hz.ydzc1.top/gtdbmzdjoo.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtlahpbfns.html

JS:   process.cwd()
来源：http://hz.cqqwz.cn/gtovlftsyx.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtlnkgelpw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtkhrhmoxf.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtatefbugy.html

Ruby: Dir.pwd
来源：http://hz.pycfn.com/gtwrccrlkm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jyoumei.cn/gtknmguplg.html

[M05] 设置退出码
来源：http://hz.bjfxy.top/gtuqugbzqj.html

Py:   sys.exit(1)
来源：http://hz.pengpengdd.cyou/gtjcgeqmyz.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gtidwbryyk.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtrntveieq.html

TS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtjvsllaff.html

Java: System.exit(1)
来源：http://hz.yanxiufei.cn/gtbykyybzl.html

Go:   os.Exit(1)
来源：http://hz.zhoulong.xyz/gtcuhmhqcd.html

Ruby: exit 1
来源：http://hz.sweek.top/gtwkcwpccs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hywenlv.cn/gtgqjhqiit.html

[M06] 向标准错误输出
来源：http://hz.zhoulong.xyz/gtikwbtvlp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtjwwducvb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gtsxbmhqdj.html

JS:   console.error("err")
来源：http://hz.chenzaomai.com/gtlglxnyfs.html

TS:   console.error("err")
来源：http://hz.zhongyouzk.top/gttnmsllym.html

Java: System.err.println("err")
来源：http://hz.quarkkingdee.top/gtfrkelssa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnqzz.top/gtkfnvgsub.html

Ruby: warn "err"
来源：http://hz.gotoacloud.top/gtrycnjslt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.vqdsnc.cn/gttzkdiyya.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gtmdtrkcod.html

Py:   if __name__ == "__main__":
来源：http://hz.gogol.net.cn/gtylhcvcsx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinyuanbaomall.cn/gtgdxidomw.html

JS:   require.main === module
来源：http://hz.yj20258888.top/gtwgsbhfeg.html

TS:   require.main === module
来源：http://hz.ydzc1.top/gthzruxhei.html

Java: public static void main(String[] args)
来源：http://hz.chenjidiqi.icu/gtjbnzhirr.html

Go:   func main()
来源：http://hz.chenlongwang.top/gtfjeqlkop.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.52xcode.cn/gtakrrqbyd.html

C#:   static void Main(string[] args)
来源：http://hz.daria6918.cn/gtzejfnjnv.html

[M08] 获取系统与运行时信息
来源：http://hz.yonumen.top/gtnjbzletv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gtlxzhomjp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxinkj.top/gtnknzjuce.html

JS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gtgrioaxur.html

TS:   process.platform;  process.version
来源：http://hz.wangshuangyany.cn/gtwgeuvrkk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangdashe.top/gtbpajuxve.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtgiciubzv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jlsjyb.cn/gtkmgpmpmg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtzagtmelg.html

================================================================================
来源：http://hz.guannengcc.top/gtyvgchbjj.html

N. 数据结构与算法
来源：http://hz.gotoacloud.top/gtobrwkshy.html

================================================================================
来源：http://hz.ppjwa.cn/gtntjxiilo.html

[N01] 二分查找（有序数组）
来源：http://hz.sweek.top/gtqtjzgnfj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtesenmidl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.kuanghao11.cn/gtbklpswmk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtvjfcmoju.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtqrwezoqa.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtmwsxraew.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.havefunace.top/gtqafyzydc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gtfgcjonyo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtaarrqyju.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gtxuzoumgj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtctjbjsrz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gttmqoeeyu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtwywjcktf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtyraaihsj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jianghu66.top/gtmnlgooqo.html

Go:   slices.Sort(arr)
来源：http://hz.cashguo.top/gtlzusxhmm.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtxltkfrer.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yonumen.top/gtwnrwjcix.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gteknzzqzm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jyoumei.cn/gttaeikdgr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgufenzy.top/gtxlhjmlpb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtrfcfsygc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtggugvovh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhengqikj.top/gtynsezqly.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gtdwcxahdq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gogol.net.cn/gtnszlhuqe.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhijiandao.cn/gtnshoqpxn.html

[N04] 斐波那契数列
来源：http://hz.hfpthk.cn/gtpptvsxoc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtaahsdvxd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhengqikj.top/gtmuelxzvk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtgkzjmrfa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtzeakngcm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtlvhruplc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.guowangkeji.top/gtiskkpkax.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtgjkhswrg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.quarkkingdee.top/gtgkkyrlup.html

[N05] 最大公约数
来源：http://hz.ydjk.org.cn/gtpsqdyfzj.html

Py:   math.gcd(a, b)
来源：http://hz.quarkkingdee.top/gtluhovisl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtjeewjdgz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shuidangran.top/gtupyfqepq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtbbvhzmaj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtqyhijdve.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydjk.org.cn/gtvoqfmomh.html

Ruby: a.gcd(b)
来源：http://hz.nanxuanxn.top/gtttwctwsa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ppjwa.cn/gtqwkionmz.html

[N06] 判断回文字符串
来源：http://hz.zdqjudy.top/gtpflbebmx.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtvuomsifo.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtlvrnbsrq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtumqakyoy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtpnmsesdz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dianchejie.cn/gtsniruzxl.html

Go:   // 双指针从两端比较
来源：http://hz.shanyushiyangtech.top/gtxdrqalaf.html

Ruby: s == s.reverse
来源：http://hz.c1oappe.top/gtmmfemtwv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gttokitmpz.html

[N07] 两数之和（返回下标）
来源：http://hz.sysykeji.top/gtsscpbtwy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhixingplan.top/gtnmgwafhq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gtxgeemkoj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tian-w.cn/gtsjsqxplo.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgfzy.top/gtlcrbhzsh.html

Java: // 手写 HashMap
来源：http://hz.zhoulong.xyz/gtlccxxljj.html

Go:   // 手写 map[int]int
来源：http://hz.gotoacloud.top/gtpqcqwrmy.html

Ruby: // 手写 Hash
来源：http://hz.jinghuilouyu.cn/gtdbgcvohi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.kuanghao11.cn/gtmidhpowy.html

[N08] 生成全排列
来源：http://hz.andypj.xyz/gtkntqsvmh.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gttpecyjvx.html

PHP:  // 手写递归交换
来源：http://hz.meibo888.top/gtxfgzbhyh.html

JS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtbwiivsfs.html

TS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gthwxdibxl.html

Java: // 手写回溯递归
来源：http://hz.ppjwa.cn/gtqeiumbvo.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtiqcrnfzl.html

Ruby: arr.permutation.to_a
来源：http://hz.fengsongda.top/gtlmutvcuf.html

C#:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtqsddhtsb.html

[N09] 栈与队列
来源：http://hz.hywenlv.cn/gtfdftcsqv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yvedp.cn/gtbreneoys.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shangyingyoupin.top/gthdjflhmm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shuidangran.top/gtkrohlmtg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hfpthk.cn/gtuayjkacr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtwrebelye.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhiwuduotai.top/gtosbndczg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gtyxbfooia.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuxming.cn/gtexvwietp.html

[N10] 链表节点定义
来源：http://hz.sweek.top/gtepkokewx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgfzy.top/gtpvqfjqnx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ybcxt.top/gtgwygcjxk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gtzhebxszr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sysykeji.top/gttvfmwdew.html

Java: class Node { int v; Node next; }
来源：http://hz.jiagoushi.top/gtcerhpifw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daxiang520.top/gteyieskam.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gtszlckqxo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj202588.top/gtrtbrivki.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtunsecgij.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.feifeiyinyue.top/gtijymkryy.html

PHP:  // 手写递归函数
来源：http://hz.aizwys.cn/gtlvcuivgo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtvelmnlbv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.mhx1999.top/gtuikkvsoz.html

Java: // 手写递归
来源：http://hz.cashguo.top/gtvtcpupzj.html

Go:   // 手写递归
来源：http://hz.sufxvd.cn/gtbesvcfdi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.dashuyun.cn/gtlakzwhuu.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtqkgkypuq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xziqi.cn/gtyuymbtbx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxuanxn.top/gthftiglcz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fengsongda.top/gtebjehqwa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtcimfriwe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtvzdfnobp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cqqwz.cn/gtqsuxbyba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gtrxrutatb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gthzhgbhkb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtsegswruz.html

================================================================================
来源：http://hz.ybcxt.top/gtvuxjiyuw.html

O. 并发与异步
来源：http://hz.fengsongda.top/gthjwkeljm.html

================================================================================
来源：http://hz.snrcjt.cn/gtxjoshnje.html

[O01] 启动一个线程
来源：http://hz.sxryk.cn/gttygmzncn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtmjtfpped.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj202588.top/gtafwxubtw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhengqikj.top/gtnbboamig.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gthioznerp.html

Java: new Thread(() -> f()).start()
来源：http://hz.xingfuxueyuan.xyz/gtqyuvghhq.html

Go:   go f()
来源：http://hz.snrcjt.cn/gtoxtaifgu.html

Ruby: Thread.new { f }
来源：http://hz.chenlongwang.top/gtsuhtwbet.html

C#:   Task.Run(() => F());
来源：http://hz.chenjidiqi.icu/gtvpbcwhrp.html

[O02] 使用线程池
来源：http://hz.chenjidiqi.icu/gtfaroaste.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hywenlv.cn/gtfzbsxojc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhiwuduotai.top/gtwkaypbul.html

JS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gteujvahub.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtlghdfjgx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.andypj.xyz/gtuhqihcdu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jlsjyb.cn/gtqmccbfmz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258888.top/gtnbooaayw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtergnmlvu.html

[O03] 加锁保护共享数据
来源：http://hz.fzhhl.top/gtavjjnhuj.html

Py:   with lock: shared += 1
来源：http://hz.quarkkingdee.top/gtthsycqih.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhaomingkeji.xyz/gtochjmney.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtjyucmlsp.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtafqjemnx.html

Java: synchronized (this) { shared++; }
来源：http://hz.yvedp.cn/gtahmuduib.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jyoumei.cn/gtebwqypcz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenlongwang.top/gtwqibovaz.html

C#:   lock (gate) { shared++; }
来源：http://hz.gogol.net.cn/gtywuvnslj.html

[O04] 定义异步函数并等待
来源：http://hz.jyoumei.cn/gtohuwrfxr.html

Py:   async def f():⏎    await g()
来源：http://hz.jiagoushi.top/gtqjqxvwds.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yueranfly.top/gtelgyadix.html

JS:   async function f() { await g(); }
来源：http://hz.dianchejie.cn/gtoywnexkl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fengsongda.top/gtegltyvxf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hammf.cn/gtiexdkpgn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aibaodan.cn/gtwaufqtph.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinghuilouyu.cn/gtiriyywgp.html

C#:   async Task F() { await G(); }
来源：http://hz.xingfuxueyuan.xyz/gtqrgvyrgb.html

[O05] 并发执行并等待全部完成
来源：http://hz.dianchejie.cn/gtqsfkqnly.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gtskcillxg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sysykeji.top/gtjzvbfnlq.html

JS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtutuvinxf.html

TS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtbixjnqmf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinghuilouyu.cn/gtobwdpkgn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gtzvihjfja.html

Ruby: threads.map(&:join)
来源：http://hz.nanxinkj.top/gtrrzyquqg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhiwuduotai.top/gtzirgjfkq.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtfonkdrfe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yuxming.cn/gthywwainj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.iojbl.cn/gthzupygwv.html

JS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gtcsdquhot.html

TS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtrdoushop.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.52xcode.cn/gtyrcvsvzc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.mhx1999.top/gthlbzpvqe.html

Ruby: // fork 块
来源：http://hz.ppjwa.cn/gtuojjydjt.html

C#:   Parallel.For
来源：http://hz.nanxinkj.top/gtlfljbjny.html

================================================================================
来源：http://hz.daxiang520.top/gtrktufxbj.html

P. 常用工具函数
来源：http://hz.xylfe.cn/gtkqltusim.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfrzbkmrm.html

[P01] 生成 UUID
来源：http://hz.chenjidiqi.icu/gtxtldqicd.html

Py:   str(uuid.uuid4())
来源：http://hz.xuanzx.com/gtyiohcjlp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.vqdsnc.cn/gthxljquet.html

JS:   crypto.randomUUID()
来源：http://hz.iojbl.cn/gtuyypjhwg.html

TS:   crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtriztnocx.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtolltisxp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xingfuxueyuan.xyz/gtgleonvek.html

Ruby: SecureRandom.uuid
来源：http://hz.fengsongda.top/gttzaijquj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.kuanghao11.cn/gtgmdfqexz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.feifeiyinyue.top/gthrnshnlc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ywan-chungtsiang.top/gtlrwbfkuc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.316326.xyz/gthbrrayqy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhaomingkeji.xyz/gtiaatphyp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gtgijgcsdr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuanzx.com/gtydgymbtf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gotoacloud.top/gtyfboipqp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tian-w.cn/gtamqchhuv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sxryk.cn/gtbzbyldxh.html

[P03] 生成短随机字符串
来源：http://hz.yangfankeji.com/gtfezkudqx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jlsjyb.cn/gtpibcrang.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tanke756.top/gtastlnnvs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtwkjripap.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtwfgfudbl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gaohongyu789.top/gtcpqorwbu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yongpay.top/gtnyenqpan.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gthqlhmutk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtwqhjziib.html

[P04] 求长度
来源：http://hz.smart0.xyz/gtxdgxghcu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhijiandao.cn/gteupaekrh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtuihltjij.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtlwjqsouw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtgnuxquvg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.feifeiyinyue.top/gtqlcvmtlb.html

Go:   len(arr);  len(m)
来源：http://hz.redwolf501.top/gtcberflgl.html

Ruby: x.length;  x.size
来源：http://hz.shzxlz.cn/gtivdeflik.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxuanxn.top/gtanhrlvea.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hfpthk.cn/gtukcodelt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtalkyfxnl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangkeji.top/gtafhmydpf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gaohongyu789.top/gtkieeafau.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtwziswzlk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gogol.net.cn/gtgjxqldwe.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenzaomai.com/gtwlmdgqfw.html

Ruby: a == b
来源：http://hz.yj202588.top/gtcbxzklda.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigufen.top/gtpwgaipoc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cucudq.cn/gtjvpqqlfi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangdashe.top/gtfqwpykii.html

PHP:  if (empty($x)) {}
来源：http://hz.havefunace.top/gtrifskzbk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jyoumei.cn/gtuiqxygoa.html

TS:   if (x == null) {}
来源：http://hz.mhx1999.top/gtdgfpxlzf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gteoomwrct.html

Go:   if x == nil {}
来源：http://hz.chenzaomai.com/gtrfunpenv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fengsongda.top/gtfmsptohj.html

C#:   if (x is null) {}
来源：http://hz.birdmap.top/gtwmwihupm.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtaevipqim.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnqzz.top/gtldmzdfdi.html

PHP:  // 手写时间戳比较
来源：http://hz.52xcode.cn/gtmcytfulm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtnitaacup.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtdixphqok.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhongyouzk.top/gtyviqebul.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ehwqpu.com/gtlhsdfraq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nanxuanxn.top/gtujebvcya.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigfzy.top/gtqadxyesn.html

[P08] 处理浮点精度问题
来源：http://hz.zhiwuduotai.top/gtflecndny.html


<!-- 参考信息 -->