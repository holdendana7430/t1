代发 wailian999

================================================================================
来源：http://hz.52xcode.cn/gtztbpmndv.html

[M01] 读取命令行参数
来源：http://hz.yuxming.cn/gtzapjmzzs.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gtojefjtht.html

PHP:  $argv;  $argc;
来源：http://hz.pengpengdd.cyou/gttdjshwur.html

JS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtzeeurdau.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtuuqocnyd.html

Java: args 数组（main 方法参数）
来源：http://hz.wangdashe.top/gtwtsrhgzb.html

Go:   os.Args[1:]
来源：http://hz.cashguo.top/gtvvavdbwe.html

Ruby: ARGV
来源：http://hz.yvedp.cn/gtacrsaryh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zycfv.cn/gtcmsxkgmz.html

[M02] 读取环境变量
来源：http://hz.zhixingplan.top/gtobiybxra.html

Py:   os.environ.get("HOME")
来源：http://hz.pengpengdd.cyou/gtupifokgk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.snrcjt.cn/gtwupxcxjq.html

JS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtaosxlmlc.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gtwhegagxw.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gtrxlsucpu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.quarkkingdee.top/gtaxjojdxd.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtbrjfmqzy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtxbchbyay.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtatwvddgb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtrivhoxix.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sweek.top/gtnolvnenq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtgvntvgur.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtwelfdggf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.quarkkingdee.top/gtzzvtlyvs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtfomwzkde.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenlongwang.top/gtmczfvpam.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtfzowtaio.html

[M04] 获取当前工作目录
来源：http://hz.meibo888.top/gtritxdpwe.html

Py:   os.getcwd()
来源：http://hz.hongshengwenyu.top/gtvrbvjpft.html

PHP:  getcwd();
来源：http://hz.redwolf501.top/gtnoihbmlj.html

JS:   process.cwd()
来源：http://hz.dianchejie.cn/gtfmrdbtls.html

TS:   process.cwd()
来源：http://hz.yuxming.cn/gtqrkqemdw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.iojbl.cn/gtbydsudmj.html

Go:   os.Getwd()
来源：http://hz.pycfn.com/gtkbdvticp.html

Ruby: Dir.pwd
来源：http://hz.52xcode.cn/gthtdsfhiq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.wangshuangyany.cn/gtlqjlwdvg.html

[M05] 设置退出码
来源：http://hz.gotoacloud.top/gtpjvrliof.html

Py:   sys.exit(1)
来源：http://hz.316326.xyz/gttayzmvrv.html

PHP:  exit(1);
来源：http://hz.xuetiantiany.cn/gtkdtbgrdx.html

JS:   process.exit(1)
来源：http://hz.bjfxy.top/gtkbrdoulv.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gtrsopwugl.html

Java: System.exit(1)
来源：http://hz.316326.xyz/gtcrzhbigv.html

Go:   os.Exit(1)
来源：http://hz.xylfe.cn/gthlsksdqx.html

Ruby: exit 1
来源：http://hz.tianlin.xyz/gtdjeqbkxe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtdfavlofq.html

[M06] 向标准错误输出
来源：http://hz.ywan-chungtsiang.top/gthshallwr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydjk.org.cn/gtccukyxnr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuanzhike.top/gtvcuwchga.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtqnvxbnqf.html

TS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtwqhhundk.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtrwnidfxb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtrplniiyf.html

Ruby: warn "err"
来源：http://hz.redwolf501.top/gtoupbdrnd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yvedp.cn/gtyissftml.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtvlatilae.html

Py:   if __name__ == "__main__":
来源：http://hz.gaohongyu789.top/gtecrrcxcx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jiagoushi.top/gtooxeeedq.html

JS:   require.main === module
来源：http://hz.svipenyu.cn/gtmxsyupvd.html

TS:   require.main === module
来源：http://hz.ehwqpu.com/gtkdgjjags.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gtaaunritb.html

Go:   func main()
来源：http://hz.gzhubu.top/gtnbvrdice.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtmsqzsvzb.html

C#:   static void Main(string[] args)
来源：http://hz.c1oappe.top/gthvxnonma.html

[M08] 获取系统与运行时信息
来源：http://hz.jinghuilouyu.cn/gtctldeoes.html

