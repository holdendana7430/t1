代发 wailian999

JS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtejkhotcy.html

TS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtpawccfos.html

Java: args 数组（main 方法参数）
来源：http://hz.hnqzz.top/gtsscsgyxd.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gtigrzueav.html

Ruby: ARGV
来源：http://hz.jianghu66.top/gtiypyiqps.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenjidiqi.icu/gtzwxmhmqs.html

[M02] 读取环境变量
来源：http://hz.tian-w.cn/gtnbmcpwjd.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtcirckcbc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aizwys.cn/gtxujijubm.html

JS:   process.env.HOME
来源：http://hz.iojbl.cn/gtsllsrnyj.html

TS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtfntlijab.html

Java: System.getenv("HOME")
来源：http://hz.dianchejie.cn/gtxjvzwfuv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yongpay.top/gtfmpqpnsy.html

Ruby: ENV["HOME"]
来源：http://hz.guannengcc.top/gtbusziysb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.smart0.xyz/gtjkwflvvq.html

[M03] 执行外部命令
来源：http://hz.nwbrower.top/gtkzhpqveu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dianchejie.cn/gtxcafcagd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigufen.top/gtrhprrfpl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtxmvudvap.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtazpqecln.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cdnleiting.top/gtxtqjhztu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shanyushiyangkeji.top/gtxizrwggt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtraosflqi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenlongwang.top/gtneqthclw.html

[M04] 获取当前工作目录
来源：http://hz.snrcjt.cn/gtfkpkaulk.html

Py:   os.getcwd()
来源：http://hz.jinyuanbaomall.cn/gtoqecbaya.html

PHP:  getcwd();
来源：http://hz.hnqzz.top/gtxcpzuccx.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtmkbvxhtb.html

TS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtysjoftex.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtdsqsujal.html

Go:   os.Getwd()
来源：http://hz.chenzaomai.com/gtnajmqrhz.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangtech.top/gtrwswuwaf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.birdmap.top/gtjukybejl.html

[M05] 设置退出码
来源：http://hz.bjfxy.top/gtwnacvtow.html

Py:   sys.exit(1)
来源：http://hz.ivvv.top/gtkbebegkw.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtafwucygn.html

JS:   process.exit(1)
来源：http://hz.sweek.top/gtcrxwtuiv.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtsgwiglfb.html

Java: System.exit(1)
来源：http://hz.daxiang520.top/gtwdslvyum.html

Go:   os.Exit(1)
来源：http://hz.yueranfly.top/gtzcfjacdt.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtqxshiwbg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shuidangran.top/gtybfnopif.html

[M06] 向标准错误输出
来源：http://hz.pycfn.com/gtzddrixzd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtplqmknaq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ivvv.top/gtebcuigjc.html

JS:   console.error("err")
来源：http://hz.xylfe.cn/gtnqkjuoza.html

TS:   console.error("err")
来源：http://hz.jianghu66.top/gtrpddxnyr.html

Java: System.err.println("err")
来源：http://hz.ppjwa.cn/gtdpsefuqe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gogol.net.cn/gtjhojzupd.html

Ruby: warn "err"
来源：http://hz.316326.xyz/gtwxjzzrjn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtewjtjzoo.html

[M07] 判断是否为主入口
来源：http://hz.xingfuxueyuan.xyz/gtgbfzlkku.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigfzy.top/gtjpfdaobb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydjk.org.cn/gtknhnzgms.html

JS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtonhseolz.html

TS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtayxvfcnk.html

Java: public static void main(String[] args)
来源：http://hz.smart0.xyz/gtiueirsmd.html

Go:   func main()
来源：http://hz.yongpay.top/gtkyvzfsgj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuanzx.com/gtokfyuxxg.html

C#:   static void Main(string[] args)
来源：http://hz.aibaodan.cn/gtpdziflnj.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtgzqopmyn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydzc1.top/gtlffypjfg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj202588.top/gtnnhnaajg.html

JS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtohetatqo.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gthejcmbjg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gtgldjcvdo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gtxatwmeji.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258.top/gtqbtreccm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.kuanghao11.cn/gtsoxmawfl.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtlmyscybf.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gtkddzlqyc.html

================================================================================
来源：http://hz.kuanghao11.cn/gtrujagwnb.html

