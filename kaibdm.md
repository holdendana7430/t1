代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtkggbeole.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtfjdbleaj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.haohaochexian.top/gtbkbwamds.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gtdxdehsvc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gteqiaewpa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pengpengdd.cyou/gtrvvsceuy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfqmyfvxp.html

M. 命令行 / 进程 / 环境
来源：http://hz.xingfuxueyuan.xyz/gtymgtnqwq.html

================================================================================
来源：http://hz.yueranfly.top/gtozuuudrl.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtzvhacbuq.html

Py:   sys.argv[1:]
来源：http://hz.chenjidiqi.icu/gtarfrtbcv.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258.top/gtihvgkqqi.html

JS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gtgmjiqodk.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtifwmtjag.html

Java: args 数组（main 方法参数）
来源：http://hz.xuetiantiany.cn/gtqyvujozp.html

Go:   os.Args[1:]
来源：http://hz.zycfv.cn/gtcwrwdbbr.html

Ruby: ARGV
来源：http://hz.zhengqikj.top/gtkacthoge.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxuanxn.top/gtkccyexxb.html

[M02] 读取环境变量
来源：http://hz.svipenyu.cn/gtlmqidklm.html

Py:   os.environ.get("HOME")
来源：http://hz.9152youxi.cn/gtfgziwyni.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtqyknrpky.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gttfybmama.html

TS:   process.env.HOME
来源：http://hz.fzhhl.top/gtxnywkqyo.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtrhwidyat.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aibaodan.cn/gtrpnhohcg.html

Ruby: ENV["HOME"]
来源：http://hz.0kj1m.cn/gtkyorkgwb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hysaishi.cn/gtcedbbelb.html

[M03] 执行外部命令
来源：http://hz.316326.xyz/gtplsutcwg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hfpthk.cn/gtpuacslpm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.bjfxy.top/gtngourste.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtkoxtnzyf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtclyruhlo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtwmlweyzt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj20258888.top/gtfzccmgpa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtilelqgfp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenzaomai.com/gtbbuvbxom.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtpppymmbl.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtyywnujam.html

PHP:  getcwd();
来源：http://hz.jinyuanbaomall.cn/gtkwpsbdja.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtbnfpyxak.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gtyyrnvfds.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtjxyppeaa.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtfdjgkqsg.html

Ruby: Dir.pwd
来源：http://hz.jinqigufen.top/gtpthlzdcc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtarhomxps.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtsegpmhjc.html

Py:   sys.exit(1)
来源：http://hz.cqqwz.cn/gtespurqdw.html

PHP:  exit(1);
来源：http://hz.pycfn.com/gtkrcmggxt.html

JS:   process.exit(1)
来源：http://hz.tian-w.cn/gtlxxbdhwr.html

TS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtpmibhnrt.html

Java: System.exit(1)
来源：http://hz.jqgfzy.top/gtfgyvijsw.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtjgignvhf.html

Ruby: exit 1
来源：http://hz.cqqwz.cn/gtumxchbox.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxuanxn.top/gteyvsubfa.html

[M06] 向标准错误输出
来源：http://hz.zhaomingkeji.xyz/gtkkklwwno.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtrpvhcaeo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gtyopqionx.html

JS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtlxgymeav.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtqdazgtxn.html

Java: System.err.println("err")
来源：http://hz.zhixingplan.top/gtdxxtnjnl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fengsongda.top/gtyxfmazau.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtogkfgqde.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtkkxfyluu.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gtkajjdwmh.html

Py:   if __name__ == "__main__":
来源：http://hz.yanxiufei.cn/gtncegqdol.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.havefunace.top/gtwjeffydz.html

JS:   require.main === module
来源：http://hz.cqqwz.cn/gtcvrhedyl.html

TS:   require.main === module
来源：http://hz.sweek.top/gtzgfmzmgf.html

Java: public static void main(String[] args)
来源：http://hz.xuetiantiany.cn/gtrolmebfn.html

Go:   func main()
来源：http://hz.meibo888.top/gtexwemwba.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hongshengwenyu.top/gtvzofpoyo.html

C#:   static void Main(string[] args)
来源：http://hz.guowangkeji.top/gtztoxydiy.html

