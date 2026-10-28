代发 wailian999

================================================================================
来源：http://hz.birdmap.top/gtzzkdqzfj.html

[M01] 读取命令行参数
来源：http://hz.ppjwa.cn/gttjxfirwu.html

Py:   sys.argv[1:]
来源：http://hz.shzxlz.cn/gtsxfqlxpu.html

PHP:  $argv;  $argc;
来源：http://hz.hnqzz.top/gtuqrthebn.html

JS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtjljksgwq.html

TS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtzaefpqqu.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtzvcwfgud.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtlounhtvl.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtbzddtnmt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.feifeiyinyue.top/gtcyuogeak.html

[M02] 读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtweqrakbx.html

Py:   os.environ.get("HOME")
来源：http://hz.gogol.net.cn/gtccpxzlhb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtcwncaicx.html

JS:   process.env.HOME
来源：http://hz.316326.xyz/gtckjtirao.html

TS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtcssvvwlz.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangtech.top/gtcgocciww.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yonumen.top/gtsxyyvirf.html

Ruby: ENV["HOME"]
来源：http://hz.wangshuangyany.cn/gtotfujymj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gterlrdxuc.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gtmgajvdtp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tian-w.cn/gtmjgxybkc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yongpay.top/gtxplvgkyz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtlaedvhfz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtzxudyalg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fzhhl.top/gtqrhxmhcd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtxxxzopwv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangdashe.top/gtnjvrlpum.html

C#:   Process.Start("ls", "-l");
来源：http://hz.c1oappe.top/gtiftmxrkd.html

[M04] 获取当前工作目录
来源：http://hz.chenzaomai.com/gtnlezzoqi.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtfffulvbu.html

PHP:  getcwd();
来源：http://hz.yvedp.cn/gtgvbokxpv.html

JS:   process.cwd()
来源：http://hz.guowangkeji.top/gtmadzuqfw.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtctwjsgpu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gogol.net.cn/gtvnmzrxpb.html

Go:   os.Getwd()
来源：http://hz.yueranfly.top/gteqtsvgni.html

Ruby: Dir.pwd
来源：http://hz.havefunace.top/gtwxmkecgt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cheryme.top/gtkncwntkl.html

[M05] 设置退出码
来源：http://hz.jinyuanbaomall.cn/gtfifcsjbu.html

Py:   sys.exit(1)
来源：http://hz.smart0.xyz/gtoiaztajf.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtnxuyplex.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtsmalxlap.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gteigvnayp.html

Java: System.exit(1)
来源：http://hz.chenjidiqi.icu/gtyglbukbq.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangtech.top/gtbevsvgnv.html

Ruby: exit 1
来源：http://hz.daxiang520.top/gtzkpomooy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258888.top/gtpzoebckf.html

[M06] 向标准错误输出
来源：http://hz.sufxvd.cn/gtnrfpmhwh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gthprmhbte.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgufenzy.top/gtsyqybalr.html

JS:   console.error("err")
来源：http://hz.jiagoushi.top/gtxdqzbjzt.html

TS:   console.error("err")
来源：http://hz.yueranfly.top/gtgtvsfbxh.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtrcawywid.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xylfe.cn/gtaovmghqi.html

Ruby: warn "err"
来源：http://hz.meibo888.top/gthhbvatnt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jyoumei.cn/gtvpubomjw.html

[M07] 判断是否为主入口
来源：http://hz.yj20258888.top/gtntenoqex.html

Py:   if __name__ == "__main__":
来源：http://hz.yanxiufei.cn/gtrhyilkmc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtdkkqfoer.html

JS:   require.main === module
来源：http://hz.meibo888.top/gttotpukfy.html

TS:   require.main === module
来源：http://hz.hfpthk.cn/gtzshnrlpx.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtlxtmzvaq.html

Go:   func main()
来源：http://hz.mhx1999.top/gtoknirfvt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shzxlz.cn/gtylqmtbfm.html

C#:   static void Main(string[] args)
来源：http://hz.sxryk.cn/gtbzblcbhz.html