[N01] 二分查找（有序数组）
来源：http://hz.yj202588.top/gtkgmfzfry.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.smart0.xyz/gtgjovaesx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtvvsxmpgs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gttirpqsvb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtwakrzbak.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtvunikvfb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.9152youxi.cn/gtbwfetpgh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.316326.xyz/gtjuqrypkc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zycfv.cn/gtdyznmlud.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aizwys.cn/gtfstjzojm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zycfv.cn/gtejmagpxx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hongshengwenyu.top/gtqmjxakwb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jianghu66.top/gtmordjbgs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtghrjburt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.c1oappe.top/gtltstjjrt.html

Go:   slices.Sort(arr)
来源：http://hz.yuxming.cn/gtvyhqecez.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtprltgmcz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.9152youxi.cn/gtxqkjcubi.html

[N03] 快速排序（分治示例）
来源：http://hz.shuidangran.top/gtqumsrvke.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ywan-chungtsiang.top/gttcxdoyan.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gtclizwefw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtgxqxstzs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtbkfeyplb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.guannengcc.top/gtxfdvujdl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dashuyun.cn/gtbmsyojbk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cqqwz.cn/gtfgrkmasy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.mhx1999.top/gteuyugfzn.html

[N04] 斐波那契数列
来源：http://hz.andypj.xyz/gtetggeljd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtmqjwcner.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aibaodan.cn/gttzvonnby.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtzfadqjfw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gteewujtzz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigfzy.top/gtbqosltbp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.guowangkeji.top/gtxgvlrnud.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtgegfoduh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtpoczhuaw.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtygyxsizm.html

Py:   math.gcd(a, b)
来源：http://hz.guannengcc.top/gtcahmiezj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.havefunace.top/gtikwpyomk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.316326.xyz/gtwmmevczb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtvprnnnmu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gtuykfklxy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ivvv.top/gtvlerslob.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtxqscgfnz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hnqzz.top/gtrxbtfdjv.html

[N06] 判断回文字符串
来源：http://hz.xinyue.icu/gtgdkvzefy.html

Py:   s == s[::-1]
来源：http://hz.haohaochexian.top/gtsjhqmvcf.html

PHP:  $s === strrev($s);
来源：http://hz.xuanzx.com/gtwiyazbdl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtwxvsbpeg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtzpdsllny.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangshuangyany.cn/gtwmluobcy.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigfzy.top/gtogrouvms.html

Ruby: s == s.reverse
来源：http://hz.cqqwz.cn/gtduzbwyyu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtzbacbpwr.html

[N07] 两数之和（返回下标）
来源：http://hz.zhaomingkeji.xyz/gtnnfwwdzp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinyuanbaomall.cn/gtvgmerhqa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cqqwz.cn/gtfcbzoync.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nwbrower.top/gttajckhaw.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhoulong.xyz/gtlsyzvowh.html

Java: // 手写 HashMap
来源：http://hz.chenjidiqi.icu/gtlxfcjjae.html

Go:   // 手写 map[int]int
来源：http://hz.gzhubu.top/gtvtxelgwb.html

Ruby: // 手写 Hash
来源：http://hz.fzhhl.top/gtdwurjbfc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aibaodan.cn/gtvroiecpp.html

[N08] 生成全排列
来源：http://hz.nanxinkj.top/gtrplaoieu.html

Py:   itertools.permutations(arr)
来源：http://hz.meibo888.top/gtpzdhxfss.html

PHP:  // 手写递归交换
来源：http://hz.yuanzhike.top/gtqppvcgca.html

JS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtkwxanvzd.html

TS:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtdkbbergd.html

Java: // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtpiwzviqv.html

Go:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtuablqnss.html

Ruby: arr.permutation.to_a
来源：http://hz.smart0.xyz/gtgznnzehg.html

C#:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtluqkwmrs.html

[N09] 栈与队列
来源：http://hz.andypj.xyz/gtgjwrczag.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.svipenyu.cn/gtvegxvizo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuanzx.com/gtbfrpkxzq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jyoumei.cn/gthtecvzzq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.kuanghao11.cn/gtgxrwtlgw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtnuqjxfgp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sysykeji.top/gtrjxoreyz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pycfn.com/gtpjhnunir.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xziqi.cn/gtxgryyozv.html