[M08] 获取系统与运行时信息
来源：http://hz.c1oappe.top/gtwyizhatd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtiqrkvxax.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shzxlz.cn/gtvltfotix.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtlnfxtdsw.html

TS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtseherldu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenjidiqi.icu/gtyxapnfce.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gtbeqsmuhn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cdnleiting.top/gtrntzrljl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.feifeiyinyue.top/gtqtybrlry.html

================================================================================
来源：http://hz.cdnleiting.top/gtivflxflg.html

N. 数据结构与算法
来源：http://hz.cashguo.top/gtgtaswfjm.html

================================================================================
来源：http://hz.tian-w.cn/gtirhaesua.html

[N01] 二分查找（有序数组）
来源：http://hz.dashuyun.cn/gtbshwpqdp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.feifeiyinyue.top/gthjlaregu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhiwuduotai.top/gtpsvluuaw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtqjpuckdu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtncyndgky.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtlklkjyhd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxinkj.top/gtnwytgnnz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sxryk.cn/gtxcbwuqst.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtrvkzmszp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gogol.net.cn/gtzlbvhzih.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtmejcbdsj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtjdqkjuqf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gttofyrdlw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtmiuqgzjy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jyoumei.cn/gtvxahtklj.html

Go:   slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gttouonodn.html

Ruby: arr.sort
来源：http://hz.dashuyun.cn/gtauxsocav.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sweek.top/gtnjpwsqak.html

[N03] 快速排序（分治示例）
来源：http://hz.shzxlz.cn/gtzuiermoy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ehwqpu.com/gtymtqoefi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhijiandao.cn/gthyrqiwrx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtwpwjireq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtddyhlrtp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtrglaixmy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.vqdsnc.cn/gtmyogppmc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.c1oappe.top/gturmlqubp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hongshengwenyu.top/gtcxgoolaq.html

[N04] 斐波那契数列
来源：http://hz.yongpay.top/gtpdefkfwr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtxfepminc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.iojbl.cn/gttyzgbmsk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtxpzaailq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtcgwtuioo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.daxiang520.top/gtdkuwelqg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hnqzz.top/gtwuhsofpb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtdwwknbki.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gtrqecjhka.html

[N05] 最大公约数
来源：http://hz.chenlongwang.top/gtltgxcofn.html

Py:   math.gcd(a, b)
来源：http://hz.chenjidiqi.icu/gtaifybahd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cqqwz.cn/gtoqqozlog.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jlsjyb.cn/gtzyojdgsq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtnotbzeoe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hfpthk.cn/gtizjnsjpb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zdqjudy.top/gtqecnnayo.html

Ruby: a.gcd(b)
来源：http://hz.zhoulong.xyz/gtqbusvyot.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinghuilouyu.cn/gtobrnqvlu.html

[N06] 判断回文字符串
来源：http://hz.yongpay.top/gtduibrtlt.html

Py:   s == s[::-1]
来源：http://hz.cucudq.cn/gtlsivmhlj.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gtsouvjtpb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtyoxsskhm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtymmteqoj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenzaomai.com/gtqlrncyow.html

Go:   // 双指针从两端比较
来源：http://hz.ybcxt.top/gtyixdjuel.html

Ruby: s == s.reverse
来源：http://hz.nanxuanxn.top/gtfvuaztvm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gzhubu.top/gtlfvsfivh.html

[N07] 两数之和（返回下标）
来源：http://hz.iojbl.cn/gtvogijbvq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jlsjyb.cn/gtbiqcfwcu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tian-w.cn/gtntarllro.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinghuilouyu.cn/gtjpervvel.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydjk.org.cn/gtjriquuna.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtymonaxdk.html

Go:   // 手写 map[int]int
来源：http://hz.xuetiantiany.cn/gtybitksbu.html

Ruby: // 手写 Hash
来源：http://hz.yj20258888.top/gtyowfjngl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtcohdoabs.html

[N08] 生成全排列
来源：http://hz.jinqigufen.top/gtpncmfuys.html

Py:   itertools.permutations(arr)
来源：http://hz.fzhhl.top/gtmntpcdyk.html