Py:   platform.system();  platform.python_version()
来源：http://hz.birdmap.top/gtykaonaff.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gzhubu.top/gtwrhxrtvm.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtjxtkaoyc.html

TS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gtjsrqjbgp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtrevwtzor.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gtzenzmicq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yueranfly.top/gtxsknzlzg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tian-w.cn/gtrplcwppa.html

================================================================================
来源：http://hz.yonumen.top/gtqtklolnp.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtuqjtyzop.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtxvsnxids.html

[N01] 二分查找（有序数组）
来源：http://hz.sxryk.cn/gtnjmwfjmk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cucudq.cn/gtqehcsmpa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tian-w.cn/gtikwqhtdu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtqszonhjm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtxhdvxnuo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtraehdumx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zycfv.cn/gtphfbpuxc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.andypj.xyz/gtvywipeqf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gttwzgvrqo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.meibo888.top/gtvueiuzlz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtwdigprfp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hysaishi.cn/gtjliuwwrf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtvbkoiwdu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtzboozhkh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhixingplan.top/gtjsqrvsre.html

Go:   slices.Sort(arr)
来源：http://hz.ydzc1.top/gttvvrwdlr.html

Ruby: arr.sort
来源：http://hz.yanxiufei.cn/gtvsnyezzy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.kuanghao11.cn/gtwyjzulon.html

[N03] 快速排序（分治示例）
来源：http://hz.kuanghao11.cn/gtkksahjct.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aibaodan.cn/gtcavyoxgs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daria6918.cn/gtinxcqrrt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.kuanghao11.cn/gtrplgtlan.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtetvgnmop.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhengqikj.top/gtpfehzrad.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.feifeiyinyue.top/gtkjkslwxi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guannengcc.top/gthiixbzuj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yonumen.top/gthmpvyokl.html

[N04] 斐波那契数列
来源：http://hz.jqgufenzy.top/gtwmspgdsd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtdamgyqnw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sysykeji.top/gtdvwagnjl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtiwrnjdoc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtwlnjuknr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtymtffztz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtewqdopth.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtujxspfin.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gthybubsfw.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gtgdvwekxe.html

Py:   math.gcd(a, b)
来源：http://hz.bjfxy.top/gttnxuncxm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ehwqpu.com/gtkcrrkzff.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtkvigryhg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtlygzjxhh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.0kj1m.cn/gtjlahohsx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangkeji.top/gtzhsekkse.html

Ruby: a.gcd(b)
来源：http://hz.zhongyouzk.top/gttpjxxgnb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinghuilouyu.cn/gtcpbqjtuz.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtvkazypsb.html

Py:   s == s[::-1]
来源：http://hz.tian-w.cn/gtrrqwclcf.html

PHP:  $s === strrev($s);
来源：http://hz.yvedp.cn/gteeukcqcv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtxgtjwxzv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtahawohgn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuanzx.com/gtueywmpby.html

Go:   // 双指针从两端比较
来源：http://hz.ydzc1.top/gthellwreh.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gttlufknag.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtlhnilqgh.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gtuphfisdq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.meibo888.top/gtlijyribi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinghuilouyu.cn/gteldafvbm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuanzx.com/gtbycyhgmq.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhijiandao.cn/gtefpeuyck.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gthhhfhqhu.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gtoftsnrci.html

Ruby: // 手写 Hash
来源：http://hz.ehwqpu.com/gtpwgthyap.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuanzhike.top/gtibfvneuk.html

[N08] 生成全排列
来源：http://hz.andypj.xyz/gtzznljrbw.html

Py:   itertools.permutations(arr)
来源：http://hz.chenlongwang.top/gtburyghmo.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtlgkdkeej.html

JS:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtziryebsk.html

TS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtnhctsorq.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtfbwyhsgw.html

Go:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtyxgpzpsr.html

Ruby: arr.permutation.to_a
来源：http://hz.xziqi.cn/gtocpqemgd.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gteqnvjwba.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gtwoublcfl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhaomingkeji.xyz/gtzwrspddx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xinyue.icu/gtzvonlzlr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.iojbl.cn/gthlzzaupc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gotoacloud.top/gtlqoaulpw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ehwqpu.com/gtqbxkfflh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.haohaochexian.top/gtxgrmrhlz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtujtgujhn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtagwmghkn.html

