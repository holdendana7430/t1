代发 wailian999

================================================================================
来源：http://hz.wangshuangyany.cn/gtbopddjtv.html

[M01] 读取命令行参数
来源：http://hz.jinqigufen.top/gtipmmnend.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtggpsdoew.html

PHP:  $argv;  $argc;
来源：http://hz.jinyuanbaomall.cn/gtfzjwxghp.html

JS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtltexzkyp.html

TS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtqliktuyg.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtjvfxjqyh.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtyuiqmhkd.html

Ruby: ARGV
来源：http://hz.daxiang520.top/gtcltehehe.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgfzy.top/gtliwaebjh.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtkvfmptyv.html

Py:   os.environ.get("HOME")
来源：http://hz.zycfv.cn/gtuygqkocf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cheryme.top/gtvrwbhehz.html

JS:   process.env.HOME
来源：http://hz.havefunace.top/gthryopxcn.html

TS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtjqwextmd.html

Java: System.getenv("HOME")
来源：http://hz.chenjidiqi.icu/gtsqqvtjwy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hongshengwenyu.top/gtczfsurot.html

Ruby: ENV["HOME"]
来源：http://hz.redwolf501.top/gtcufepejv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daria6918.cn/gtrbbfnmdt.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtsntyeebr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenlongwang.top/gtzubwzrmw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuanzhike.top/gtwheotuhw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtekxawigr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtlvomnrac.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gteaxnlftq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cqqwz.cn/gtglunqbtz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.haohaochexian.top/gtkbcqzfrn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtemtfqprp.html

[M04] 获取当前工作目录
来源：http://hz.yj20258.top/gtfhzcbxbv.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtdwdqxpsn.html

PHP:  getcwd();
来源：http://hz.zhengqikj.top/gthrqbsasc.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtrghcibbd.html

TS:   process.cwd()
来源：http://hz.meibo888.top/gtdfqjvojj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pycfn.com/gtyedxtoqw.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtqllqajxt.html

Ruby: Dir.pwd
来源：http://hz.hnxiangtu.top/gtuypzrawi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cheryme.top/gtpaalcsvz.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtnkvvqtcl.html

Py:   sys.exit(1)
来源：http://hz.mhx1999.top/gtjbcqwfxk.html

PHP:  exit(1);
来源：http://hz.ydjk.org.cn/gtqvqnnnle.html

JS:   process.exit(1)
来源：http://hz.fzhhl.top/gtrerkbyhu.html

TS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtrwtlngnc.html

Java: System.exit(1)
来源：http://hz.jinqigfzy.top/gtgaoqymfb.html

Go:   os.Exit(1)
来源：http://hz.fengsongda.top/gtuoxpgyjb.html

Ruby: exit 1
来源：http://hz.sysykeji.top/gtakelcloo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yonumen.top/gtgcfxemje.html

[M06] 向标准错误输出
来源：http://hz.iojbl.cn/gtzufwthqx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtotvnocof.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtxuejmnep.html

JS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtnjriwjbc.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtrkpfgtal.html

Java: System.err.println("err")
来源：http://hz.tanke756.top/gtqsczvfbo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ywan-chungtsiang.top/gtdsnzrkhk.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtruhfaxmi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hywenlv.cn/gtihrmblnx.html

[M07] 判断是否为主入口
来源：http://hz.jqgfzy.top/gtlkiqajki.html

Py:   if __name__ == "__main__":
来源：http://hz.daria6918.cn/gtajkjqrfr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guannengcc.top/gtdlddlowm.html

JS:   require.main === module
来源：http://hz.jyoumei.cn/gtfpbryfqe.html

TS:   require.main === module
来源：http://hz.hnqzz.top/gtxaiedxeo.html

Java: public static void main(String[] args)
来源：http://hz.ywan-chungtsiang.top/gtwntgtezq.html

Go:   func main()
来源：http://hz.gogol.net.cn/gtijejasem.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yanxiufei.cn/gtulurdupv.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtulkprijz.html

[M08] 获取系统与运行时信息
来源：http://hz.kuanghao11.cn/gtewmuugnr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtsykybpzi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhijiandao.cn/gtkszllvpi.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtuzpxjcgu.html