PHP:  // 手写递归交换
来源：http://hz.jqgfzy.top/gtqkggbyjj.html

JS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtbachmvcx.html

TS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtdxkglzyu.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtmyuobmdc.html

Go:   // 手写回溯递归
来源：http://hz.316326.xyz/gtnlbyiflc.html

Ruby: arr.permutation.to_a
来源：http://hz.yuanzhike.top/gtrldpnvwr.html

C#:   // 手写回溯递归
来源：http://hz.yonumen.top/gtnhzvycpu.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gtzfqyjjof.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtpqdlzoow.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtueywnuxe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tanke756.top/gtcnrhwtrp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtsgbtcekx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yvedp.cn/gtyegestea.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yueranfly.top/gtyvtjithc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shuidangran.top/gtsommwwca.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.meibo888.top/gtqjoeqttb.html

[N10] 链表节点定义
来源：http://hz.hammf.cn/gtvywjptkt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtpdkmjwxi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangkeji.top/gteohwijyx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jlsjyb.cn/gtoonabivg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.c1oappe.top/gtptnmkfgf.html

Java: class Node { int v; Node next; }
来源：http://hz.bjfxy.top/gtsjbbgzzr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangtech.top/gtcajixiqd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangshuangyany.cn/gtcqhnnxae.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tanke756.top/gthmqegiaw.html

[N11] 二叉树中序遍历
来源：http://hz.yuanzhike.top/gtiqchlccg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtoqarkvuu.html

PHP:  // 手写递归函数
来源：http://hz.aibaodan.cn/gtacqjifqy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gtofcdtyee.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtshwoxxzk.html

Java: // 手写递归
来源：http://hz.shuidangran.top/gthoquomeu.html

Go:   // 手写递归
来源：http://hz.cashguo.top/gtqpvibxvw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.snrcjt.cn/gtetkgqtuj.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gthwojazxl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xingfuxueyuan.xyz/gtlxrrihlo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhoulong.xyz/gtmqcctidb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tianlin.xyz/gtemujkjys.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtrnmfqfgj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daria6918.cn/gthdtwuhfl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinyuanbaomall.cn/gtxylrctzj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yangfankeji.com/gtdguimtrn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dashuyun.cn/gtsxgwviac.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtcquitvrx.html

================================================================================
来源：http://hz.mhx1999.top/gthopimbtd.html

O. 并发与异步
来源：http://hz.xuetiantiany.cn/gtvihzvodo.html

================================================================================
来源：http://hz.gzhubu.top/gtapehlqtp.html

[O01] 启动一个线程
来源：http://hz.cdnleiting.top/gtpyfealds.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cheryme.top/gtpvqlexwq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cqqwz.cn/gthqwzuteu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xuanzx.com/gtnmjzdanm.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gttfkmuswg.html

Java: new Thread(() -> f()).start()
来源：http://hz.haohaochexian.top/gtrxjgvbhb.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtkqswucqt.html

Ruby: Thread.new { f }
来源：http://hz.zhengqikj.top/gtifdueexv.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtuoezpeni.html

[O02] 使用线程池
来源：http://hz.cqqwz.cn/gttrpmeido.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnqzz.top/gtwqvixqtd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuanzhike.top/gtsoitzcia.html

JS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gthzpcvsry.html

TS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtbgqffojf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guowangkeji.top/gtlgmjvbsh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guowangkeji.top/gtfvnckhzw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yonumen.top/gtohpxvmxv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.haohaochexian.top/gtijhpdhsg.html

[O03] 加锁保护共享数据
来源：http://hz.xingfuxueyuan.xyz/gtglcrwtxu.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtxnbdwjxn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtjmhajdel.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.vqdsnc.cn/gtreppmglu.html

TS:   // 同 JS
来源：http://hz.ehwqpu.com/gtqniocfed.html

Java: synchronized (this) { shared++; }
来源：http://hz.daria6918.cn/gtfflfobvc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gogol.net.cn/gtxjsaotni.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.wangshuangyany.cn/gtyooptrvb.html

C#:   lock (gate) { shared++; }
来源：http://hz.hywenlv.cn/gthpsyzndh.html

