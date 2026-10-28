代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhixingplan.top/gtqibbunrs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gotoacloud.top/gtlwprkbrl.html

================================================================================
来源：http://hz.ivvv.top/gtuxdfcngk.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gtglbkbmot.html

================================================================================
来源：http://hz.gaohongyu789.top/gtffsflrze.html

[M01] 读取命令行参数
来源：http://hz.yvedp.cn/gtpukvmtju.html

Py:   sys.argv[1:]
来源：http://hz.sweek.top/gtpdzjpigc.html

PHP:  $argv;  $argc;
来源：http://hz.feifeiyinyue.top/gtovbgbtil.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtiwhuvjqc.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtxvruurwf.html

Java: args 数组（main 方法参数）
来源：http://hz.ybcxt.top/gtdwgwqowb.html

Go:   os.Args[1:]
来源：http://hz.hysaishi.cn/gtziacmwyb.html

Ruby: ARGV
来源：http://hz.hysaishi.cn/gtbdcsvqhb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aizwys.cn/gtburdmcne.html

[M02] 读取环境变量
来源：http://hz.ydzc1.top/gtsjkginve.html

Py:   os.environ.get("HOME")
来源：http://hz.birdmap.top/gtgdxjzcet.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtxytahxdj.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtgflnojfc.html

TS:   process.env.HOME
来源：http://hz.yonumen.top/gtzarfcqcl.html

Java: System.getenv("HOME")
来源：http://hz.gotoacloud.top/gtvisszcrt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.feifeiyinyue.top/gtuhhpvqsd.html

Ruby: ENV["HOME"]
来源：http://hz.zhongyouzk.top/gtowdrmcgl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xinyue.icu/gtbujmobsb.html

[M03] 执行外部命令
来源：http://hz.smart0.xyz/gtsrjetuwc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtrdgzbtps.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gogol.net.cn/gtbrypqluz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtjjvuwwdn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gttzprgiga.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yongpay.top/gtrclsnbbo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtizrrxmze.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jianghu66.top/gtsjzexyeh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guannengcc.top/gtohywplzd.html

[M04] 获取当前工作目录
来源：http://hz.gotoacloud.top/gtixdtjied.html

Py:   os.getcwd()
来源：http://hz.nanxinkj.top/gtyhylpwot.html

PHP:  getcwd();
来源：http://hz.zdqjudy.top/gtlyphjuks.html

JS:   process.cwd()
来源：http://hz.yj20258888.top/gtvxhpylji.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gtovuqrhcb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ppjwa.cn/gthgyeqtic.html

Go:   os.Getwd()
来源：http://hz.tian-w.cn/gtxtlpclyt.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtnppnawpd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aizwys.cn/gtwnmwlowf.html

[M05] 设置退出码
来源：http://hz.ivvv.top/gttxtxmtnn.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtxjrjkfqb.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gtdstzoezu.html

JS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtljkkepon.html

TS:   process.exit(1)
来源：http://hz.xylfe.cn/gtpnmwvclp.html

Java: System.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtqbymqycw.html

Go:   os.Exit(1)
来源：http://hz.xylfe.cn/gttctybarf.html

Ruby: exit 1
来源：http://hz.ydjk.org.cn/gttyrufgag.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenjidiqi.icu/gtqghvftde.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gtcjdyulzn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtujeoyhiq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuanzhike.top/gtjazdjgut.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtiktslbvp.html

TS:   console.error("err")
来源：http://hz.sxryk.cn/gtnplbdpul.html

Java: System.err.println("err")
来源：http://hz.iojbl.cn/gtbwzbhcpf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangtech.top/gtjtdjikqa.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gtjemqsgby.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gtpurhrfzf.html

[M07] 判断是否为主入口
来源：http://hz.snrcjt.cn/gtujmxvoul.html

Py:   if __name__ == "__main__":
来源：http://hz.zycfv.cn/gtmybzrbfw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuetiantiany.cn/gtvkwpjlaq.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtckjwekri.html