[M08] 获取系统与运行时信息
来源：http://hz.52xcode.cn/gteidovbmu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yongpay.top/gtidegsxxf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.guannengcc.top/gtlhrhqoia.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtyenogppj.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtmljcafgo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ppjwa.cn/gtgfdypgvk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pycfn.com/gtdvmikyfh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigfzy.top/gtjzpcqpfj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cdnleiting.top/gtepaqpffy.html

================================================================================
来源：http://hz.gaohongyu789.top/gtzhwkivog.html

N. 数据结构与算法
来源：http://hz.sweek.top/gtqyesgglj.html

================================================================================
来源：http://hz.hfpthk.cn/gtqhiciprh.html

[N01] 二分查找（有序数组）
来源：http://hz.andypj.xyz/gtjwmqnpwz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tanke756.top/gtfoioljwz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnxiangtu.top/gtyvijsjto.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtnlhmvryb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtowddpmau.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtqowfhwbv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hammf.cn/gtexlywjgr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.vqdsnc.cn/gtmjnufhpr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.c1oappe.top/gtspnfspkf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yvedp.cn/gtzvgwjrvy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hongshengwenyu.top/gtkgmdpqts.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinyuanbaomall.cn/gtziminthd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gthumvajhd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtczqwmclx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.snrcjt.cn/gtmsobffgc.html

Go:   slices.Sort(arr)
来源：http://hz.nwbrower.top/gtcfhgvejx.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtwdphgmks.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtnlxbtdca.html

[N03] 快速排序（分治示例）
来源：http://hz.gogol.net.cn/gtyuwsvkxy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hammf.cn/gtxaxfmnar.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtpajvnwnm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangkeji.top/gtczmpwqyt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtelmirqpm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.havefunace.top/gthctnwcad.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gtjeovpzlp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtzvkesvrv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gtdynrgpes.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtvrawbipi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtxpxgorlx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj20258888.top/gtclqbrxnf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtfzalkgpb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtjuianosv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtemmrjqvc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.fengsongda.top/gtyzujtris.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtzizkikpe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gtulhxkvic.html

[N05] 最大公约数
来源：http://hz.tian-w.cn/gtjdzmkkel.html

Py:   math.gcd(a, b)
来源：http://hz.birdmap.top/gtnizdiqnq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yvedp.cn/gtvezzogev.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtdolcxcbv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtrtgoxpma.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigufen.top/gtxfkqlfvg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sufxvd.cn/gtykamyrop.html

Ruby: a.gcd(b)
来源：http://hz.yj20258888.top/gtzarlwcbx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.0kj1m.cn/gthmkidfah.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gthipfaksp.html

Py:   s == s[::-1]
来源：http://hz.shuidangran.top/gtwjhhlpad.html

PHP:  $s === strrev($s);
来源：http://hz.cheryme.top/gtrtidaegz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtlwtwakgt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtacrbdduc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xingfuxueyuan.xyz/gtkuspjyhw.html

Go:   // 双指针从两端比较
来源：http://hz.guannengcc.top/gtabruyqwy.html

Ruby: s == s.reverse
来源：http://hz.chenzaomai.com/gtwjkgowaj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtjnxnfoid.html

[N07] 两数之和（返回下标）
来源：http://hz.jinghuilouyu.cn/gtorlyospd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xziqi.cn/gtpywaozwm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tianlin.xyz/gtdbffdakd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fengsongda.top/gtjquamrrj.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtuoniuqfu.html

Java: // 手写 HashMap
来源：http://hz.quarkkingdee.top/gtmkzkyxuv.html

Go:   // 手写 map[int]int
来源：http://hz.birdmap.top/gtnmztirhx.html

Ruby: // 手写 Hash
来源：http://hz.zhoulong.xyz/gteyehyyfa.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.9152youxi.cn/gtkvdwlygh.html

[N08] 生成全排列
来源：http://hz.xuanzx.com/gttaawrdzm.html

Py:   itertools.permutations(arr)
来源：http://hz.chenlongwang.top/gtkrpkuwbl.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtgfxoqjgk.html

JS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtcsgbmwma.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtsylpmztb.html

Java: // 手写回溯递归
来源：http://hz.fengsongda.top/gtheitlldt.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtvtvzpzui.html

Ruby: arr.permutation.to_a
来源：http://hz.mhx1999.top/gtlmwzsmbl.html

C#:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtnrsnnwut.html