TS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtdcmseygm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gtsereeihm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuanzx.com/gtudpjfcpd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fzhhl.top/gtdngfmsrd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydzc1.top/gtylwbrmpt.html

================================================================================
来源：http://hz.smart0.xyz/gtxgqafcks.html

N. 数据结构与算法
来源：http://hz.chenlongwang.top/gtxphhfdhn.html

================================================================================
来源：http://hz.chenlongwang.top/gtshyznklu.html

[N01] 二分查找（有序数组）
来源：http://hz.andypj.xyz/gtgpflfghs.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ppjwa.cn/gthxcbteys.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yueranfly.top/gtapbnefiy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtbvywawwb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtaupbluxu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtwoyxgktz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhijiandao.cn/gtmqixdwhe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxinkj.top/gtmdrbsssi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydzc1.top/gtbvfmyruk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhixingplan.top/gtngjajdmp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtnlxlojpc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shzxlz.cn/gtfgigardl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtjxrmkdnr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gticixrnbg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zdqjudy.top/gtraoixegx.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gthknkxbze.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtypmfxidp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenzaomai.com/gtzahbdpjm.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gtnjxpfjlc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yanxiufei.cn/gtzcqupltg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtanxqerza.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtwzecyhvs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtdczlxwbe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.andypj.xyz/gtnalpgpgk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuanzhike.top/gtftiyqvfg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhengqikj.top/gtucweywmh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtqranfxtq.html

[N04] 斐波那契数列
来源：http://hz.gaohongyu789.top/gtgffjezvn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtuvpsvgtp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtshxagowk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gtsmimineb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtqlnhaqcn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gtwjzelhnm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hfpthk.cn/gteycckxxr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtoohdfdwv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.9152youxi.cn/gtkotslljn.html

[N05] 最大公约数
来源：http://hz.snrcjt.cn/gtvuipsqjm.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gtnlzfpobd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.redwolf501.top/gtzelxnmxy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtfvttijft.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.9152youxi.cn/gtgqrhgdzn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydzc1.top/gtpnttdnlb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.smart0.xyz/gtipdjebxz.html

Ruby: a.gcd(b)
来源：http://hz.ydjk.org.cn/gtlqyycjhn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydjk.org.cn/gtjlmxhxcy.html

[N06] 判断回文字符串
来源：http://hz.ivvv.top/gturxbsefw.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtzcwuusus.html

PHP:  $s === strrev($s);
来源：http://hz.chenzaomai.com/gtqtfpdmby.html

JS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtxubswnzh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtofiwcnbw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aizwys.cn/gtsqurxswb.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtscamwhvy.html

Ruby: s == s.reverse
来源：http://hz.zhixingplan.top/gtcwgqbpcw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gttcgbjddo.html

[N07] 两数之和（返回下标）
来源：http://hz.xuetiantiany.cn/gtownpvazb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gaohongyu789.top/gttqbkwybu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.vqdsnc.cn/gtxqzxpklj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cheryme.top/gttwzgdpfj.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtlzuzbdrc.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtvtevqzsq.html

Go:   // 手写 map[int]int
来源：http://hz.iojbl.cn/gtgeuntsef.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtaxoxqcqj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhoulong.xyz/gttgnlkyyg.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtvvlsuonk.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtgyrcitln.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangtech.top/gtsmrjbbcc.html

JS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtastdtgoz.html

TS:   // 手写回溯递归
来源：http://hz.yj20258.top/gttuismfce.html

Java: // 手写回溯递归
来源：http://hz.redwolf501.top/gtbsnbsxlt.html

Go:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtxpeschdv.html

Ruby: arr.permutation.to_a
来源：http://hz.dianchejie.cn/gtxcgikezj.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtumavjnec.html

[N09] 栈与队列
来源：http://hz.chenlongwang.top/gtijoubyab.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtubuidhke.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dashuyun.cn/gtvaeqoroe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.havefunace.top/gtcxczphkp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuanzx.com/gtxkttxzhd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenzaomai.com/gtcppmiffs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nanxuanxn.top/gtwwyoigqy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.meibo888.top/gttckwfgvx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.snrcjt.cn/gtykgwkjsi.html