[O04] 定义异步函数并等待
来源：http://hz.yueranfly.top/gtjhkvqlgn.html

Py:   async def f():⏎    await g()
来源：http://hz.zhoulong.xyz/gtmbsukfdm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258888.top/gtfgghxfln.html

JS:   async function f() { await g(); }
来源：http://hz.shzxlz.cn/gtakkdhdvj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigfzy.top/gtvvmovrqt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gtbmoadfra.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhijiandao.cn/gtysafxsjk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hysaishi.cn/gtesrnibkn.html

C#:   async Task F() { await G(); }
来源：http://hz.jyoumei.cn/gtogpmcnsl.html

[O05] 并发执行并等待全部完成
来源：http://hz.hywenlv.cn/gtqgsjlfsu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuetiantiany.cn/gtervehfbp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xingfuxueyuan.xyz/gtejnhkhyk.html

JS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtaptxadmo.html

TS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtqeolvvzw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fzhhl.top/gtzbzrqivj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhoulong.xyz/gtkmghpeqs.html

Ruby: threads.map(&:join)
来源：http://hz.ivvv.top/gtkgbaprwt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hongshengwenyu.top/gtrukofhhw.html

[O06] 使用进程池
来源：http://hz.jqgfzy.top/gtkpmkotjc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.haohaochexian.top/gtsvtnxaqv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhengqikj.top/gtwnrsslsd.html

JS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gttuttgprx.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gttxmcqtmm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hammf.cn/gtgvmtwgcd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gtuvxhnwae.html

Ruby: // fork 块
来源：http://hz.jqgufenzy.top/gtctyfcaqy.html

C#:   Parallel.For
来源：http://hz.daxiang520.top/gtiueldguu.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvqriybfm.html

P. 常用工具函数
来源：http://hz.hammf.cn/gtiohgygpb.html

================================================================================
来源：http://hz.cqqwz.cn/gtmoomnife.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gtbqcohraq.html

Py:   str(uuid.uuid4())
来源：http://hz.cdnleiting.top/gtluiirems.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hfpthk.cn/gtisocnwlo.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtcgkbliuo.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtwwjrgvmm.html

Java: UUID.randomUUID().toString()
来源：http://hz.shzxlz.cn/gtuicfujnc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sweek.top/gtescgjpzr.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtfkybkqke.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yanxiufei.cn/gtbahptlji.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hnqzz.top/gtnwdlksbt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydjk.org.cn/gtgciimsyt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.quarkkingdee.top/gtwcxbndkw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuanzhike.top/gttfpmlzau.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.haohaochexian.top/gtbldyqyqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daria6918.cn/gtvglixqvn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.snrcjt.cn/gtjamfxdug.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gtmaxibznz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.52xcode.cn/gtgnoixlxj.html

[P03] 生成短随机字符串
来源：http://hz.zycfv.cn/gtfkzlbftk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jlsjyb.cn/gtvfgucxly.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fzhhl.top/gtnzjrersf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtwhndiucr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtgantlylr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.52xcode.cn/gtbwnrvmwn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtfvoutrsy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tian-w.cn/gtdbuhhjzx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.andypj.xyz/gtorbrbvin.html

[P04] 求长度
来源：http://hz.jyoumei.cn/gtmeuubkgq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtaqdqunyf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtjcjlwbqj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtuvsgclci.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtsorxnxtp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtaybucrrl.html

Go:   len(arr);  len(m)
来源：http://hz.svipenyu.cn/gttzntnbdx.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtftspefdk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhengqikj.top/gtjcilbrrf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinyuanbaomall.cn/gtvsmhxcad.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.andypj.xyz/gtyupecchh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hongshengwenyu.top/gtpuasccjc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jiagoushi.top/gtgrjerisc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zycfv.cn/gtzupvcgcr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangshuangyany.cn/gtwrqluduw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhongyouzk.top/gttwchofob.html

Ruby: a == b
来源：http://hz.yuanzhike.top/gthhuihlfs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tianlin.xyz/gtlnmaxuia.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zdqjudy.top/gtiqzcnvkf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtqyyrnlvt.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gtjtdbhpxt.html


<!-- 参考信息 -->