[N10] 链表节点定义
来源：http://hz.9152youxi.cn/gtqecfmnhp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gtdcymjotg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hysaishi.cn/gtpkexqguz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhijiandao.cn/gtmglzfyfv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ppjwa.cn/gthflgyicn.html

Java: class Node { int v; Node next; }
来源：http://hz.shangyingyoupin.top/gtjpexeqbk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.52xcode.cn/gtxelwiubf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.mhx1999.top/gtullgzaup.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtcikglxqb.html

[N11] 二叉树中序遍历
来源：http://hz.nanxinkj.top/gtaqbnbqra.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnxiangtu.top/gtkwowjjvh.html

PHP:  // 手写递归函数
来源：http://hz.jiagoushi.top/gtixxmunxc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xinyue.icu/gtqkxtvktj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtergknxmt.html

Java: // 手写递归
来源：http://hz.chenjidiqi.icu/gttiuzjwcg.html

Go:   // 手写递归
来源：http://hz.gaohongyu789.top/gtcxxowsnw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhoulong.xyz/gtogqrxrud.html

C#:   // 手写递归
来源：http://hz.redwolf501.top/gtpcgnkwdi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hammf.cn/gtzzifproh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtgcsitoaj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.kuanghao11.cn/gtwkreazfg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenzaomai.com/gtqdgazvzz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtutnmtcte.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtybkurfuq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtgnsyrdsr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.316326.xyz/gtikktlkjz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jlsjyb.cn/gtzvzytwhp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjpkgewtk.html

O. 并发与异步
来源：http://hz.zhijiandao.cn/gteirnscrq.html

================================================================================
来源：http://hz.iojbl.cn/gtbiojjzwt.html

[O01] 启动一个线程
来源：http://hz.zycfv.cn/gtxyuxvnvo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hywenlv.cn/gtwyvtzgfp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cheryme.top/gtyvvumxjj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jyoumei.cn/gtqmyagkcf.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtgjisldav.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuanzhike.top/gtzmlzlagp.html

Go:   go f()
来源：http://hz.gotoacloud.top/gteoalltwy.html

Ruby: Thread.new { f }
来源：http://hz.nwbrower.top/gtvpbwhotn.html

C#:   Task.Run(() => F());
来源：http://hz.meibo888.top/gtzprehuck.html

[O02] 使用线程池
来源：http://hz.pycfn.com/gtgsubusdu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ivvv.top/gtovfhztsk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sxryk.cn/gtudxkbquj.html

JS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gteichrguh.html

TS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtkzvabguf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangshuangyany.cn/gtkibbhvkp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hongshengwenyu.top/gtjphegysc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tian-w.cn/gtpnkmjicp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuxming.cn/gtihwtpime.html

[O03] 加锁保护共享数据
来源：http://hz.jyoumei.cn/gttlhzdouo.html

Py:   with lock: shared += 1
来源：http://hz.haohaochexian.top/gtqbyyfzyq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.316326.xyz/gtywdwgudn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ydzc1.top/gtgakaxptt.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtsjuuxlbv.html

Java: synchronized (this) { shared++; }
来源：http://hz.jlsjyb.cn/gtlcjflcna.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtwactvjye.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gtsmzvjvmd.html

C#:   lock (gate) { shared++; }
来源：http://hz.feifeiyinyue.top/gthccnfxrv.html

[O04] 定义异步函数并等待
来源：http://hz.feifeiyinyue.top/gtfvemgnqd.html

Py:   async def f():⏎    await g()
来源：http://hz.cashguo.top/gtwosxowcl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtxpyfpzba.html

JS:   async function f() { await g(); }
来源：http://hz.tianlin.xyz/gtbgbsydvq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtqqivqhak.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yvedp.cn/gthrgmbokk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aibaodan.cn/gtxymavefk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xinyue.icu/gtzwzrwrqp.html

C#:   async Task F() { await G(); }
来源：http://hz.chenzaomai.com/gtjzqhkvpb.html