[N10] 链表节点定义
来源：http://hz.gzhubu.top/gtaghurdem.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.kuanghao11.cn/gtqipifxpk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gzhubu.top/gtuobqbiuv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.feifeiyinyue.top/gtyumydgmj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenjidiqi.icu/gtjqpguvmq.html

Java: class Node { int v; Node next; }
来源：http://hz.shzxlz.cn/gtmqrsdfcx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.svipenyu.cn/gtmxrvguuu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtsmslcwmb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xziqi.cn/gtnvzwfpcf.html

[N11] 二叉树中序遍历
来源：http://hz.sufxvd.cn/gtltjpygyn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtaojyvvgu.html

PHP:  // 手写递归函数
来源：http://hz.shanyushiyangtech.top/gtlxjfexim.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtvscuuvku.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtpioieqni.html

Java: // 手写递归
来源：http://hz.c1oappe.top/gtaienyktn.html

Go:   // 手写递归
来源：http://hz.ydjk.org.cn/gtisxziwwn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtrdldjlde.html

C#:   // 手写递归
来源：http://hz.zhijiandao.cn/gtjsgqjeak.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtaqkbrcry.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtnlwtbbuz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hysaishi.cn/gtnlupyvct.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtaydccupg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ivvv.top/gtdgbcestv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtuqufytta.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sxryk.cn/gtnejzmcic.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pycfn.com/gtvjekfpwp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigfzy.top/gtzksinvnv.html

================================================================================
来源：http://hz.chenzaomai.com/gtncisjwju.html

O. 并发与异步
来源：http://hz.c1oappe.top/gtggtuwsbg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkccbtklp.html

[O01] 启动一个线程
来源：http://hz.yongpay.top/gtoraddpjo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinghuilouyu.cn/gtrwsiavmk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gtidpnmhsb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtzxrieley.html

TS:   // 同 JS
来源：http://hz.nanxinkj.top/gtiedtchzw.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtrzeopwlo.html

Go:   go f()
来源：http://hz.yuanzhike.top/gtmgdxoiyw.html

Ruby: Thread.new { f }
来源：http://hz.ydzc1.top/gtegnjsnwu.html

C#:   Task.Run(() => F());
来源：http://hz.ivvv.top/gtaizxsztl.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtjjodplez.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.0kj1m.cn/gthazjwkzt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.snrcjt.cn/gtkizdzrgp.html

JS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtfgqzaana.html

TS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtuzpeuygu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gtimcxtggz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.316326.xyz/gtvtfnygzn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aibaodan.cn/gtvaruzjlt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gtuyabfrui.html

[O03] 加锁保护共享数据
来源：http://hz.zhixingplan.top/gthrnzhxzd.html

Py:   with lock: shared += 1
来源：http://hz.ydzc1.top/gtyqkxdbkj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shangyingyoupin.top/gtqshwcthz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dianchejie.cn/gttkwurouz.html

TS:   // 同 JS
来源：http://hz.cqqwz.cn/gtevukjazi.html

Java: synchronized (this) { shared++; }
来源：http://hz.cashguo.top/gtflblezxe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gtdodmxmxg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gtoghsmzon.html

C#:   lock (gate) { shared++; }
来源：http://hz.yuanzhike.top/gtozwbjupf.html

[O04] 定义异步函数并等待
来源：http://hz.iojbl.cn/gtzlxwlcoi.html

Py:   async def f():⏎    await g()
来源：http://hz.0kj1m.cn/gtujuuyzqy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daria6918.cn/gtgnllcqle.html

JS:   async function f() { await g(); }
来源：http://hz.ydjk.org.cn/gtymkuphpn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenjidiqi.icu/gtagmgpvfk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jyoumei.cn/gtulxmhkbx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daria6918.cn/gtcqfukwdk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258.top/gtktxjakuj.html

C#:   async Task F() { await G(); }
来源：http://hz.ybcxt.top/gtvkycqjox.html

[O05] 并发执行并等待全部完成
来源：http://hz.fzhhl.top/gtppqhgqam.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuanzhike.top/gtrprqpakq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hammf.cn/gtcbpiqajh.html

JS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gtglhpehnb.html

TS:   await Promise.all(tasks)
来源：http://hz.guannengcc.top/gtzbqpqcux.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cashguo.top/gtzufwutmx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ybcxt.top/gthxbeleix.html