TS:   require.main === module
来源：http://hz.sweek.top/gtqzrtymod.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtdjrnlfgv.html

Go:   func main()
来源：http://hz.nanxinkj.top/gtpnrjzbmd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gtjhobgipj.html

C#:   static void Main(string[] args)
来源：http://hz.xziqi.cn/gtuzfzyvtr.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gtsehlbuss.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gteyvmgbvl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.redwolf501.top/gtophxahpd.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtjkbcsetv.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtcruojavn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yueranfly.top/gtgjrcbhmy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shzxlz.cn/gtethyifhc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.52xcode.cn/gtzvjkwkgr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhixingplan.top/gtpwvdcwgq.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxehmqwcn.html

N. 数据结构与算法
来源：http://hz.zhaomingkeji.xyz/gtoqhzwtph.html

================================================================================
来源：http://hz.daria6918.cn/gthbuoilpi.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtmbrhbusu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigufen.top/gtbjhyigwx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtbusdsgrm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtujzqjotr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtehqhmaye.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tian-w.cn/gtdhqklxnt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtqsjpwegs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhongyouzk.top/gtfloeeosu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yueranfly.top/gtmzlqatgt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhiwuduotai.top/gtncyjtcwr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtepgkabmh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtxwmbtquu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtrefyrtnr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtjnyyvzyh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tianlin.xyz/gtiiilqydj.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtnxsjhtzj.html

Ruby: arr.sort
来源：http://hz.zycfv.cn/gtienwntar.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hongshengwenyu.top/gtjbxnfiql.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258.top/gtsuvoazpw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigfzy.top/gtknkjuwkz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigufen.top/gtihalbilp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gtwspymdlz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtycbojdba.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xingfuxueyuan.xyz/gttutokggc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.vqdsnc.cn/gtgrbowzzf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuanzhike.top/gtribldxxf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dashuyun.cn/gtqkeicjti.html

[N04] 斐波那契数列
来源：http://hz.jinyuanbaomall.cn/gtifrfspvo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtsccdvoxo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xziqi.cn/gtkzrnjhtc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtqxblyiqh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtgkmmhhsv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnqzz.top/gtbzlqldal.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xingfuxueyuan.xyz/gtijmvnicg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gthhhewxcl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xinyue.icu/gtlxjchkum.html

[N05] 最大公约数
来源：http://hz.tanke756.top/gtefgpnlns.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gtlgguguao.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.birdmap.top/gtephvaqwp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtjgcpciev.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtkcwvpgas.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhijiandao.cn/gtpsfiwzya.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.vqdsnc.cn/gtrimyyvpf.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtkgnwfdut.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nwbrower.top/gtkiycnhva.html

[N06] 判断回文字符串
来源：http://hz.jyoumei.cn/gtyzrgzeyz.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gtiyviwwel.html

PHP:  $s === strrev($s);
来源：http://hz.gotoacloud.top/gtylpopdgk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtqyntzeek.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtbndxqpok.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuanzx.com/gtddciwkmd.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtuwfnotpa.html

Ruby: s == s.reverse
来源：http://hz.cheryme.top/gtnjpgasba.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtzsguqsma.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtlspzimar.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.haohaochexian.top/gtyqiepuuf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.bjfxy.top/gtupoputyz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenlongwang.top/gtdxyltoea.html

TS:   // 手写 Map<string, number>
来源：http://hz.hammf.cn/gtristbqwt.html

Java: // 手写 HashMap
来源：http://hz.bjfxy.top/gtyjffazzf.html

Go:   // 手写 map[int]int
来源：http://hz.hongshengwenyu.top/gthuoadpqs.html

Ruby: // 手写 Hash
来源：http://hz.quarkkingdee.top/gtmhlrcvve.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yonumen.top/gtimqvpieu.html

[N08] 生成全排列
来源：http://hz.feifeiyinyue.top/gteigjymwt.html

Py:   itertools.permutations(arr)
来源：http://hz.fengsongda.top/gtpbfkctzi.html