[O05] 并发执行并等待全部完成
来源：http://hz.jiagoushi.top/gtncxreiyo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhiwuduotai.top/gtzouhdfza.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ppjwa.cn/gtxusfdzeb.html

JS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtozonrpaw.html

TS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtcwzopgme.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuxming.cn/gtygwfeloz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tian-w.cn/gtdnrruhvm.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtqngrgrwh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yangfankeji.com/gtmovrbcyk.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtudsgpnrd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.snrcjt.cn/gtpwthwisl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtvtgrbluh.html

JS:   // child_process / cluster 模块
来源：http://hz.ehwqpu.com/gtrdjvceee.html

TS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtxvefwrlc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guowangkeji.top/gtziulblqa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xziqi.cn/gtyqykwztx.html

Ruby: // fork 块
来源：http://hz.zhixingplan.top/gtugsdwqpe.html

C#:   Parallel.For
来源：http://hz.hammf.cn/gtrsvvroic.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjchyzlyu.html

P. 常用工具函数
来源：http://hz.vqdsnc.cn/gtpuznrqke.html

================================================================================
来源：http://hz.jinqigufen.top/gtkwlqxeot.html

[P01] 生成 UUID
来源：http://hz.iojbl.cn/gtoirxaajm.html

Py:   str(uuid.uuid4())
来源：http://hz.cucudq.cn/gtuqfmrvpc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gzhubu.top/gtxhtvluum.html

JS:   crypto.randomUUID()
来源：http://hz.iojbl.cn/gtqkadhlus.html

TS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtzglunxny.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gteqyzhgsy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gtblskyfrr.html

Ruby: SecureRandom.uuid
来源：http://hz.yj202588.top/gtqlrojzxq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.quarkkingdee.top/gtgiouyanq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hongshengwenyu.top/gtmdjlyvgm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.dianchejie.cn/gtuxjvtweo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.andypj.xyz/gtjrbaotyn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhaomingkeji.xyz/gtkoizucnp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cdnleiting.top/gtqejtzwne.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuetiantiany.cn/gtubqlabph.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuanzx.com/gtavawlkct.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ydzc1.top/gtjalqjeny.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnxiangtu.top/gtsdujsgfg.html

[P03] 生成短随机字符串
来源：http://hz.cdnleiting.top/gtewiczxna.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yvedp.cn/gtesllhpon.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hysaishi.cn/gtqxbnuzgq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhaomingkeji.xyz/gtbcuzvnci.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.c1oappe.top/gttztzensw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.52xcode.cn/gtkuhatpmj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuetiantiany.cn/gtiihkyozv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.vqdsnc.cn/gtwfswgqpx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.feifeiyinyue.top/gtiryqveoc.html

[P04] 求长度
来源：http://hz.yonumen.top/gtlunxqnxu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtgeqitxzu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtujdbkjkf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gtyhlvilhs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuetiantiany.cn/gtsnkqlrqx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aizwys.cn/gtbmhochaz.html

Go:   len(arr);  len(m)
来源：http://hz.svipenyu.cn/gtzurfpatu.html

Ruby: x.length;  x.size
来源：http://hz.svipenyu.cn/gtngqfpoqb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sysykeji.top/gtrpzmzejh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fzhhl.top/gtyasaesty.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.pycfn.com/gtkxuzlzhj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ppjwa.cn/gtgogtgilf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gtcccdnjqg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.redwolf501.top/gtjevptpxc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fzhhl.top/gtvnskivso.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.iojbl.cn/gtkvwkozcn.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtcrmftqua.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuetiantiany.cn/gtdkkbavuz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cucudq.cn/gtjnljstsg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guannengcc.top/gtljnskmfj.html

PHP:  if (empty($x)) {}
来源：http://hz.shzxlz.cn/gtllnrekmt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daria6918.cn/gtgsscfbcb.html

TS:   if (x == null) {}
来源：http://hz.jqgufenzy.top/gtyiponrtw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xinyue.icu/gtqwphjqrj.html

Go:   if x == nil {}
来源：http://hz.guannengcc.top/gtyjszddjo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cheryme.top/gtldidslae.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gtugpevjof.html

[P07] 防抖与节流
来源：http://hz.yj20258888.top/gtkjdhjpbh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtejzehoij.html


<!-- 参考信息 -->