Ruby: threads.map(&:join)
来源：http://hz.haohaochexian.top/gtabuhpxgh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.kuanghao11.cn/gtlrjyclee.html

[O06] 使用进程池
来源：http://hz.zhoulong.xyz/gtemlexlhk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhengqikj.top/gtwjmimzfc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuanzhike.top/gtwtlbqrxu.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtpkbgwslg.html

TS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtajldksgr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhijiandao.cn/gtamnfdffk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xinyue.icu/gtajuwslcb.html

Ruby: // fork 块
来源：http://hz.jyoumei.cn/gthjvismsk.html

C#:   Parallel.For
来源：http://hz.yangfankeji.com/gtjpjebsdm.html

================================================================================
来源：http://hz.sxryk.cn/gtsewqymiy.html

P. 常用工具函数
来源：http://hz.hongshengwenyu.top/gtgqyqtsiv.html

================================================================================
来源：http://hz.zhoulong.xyz/gthyztzrlq.html

[P01] 生成 UUID
来源：http://hz.birdmap.top/gtqjesjepb.html

Py:   str(uuid.uuid4())
来源：http://hz.jyoumei.cn/gtgjwbrwem.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hfpthk.cn/gtcswbvuhm.html

JS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtorrenceh.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtwsugqbnc.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhengqikj.top/gtjezyowsl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gotoacloud.top/gtzedhievm.html

Ruby: SecureRandom.uuid
来源：http://hz.zhijiandao.cn/gtmyjtycfj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yongpay.top/gtbnhlwtxb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gtzdvzlydi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jiagoushi.top/gtvpuluazg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sufxvd.cn/gtvktmindx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cdnleiting.top/gtenxajgrx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.redwolf501.top/gtimbdsoyw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangshuangyany.cn/gtpsrabtgs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tanke756.top/gtkwutxwlg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtjxsffonu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pycfn.com/gtfanzxwha.html

[P03] 生成短随机字符串
来源：http://hz.mhx1999.top/gtwbvnbneh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cqqwz.cn/gtbviqxvap.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cqqwz.cn/gtttmdmchh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtffognhrq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtwyfyphly.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhiwuduotai.top/gtfpjfezmk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daria6918.cn/gtujbmfwpw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jyoumei.cn/gtyeeioyhz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ywan-chungtsiang.top/gtcuixxibn.html

[P04] 求长度
来源：http://hz.ywan-chungtsiang.top/gtjfixecla.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xinyue.icu/gtetyltomo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtzhhxprdp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtffafkgft.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sufxvd.cn/gtstwwdvpi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cdnleiting.top/gtmsekbyqb.html

Go:   len(arr);  len(m)
来源：http://hz.hysaishi.cn/gterhmlyow.html

Ruby: x.length;  x.size
来源：http://hz.ydjk.org.cn/gtafoxcelh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenjidiqi.icu/gtiaaayrgy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hfpthk.cn/gteuvmffrs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.quarkkingdee.top/gtaunkbawo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.vqdsnc.cn/gtdyadoylu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gtkvvjuwiv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtyngvgwgo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.haohaochexian.top/gtpllmqphj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhoulong.xyz/gtwbqaafrv.html

Ruby: a == b
来源：http://hz.cashguo.top/gtpvyvogyl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.0kj1m.cn/gtnvaytsmn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.snrcjt.cn/gtgnkutmoc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydjk.org.cn/gtwdebulks.html

PHP:  if (empty($x)) {}
来源：http://hz.gotoacloud.top/gtzqssqvfe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.vqdsnc.cn/gtlvsaylnb.html

TS:   if (x == null) {}
来源：http://hz.xylfe.cn/gtomzodjcv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shangyingyoupin.top/gtgjpkhcsa.html

Go:   if x == nil {}
来源：http://hz.andypj.xyz/gtqrgwvtpz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xingfuxueyuan.xyz/gtuglkfvve.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtczeqhuhx.html

[P07] 防抖与节流
来源：http://hz.andypj.xyz/gtgcqiufae.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.kuanghao11.cn/gtfqiyaqek.html


<!-- 参考信息 -->