[N09] 栈与队列
来源：http://hz.smart0.xyz/gtysqnmfeo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tanke756.top/gtsceryskm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dashuyun.cn/gtwmmgtnzu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigufen.top/gtdhszukql.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yangfankeji.com/gtsaetfbss.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.andypj.xyz/gtdgjkfstu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nwbrower.top/gtjzdjhyhs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.svipenyu.cn/gtlujfxdcz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yueranfly.top/gtbdrgnmlh.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtwhbhapjc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gotoacloud.top/gtxxysfgao.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.kuanghao11.cn/gtswkoxlho.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.smart0.xyz/gttkonvwwp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.smart0.xyz/gtbnmfbmhs.html

Java: class Node { int v; Node next; }
来源：http://hz.mhx1999.top/gtavmovqwk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gzhubu.top/gteioxveoa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.316326.xyz/gthtrecrro.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.redwolf501.top/gttxfpetfw.html

[N11] 二叉树中序遍历
来源：http://hz.smart0.xyz/gtacyodive.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.bjfxy.top/gtbtkhjbvg.html

PHP:  // 手写递归函数
来源：http://hz.redwolf501.top/gtctegdfhc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtnrzrgolp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtkhmlyuep.html

Java: // 手写递归
来源：http://hz.xziqi.cn/gtuauxsztz.html

Go:   // 手写递归
来源：http://hz.dashuyun.cn/gtvnyrnhnv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daxiang520.top/gtlewfyesh.html

C#:   // 手写递归
来源：http://hz.mhx1999.top/gtnsnbqunf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hammf.cn/gtlqsqviek.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhengqikj.top/gtgganblfj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cheryme.top/gtkfpduzqf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.quarkkingdee.top/gtrvrmmpar.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gttrxpdddz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtwwtpzkhl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.52xcode.cn/gtwqeykuek.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhiwuduotai.top/gtpvrvawmp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtzjpztoio.html

================================================================================
来源：http://hz.bjfxy.top/gtpownkcoh.html

O. 并发与异步
来源：http://hz.yongpay.top/gtjmcmptna.html

================================================================================
来源：http://hz.ydzc1.top/gtqhrhheub.html

[O01] 启动一个线程
来源：http://hz.xinyue.icu/gtvwxpjpkm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtgriorawd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.kuanghao11.cn/gtciaheuun.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shuidangran.top/gtgvemhabh.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gtqyeaqdgi.html

Java: new Thread(() -> f()).start()
来源：http://hz.shangyingyoupin.top/gtzykdqznh.html

Go:   go f()
来源：http://hz.sufxvd.cn/gtpjdkgljs.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtcydfgusr.html

C#:   Task.Run(() => F());
来源：http://hz.yonumen.top/gthtnlfifd.html

[O02] 使用线程池
来源：http://hz.yangfankeji.com/gtdaebnlac.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuanzx.com/gtzfmulior.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gtzkphsfvs.html

JS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtwcvyiccy.html

TS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gttwcobgmr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuanzhike.top/gtzbksmrzx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nwbrower.top/gtsrbnzzmj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yangfankeji.com/gthbpbmjph.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.haohaochexian.top/gtnvlftjxr.html

[O03] 加锁保护共享数据
来源：http://hz.bjfxy.top/gtzpoeeiel.html

Py:   with lock: shared += 1
来源：http://hz.sufxvd.cn/gtddenlgvi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gtugsmvezj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.c1oappe.top/gtpispwyzg.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gthbjbgmct.html

Java: synchronized (this) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtxflglhlc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhongyouzk.top/gttuiqafpq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtkptvvtcj.html

C#:   lock (gate) { shared++; }
来源：http://hz.cdnleiting.top/gtwulfkdne.html

[O04] 定义异步函数并等待
来源：http://hz.ybcxt.top/gtlrgiawuy.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gthslghbzb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shuidangran.top/gtcnehrvxm.html

JS:   async function f() { await g(); }
来源：http://hz.xingfuxueyuan.xyz/gtdifxgjmj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtvmicczov.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hywenlv.cn/gtrxbimznd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.vqdsnc.cn/gtppqxnwgp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nwbrower.top/gtcvmjfzue.html