[N10] 链表节点定义
来源：http://hz.jinyuanbaomall.cn/gtfpgnskjo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xingfuxueyuan.xyz/gtlhcdlyzr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.0kj1m.cn/gtrqymyxxf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhixingplan.top/gtfqpnehdj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shuidangran.top/gttxrppuhp.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gtropxsczx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhoulong.xyz/gthiaiifra.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guannengcc.top/gtmilvtiwc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenjidiqi.icu/gtcdqcmlkf.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtxdvjnomv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yangfankeji.com/gtogffagqg.html

PHP:  // 手写递归函数
来源：http://hz.cashguo.top/gtkkdusrxl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhiwuduotai.top/gtfommjdli.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangtech.top/gtulnidcsg.html

Java: // 手写递归
来源：http://hz.ppjwa.cn/gtmjbyyqju.html

Go:   // 手写递归
来源：http://hz.c1oappe.top/gtwrxorbno.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtcsjkmqws.html

C#:   // 手写递归
来源：http://hz.gaohongyu789.top/gtqcxcltjb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgfzy.top/gtblmvpjpk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fzhhl.top/gtvzklawkx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhixingplan.top/gtzbcmtrmp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtwsbkikvb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtbtgwadxl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxuanxn.top/gtctesuuou.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtehjxgqfj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yanxiufei.cn/gtpmkelvao.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtikeiebtk.html

================================================================================
来源：http://hz.c1oappe.top/gtszzspnqh.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtvenvekuv.html

================================================================================
来源：http://hz.zhixingplan.top/gtpzbiauxm.html

[O01] 启动一个线程
来源：http://hz.svipenyu.cn/gtxtqwcjab.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenzaomai.com/gtmemdnazz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxuanxn.top/gtohdestrp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gticflfkzj.html

TS:   // 同 JS
来源：http://hz.hongshengwenyu.top/gthtlhxsad.html

Java: new Thread(() -> f()).start()
来源：http://hz.dianchejie.cn/gthvwqhczp.html

Go:   go f()
来源：http://hz.ydzc1.top/gtdzomhhhi.html

Ruby: Thread.new { f }
来源：http://hz.jqgufenzy.top/gtxrirhfvr.html

C#:   Task.Run(() => F());
来源：http://hz.smart0.xyz/gtltvmwivw.html

[O02] 使用线程池
来源：http://hz.chenlongwang.top/gtrhtxzdld.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.fengsongda.top/gtpilfamlc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.haohaochexian.top/gtevlylsah.html

JS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gtgrfsylos.html

TS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtmhgzkcce.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xinyue.icu/gtrcpnnxcc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenjidiqi.icu/gtaanstftf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jlsjyb.cn/gtlrjztcgl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jqgfzy.top/gtfhxdkqst.html

[O03] 加锁保护共享数据
来源：http://hz.zhaomingkeji.xyz/gtzkgjepqv.html

Py:   with lock: shared += 1
来源：http://hz.ydzc1.top/gtptwpoxij.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sweek.top/gtsjlrfycv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.9152youxi.cn/gtwbmfyscy.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtbhjciwjc.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtxdiqsajn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cashguo.top/gtgulincda.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xinyue.icu/gtfafikhob.html

C#:   lock (gate) { shared++; }
来源：http://hz.jlsjyb.cn/gtxhpclvgb.html

[O04] 定义异步函数并等待
来源：http://hz.shuidangran.top/gtyttuiwmy.html

Py:   async def f():⏎    await g()
来源：http://hz.birdmap.top/gtwgpvosgw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenjidiqi.icu/gtsvwkrrjh.html

JS:   async function f() { await g(); }
来源：http://hz.bjfxy.top/gtpsobfvou.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.0kj1m.cn/gtowswavae.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnxiangtu.top/gttqraczzj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cashguo.top/gthqclpxsa.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.0kj1m.cn/gtebbcbwmv.html

C#:   async Task F() { await G(); }
来源：http://hz.jiagoushi.top/gttytmvzvw.html

[O05] 并发执行并等待全部完成
来源：http://hz.cqqwz.cn/gtzxwvlsfj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhiwuduotai.top/gtugckqwrc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgufenzy.top/gtsnhntojz.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtoyspmogi.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtmstbcgsw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.daria6918.cn/gtvsgifdtt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jlsjyb.cn/gtuzluccbd.html