PHP:  // 手写递归交换
来源：http://hz.cucudq.cn/gtdafvtihf.html

JS:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtkzyffcsm.html

TS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtudwxfrpk.html

Java: // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtjmeriend.html

Go:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtnhfcfidq.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gtetulrnqb.html

C#:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtsikrwnbu.html

[N09] 栈与队列
来源：http://hz.sxryk.cn/gtniqcrwvs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gtiebyxmdf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yongpay.top/gtckfzolmx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ppjwa.cn/gtfhoqbbpr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.52xcode.cn/gtfpfoifir.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtdxxzetjr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.birdmap.top/gtokzsftwb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gthvdjigfv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daxiang520.top/gtoqinhctt.html

[N10] 链表节点定义
来源：http://hz.jqgfzy.top/gthwyflouz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shangyingyoupin.top/gteelmyfrk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangtech.top/gthybdmthr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tian-w.cn/gtpgmkapaj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gtzfncqmqy.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gthpupimgy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hysaishi.cn/gtqtoveboc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ehwqpu.com/gtpkaqjlry.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jiagoushi.top/gtcwjcforz.html

[N11] 二叉树中序遍历
来源：http://hz.vqdsnc.cn/gtkboshrqs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinghuilouyu.cn/gtiawfmtll.html

PHP:  // 手写递归函数
来源：http://hz.xinyue.icu/gtkmugbror.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnxiangtu.top/gtjuupcejb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtnxpfkxqs.html

Java: // 手写递归
来源：http://hz.wangdashe.top/gtqicudkaf.html

Go:   // 手写递归
来源：http://hz.yj202588.top/gtmmjfufxx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.316326.xyz/gtbqmhlixt.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gttngprxcz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sweek.top/gtczqbifno.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.bjfxy.top/gtngzqurqm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sysykeji.top/gthobsxzzu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtmabzmdnl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtetufynrg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtlccntqeg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.kuanghao11.cn/gtgvjnphmk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.kuanghao11.cn/gtllsfbppq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gttpmmgjeo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtusrerjst.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtlprgobiy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvgbdtnjg.html

[O01] 启动一个线程
来源：http://hz.xuanzx.com/gtkkwlwqjk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangdashe.top/gtacxrxkrj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xingfuxueyuan.xyz/gtcpevtyhd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cheryme.top/gtlxvrlmui.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtvgmbmthk.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gtkeoplzsg.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gthrzmmwst.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gtikrlxnhu.html

C#:   Task.Run(() => F());
来源：http://hz.hammf.cn/gtzpvcoszc.html

[O02] 使用线程池
来源：http://hz.shangyingyoupin.top/gtqyvwnyak.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtlzhxpvrb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shzxlz.cn/gtefaprart.html

JS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtnjlnbdij.html

TS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtlvaspwed.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj20258.top/gtotglhsgs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtyonqbaoq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yangfankeji.com/gtbgaqzfox.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yanxiufei.cn/gtylhhezbt.html

[O03] 加锁保护共享数据
来源：http://hz.ydzc1.top/gtbufwwsbu.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtzvscrseo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jiagoushi.top/gtdlckpdud.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sufxvd.cn/gtiviiansi.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtocazrywx.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258888.top/gtchjfppok.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cdnleiting.top/gtkhkqbctd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gthobcwqbr.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258.top/gtogayezib.html

[O04] 定义异步函数并等待
来源：http://hz.zdqjudy.top/gtnrjnnwxe.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxuanxn.top/gtcuqxvomi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgufenzy.top/gtfcptzoxr.html