C#:   async Task F() { await G(); }
来源：http://hz.fzhhl.top/gtekafzlgx.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuxming.cn/gtwflawtiv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhongyouzk.top/gtjvingetn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.mhx1999.top/gthzuglrmq.html

JS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtyqzgtrbs.html

TS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtwvhxxiqy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangtech.top/gtpfmxlobw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuetiantiany.cn/gtudjdrfrz.html

Ruby: threads.map(&:join)
来源：http://hz.redwolf501.top/gtzapaarmd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gtayoydpde.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtubdtcoiz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gotoacloud.top/gteosublvz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fengsongda.top/gtggigymio.html

JS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtiakpjtza.html

TS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtfercmkqh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xinyue.icu/gtiukywzem.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gogol.net.cn/gtzoddbnpo.html

Ruby: // fork 块
来源：http://hz.xylfe.cn/gtwwkzffim.html

C#:   Parallel.For
来源：http://hz.andypj.xyz/gtmpodtmei.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzyfrnews.html

P. 常用工具函数
来源：http://hz.jinqigufen.top/gtcxrwibln.html

================================================================================
来源：http://hz.tianlin.xyz/gtpmuxmmwm.html

[P01] 生成 UUID
来源：http://hz.xuanzx.com/gtpcpjsywp.html

Py:   str(uuid.uuid4())
来源：http://hz.yj202588.top/gtjwvzqfrf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigufen.top/gtzoikhmou.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtsipcwixj.html

TS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtakryqpkl.html

Java: UUID.randomUUID().toString()
来源：http://hz.meibo888.top/gtrrhubhhz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangtech.top/gtwumamcwc.html

Ruby: SecureRandom.uuid
来源：http://hz.cashguo.top/gtjlxzmuau.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtmuqgpsmf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtdphwytcg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuanzx.com/gtmjuaerpr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tianlin.xyz/gtzjhsuyfm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.vqdsnc.cn/gtaesezmjj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtgfxwpcsf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dashuyun.cn/gtlxkjnlbp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangdashe.top/gtrcuppbhf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gthopetlnx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gtnfvjzveu.html

[P03] 生成短随机字符串
来源：http://hz.sweek.top/gtmmfafyup.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuanzx.com/gtwykdbjdt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnqzz.top/gtdbqaexfi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtjkzhodol.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtpkrytgku.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtvcphidgp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gtjcbazzfa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yonumen.top/gtibtpweec.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yueranfly.top/gtpumzgjzb.html

[P04] 求长度
来源：http://hz.nanxuanxn.top/gtscjgrzdx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cqqwz.cn/gtfsnguphv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtuuqpmzce.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtsxqmrfsn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtwktywxmt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dianchejie.cn/gttxrkuwzb.html

Go:   len(arr);  len(m)
来源：http://hz.snrcjt.cn/gtkkssrcyi.html

Ruby: x.length;  x.size
来源：http://hz.tian-w.cn/gtljxyuxmw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shzxlz.cn/gtwmdvgudc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhijiandao.cn/gtjihbealp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuanzx.com/gtcnnqafrt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fengsongda.top/gtoxvjekpe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gtzkdtmyau.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenzaomai.com/gtcsnalpcv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.aizwys.cn/gtyerhqfbp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xziqi.cn/gttabknxcg.html

Ruby: a == b
来源：http://hz.guowangkeji.top/gtcuuxpudn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.kuanghao11.cn/gtgyiqnolh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sysykeji.top/gtecqebpot.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxuanxn.top/gtrtqmtvtb.html

PHP:  if (empty($x)) {}
来源：http://hz.chenlongwang.top/gtfhlouctv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhijiandao.cn/gteotilpca.html

TS:   if (x == null) {}
来源：http://hz.yvedp.cn/gtkjjpeuer.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zycfv.cn/gtnssubbla.html

Go:   if x == nil {}
来源：http://hz.dianchejie.cn/gtgpdhrfta.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ybcxt.top/gtcwboffjp.html

C#:   if (x is null) {}
来源：http://hz.yuxming.cn/gtrmojwnbb.html

[P07] 防抖与节流
来源：http://hz.shuidangran.top/gtosgcnbjf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinyuanbaomall.cn/gtyegucrlb.html


<!-- 参考信息 -->