Ruby: threads.map(&:join)
来源：http://hz.hfpthk.cn/gtlcfspieh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gogol.net.cn/gtnrzovqqt.html

[O06] 使用进程池
来源：http://hz.quarkkingdee.top/gtadggjhhr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.vqdsnc.cn/gtphrnbxrg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cqqwz.cn/gtvqqrmnau.html

JS:   // child_process / cluster 模块
来源：http://hz.zhengqikj.top/gtmskdwahc.html

TS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtksxzickj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtuamtrwvw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fengsongda.top/gtzqdhvbdq.html

Ruby: // fork 块
来源：http://hz.jinghuilouyu.cn/gtazqdtzou.html

C#:   Parallel.For
来源：http://hz.zhongyouzk.top/gtoalussjp.html

================================================================================
来源：http://hz.quarkkingdee.top/gtcibxbfqr.html

P. 常用工具函数
来源：http://hz.hfpthk.cn/gtgmytkknw.html

================================================================================
来源：http://hz.ybcxt.top/gtzcuirngb.html

[P01] 生成 UUID
来源：http://hz.jqgufenzy.top/gtvvvnenej.html

Py:   str(uuid.uuid4())
来源：http://hz.cheryme.top/gtcvpvukxw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj202588.top/gtgnvanpaj.html

JS:   crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtizemkjxn.html

TS:   crypto.randomUUID()
来源：http://hz.zycfv.cn/gtdmyaobyy.html

Java: UUID.randomUUID().toString()
来源：http://hz.andypj.xyz/gtstxmmzap.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtunzrbttr.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigufen.top/gtvpwbufmf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hfpthk.cn/gtdyuunwfv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xingfuxueyuan.xyz/gtisndbhfn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cdnleiting.top/gtsxmfqtvm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shzxlz.cn/gtdiftupui.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.aizwys.cn/gtnvxjcekw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cdnleiting.top/gthctpvjrh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.birdmap.top/gtvbxegxxr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shzxlz.cn/gtobfustny.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigfzy.top/gtwopwwcci.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuxming.cn/gtccrppoqo.html

[P03] 生成短随机字符串
来源：http://hz.chenlongwang.top/gtuofwquvw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgfzy.top/gtsqzvpexn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.0kj1m.cn/gtayojqddg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtmfeomsdg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtvpsacgbg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.0kj1m.cn/gtrjrlwsgj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.haohaochexian.top/gtlovoyvoc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtkawargte.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fengsongda.top/gtpyombjci.html

[P04] 求长度
来源：http://hz.yj20258.top/gtoechncip.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zycfv.cn/gtumueuqgz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtwgccvrfm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuetiantiany.cn/gtfjvjcbcm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gtbaagierx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jiagoushi.top/gtelviapdg.html

Go:   len(arr);  len(m)
来源：http://hz.gogol.net.cn/gtkcrxynuh.html

Ruby: x.length;  x.size
来源：http://hz.jyoumei.cn/gtucyfuxik.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hysaishi.cn/gtairarbch.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aizwys.cn/gtrgqarkbl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ybcxt.top/gtpiwpvzsj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jiagoushi.top/gtxhyyhsnt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangshuangyany.cn/gtppbgfrnk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gthxkfsczr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigufen.top/gtrcgzqate.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gtfgskahzf.html

Ruby: a == b
来源：http://hz.yuanzhike.top/gtitgxgxqz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yvedp.cn/gtjwoujyul.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gotoacloud.top/gtclikmuid.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhongyouzk.top/gtvsmnatdd.html

PHP:  if (empty($x)) {}
来源：http://hz.tanke756.top/gtlpwlsnpa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gzhubu.top/gtjccbofte.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtaklpvpud.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtdtzridbw.html

Go:   if x == nil {}
来源：http://hz.chenzaomai.com/gttctxjvkq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yongpay.top/gtuxmnypze.html

C#:   if (x is null) {}
来源：http://hz.yuanzhike.top/gtuqdnpaki.html

[P07] 防抖与节流
来源：http://hz.mhx1999.top/gtkzmulbph.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.vqdsnc.cn/gtlgnwufea.html

PHP:  // 手写时间戳比较
来源：http://hz.vqdsnc.cn/gtsqkghexo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gttxmlqnbs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtcivsvsdj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhengqikj.top/gtfuhdgxfx.html


<!-- 参考信息 -->