JS:   async function f() { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtvucwysrv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtgzyurjej.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aizwys.cn/gtmpnfoybz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gogol.net.cn/gtlhpuziod.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhiwuduotai.top/gtuwrzvtfg.html

C#:   async Task F() { await G(); }
来源：http://hz.wangshuangyany.cn/gtvmsdmjbp.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgufenzy.top/gtqcojgnqa.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daria6918.cn/gtytybatdt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shangyingyoupin.top/gtzhorzxvg.html

JS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtxemeatjf.html

TS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtfxfpvfyo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhongyouzk.top/gtkpbncqzp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ybcxt.top/gtqmlzxcxg.html

Ruby: threads.map(&:join)
来源：http://hz.yuxming.cn/gtlgvveexb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gotoacloud.top/gtzoncjchq.html

[O06] 使用进程池
来源：http://hz.sufxvd.cn/gtcjkulnmv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.quarkkingdee.top/gtjkhhnqed.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.mhx1999.top/gtbnofluhc.html

JS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtwlzesnxt.html

TS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtkpuhcgcj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhoulong.xyz/gtgwsdcpva.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.c1oappe.top/gttpwyviss.html

Ruby: // fork 块
来源：http://hz.zhiwuduotai.top/gtpffwphsq.html

C#:   Parallel.For
来源：http://hz.gogol.net.cn/gtblmnpsde.html

================================================================================
来源：http://hz.yangfankeji.com/gtqxrwkyhw.html

P. 常用工具函数
来源：http://hz.ybcxt.top/gtvriulabn.html

================================================================================
来源：http://hz.vqdsnc.cn/gtiqpkdawd.html

[P01] 生成 UUID
来源：http://hz.ivvv.top/gtmvijqdaz.html

Py:   str(uuid.uuid4())
来源：http://hz.guannengcc.top/gtkcacjtes.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.feifeiyinyue.top/gtndyqclmd.html

JS:   crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtvneoocku.html

TS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtwasoajbs.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnqzz.top/gtsftbatyo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daxiang520.top/gtsscphnhu.html

Ruby: SecureRandom.uuid
来源：http://hz.cucudq.cn/gtmleezwnh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.svipenyu.cn/gtmslgwovi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhongyouzk.top/gtzxgwsftq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.redwolf501.top/gtlhfpmjbt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenlongwang.top/gtytxehmow.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.dashuyun.cn/gtvnpdwkvr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.kuanghao11.cn/gtvxbocgdl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shuidangran.top/gthtnlprbc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gttmajgzxt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinghuilouyu.cn/gtxnuldnqa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fengsongda.top/gtpcovcqpn.html

[P03] 生成短随机字符串
来源：http://hz.jinqigfzy.top/gtmkvjvtfy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gtizfxcleh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.quarkkingdee.top/gtctowrrdv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtzawvkbpt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtsxxisofe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtvezeccpk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gtlyblpanu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yangfankeji.com/gtujwaxuef.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuanzhike.top/gtbpysgwxe.html

[P04] 求长度
来源：http://hz.redwolf501.top/gtcqpsslsv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhiwuduotai.top/gtrpejggdl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtgwyijtzl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sysykeji.top/gtureeopzc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtqvovsnay.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jqgfzy.top/gtmiqglsic.html

Go:   len(arr);  len(m)
来源：http://hz.yangfankeji.com/gtdndgvrbe.html

Ruby: x.length;  x.size
来源：http://hz.jinqigfzy.top/gtddyvnyvx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zdqjudy.top/gtmxllzlrs.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xinyue.icu/gtmjqqgkke.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shzxlz.cn/gtcgcmlhgo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jyoumei.cn/gtldfjehxm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.havefunace.top/gtfszqlvzb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtawrxfboy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zycfv.cn/gtvoocchrj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.haohaochexian.top/gtwpabdrkf.html

Ruby: a == b
来源：http://hz.xziqi.cn/gtwvnwgckt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nanxuanxn.top/gtfesaptge.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgufenzy.top/gtqwyvvmwp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.52xcode.cn/gtokwmuyws.html

PHP:  if (empty($x)) {}
来源：http://hz.kuanghao11.cn/gthsmequks.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daria6918.cn/gtxdecocip.html

TS:   if (x == null) {}
来源：http://hz.hammf.cn/gtuankeztz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ivvv.top/gtjwfnvagd.html

Go:   if x == nil {}
来源：http://hz.shuidangran.top/gtgainboly.html


<!-- 参考信息 -->