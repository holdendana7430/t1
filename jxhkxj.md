代发 wailian999

================================================================================
来源：http://hz.0kj1m.cn/gtbquedcbq.html

[M01] 读取命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtsathvazm.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtxqtqajsi.html

PHP:  $argv;  $argc;
来源：http://hz.ehwqpu.com/gttrlpzqhy.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtrskyorxd.html

TS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gttjzinidt.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtvatlysju.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtscwrrbls.html

Ruby: ARGV
来源：http://hz.hammf.cn/gtseprtvdl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hammf.cn/gtldwkxjbe.html

[M02] 读取环境变量
来源：http://hz.jlsjyb.cn/gtazzpqyot.html

Py:   os.environ.get("HOME")
来源：http://hz.zhengqikj.top/gtabpdceke.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.9152youxi.cn/gtxmayguhr.html

JS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gticqdwtqe.html

TS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtzcmrogql.html

Java: System.getenv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtjkcfertc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gotoacloud.top/gtrluwndyr.html

Ruby: ENV["HOME"]
来源：http://hz.chenjidiqi.icu/gtypzzjxmw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ywan-chungtsiang.top/gtcesqtvqz.html

[M03] 执行外部命令
来源：http://hz.chenzaomai.com/gthpexemoe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinyuanbaomall.cn/gtokgswibz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gtockuwnyn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtwucsyueu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtsuhwprte.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yonumen.top/gtwrqfreis.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtwtfvvjos.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.316326.xyz/gtafpvzvha.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gtllujaxbn.html

[M04] 获取当前工作目录
来源：http://hz.ehwqpu.com/gtlqzwrqbl.html

Py:   os.getcwd()
来源：http://hz.bjfxy.top/gtpzkuwvfh.html

PHP:  getcwd();
来源：http://hz.aibaodan.cn/gtoxeavgif.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtystggmac.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtkncjduhk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.andypj.xyz/gtyjdkbhxv.html

Go:   os.Getwd()
来源：http://hz.ywan-chungtsiang.top/gtipvddcyd.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gtxusxemik.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zycfv.cn/gtqlpwpqil.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtiensiqtx.html

Py:   sys.exit(1)
来源：http://hz.meibo888.top/gtzrlzinac.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtnxyfvsdr.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtzfngqkyz.html

TS:   process.exit(1)
来源：http://hz.cucudq.cn/gtgfdqtkzk.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtyeuliejl.html

Go:   os.Exit(1)
来源：http://hz.ydjk.org.cn/gthcrmmfom.html

Ruby: exit 1
来源：http://hz.tianlin.xyz/gtvwcrwiaf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.havefunace.top/gtnlvuetaw.html

[M06] 向标准错误输出
来源：http://hz.ppjwa.cn/gtnsxhwjmz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtxspikxdh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ehwqpu.com/gtpzptmaun.html

JS:   console.error("err")
来源：http://hz.ehwqpu.com/gtxnutejpk.html

TS:   console.error("err")
来源：http://hz.gzhubu.top/gtixxgskfo.html

Java: System.err.println("err")
来源：http://hz.316326.xyz/gtdqhprbjo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hywenlv.cn/gtfadjqgff.html

Ruby: warn "err"
来源：http://hz.jiagoushi.top/gtdrqybpat.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.havefunace.top/gtgtxmvxwo.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtgsgnpsih.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtiwkvodyo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuanzx.com/gtvuqrulfk.html

JS:   require.main === module
来源：http://hz.gaohongyu789.top/gtoygpstlu.html

TS:   require.main === module
来源：http://hz.jyoumei.cn/gtypjxovno.html

Java: public static void main(String[] args)
来源：http://hz.jiagoushi.top/gtkyyfroxt.html

Go:   func main()
来源：http://hz.gaohongyu789.top/gtgxtgjmzs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gthqjljvew.html

C#:   static void Main(string[] args)
来源：http://hz.ydjk.org.cn/gtoskahlnh.html

[M08] 获取系统与运行时信息
来源：http://hz.tanke756.top/gtrrvjrrcy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fzhhl.top/gtrnurtjvr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj202588.top/gtdbksjtga.html

JS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtjqilslta.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtlupuaijc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yongpay.top/gtowdrbirv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shuidangran.top/gtcqchqixg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangdashe.top/gtyoywyqii.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gtwlhesqnl.html

================================================================================
来源：http://hz.guannengcc.top/gtmcjtckvx.html

N. 数据结构与算法
来源：http://hz.pengpengdd.cyou/gtfrlkmeya.html

================================================================================
来源：http://hz.zycfv.cn/gtsbskwoxr.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtegxzxkxb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sysykeji.top/gtwbvugmsw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtulxgoieb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtvzvdflfo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtfbptwxem.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtwyzjmrhn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuanzhike.top/gtiuzsymmc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtsvvarkzt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gtssmdglgd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hywenlv.cn/gtcymslgpz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtiraaglbd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cqqwz.cn/gtnggifdqt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gtdtvsbabb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtgmuoemqv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tanke756.top/gtoqrknfku.html

Go:   slices.Sort(arr)
来源：http://hz.ybcxt.top/gtdlejkfks.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtewpjnuyh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sxryk.cn/gttpvptoci.html

[N03] 快速排序（分治示例）
来源：http://hz.cheryme.top/gtzbyytzgc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtpeuughit.html

PHP:  // 递归实现，或用 usort
来源：http://hz.iojbl.cn/gtmmeqyyby.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gtctsmwuny.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtxnjckopz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yanxiufei.cn/gtkufddnez.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tian-w.cn/gtasvpfyyr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cucudq.cn/gtyurrnygz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fzhhl.top/gtosqmlpgk.html

[N04] 斐波那契数列
来源：http://hz.zhiwuduotai.top/gtqlsiscrr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtvjzlhgpn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.316326.xyz/gtbkkpnyhd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtdfeubjar.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtzbperjsl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ivvv.top/gtqjildltj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daria6918.cn/gtrushdqjo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtaakweskn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtgjtgpskt.html

[N05] 最大公约数
来源：http://hz.snrcjt.cn/gtytuqpunb.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gttiminwab.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yueranfly.top/gtfptbeyyc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtcjarpbfj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtqmxgpzga.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gthgifajrk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.havefunace.top/gtlsuidoxs.html

Ruby: a.gcd(b)
来源：http://hz.bjfxy.top/gtbdeyhigm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.fengsongda.top/gttghxlphr.html

[N06] 判断回文字符串
来源：http://hz.zhaomingkeji.xyz/gtwagusndi.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtjcdwlgyf.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtadnrldyy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtyumvhwzg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtovkwdiat.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guowangkeji.top/gtlmrhaoeg.html

Go:   // 双指针从两端比较
来源：http://hz.chenlongwang.top/gtgmijdcqi.html

Ruby: s == s.reverse
来源：http://hz.yuxming.cn/gtznpvmiuf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydjk.org.cn/gtrjhsllzi.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigufen.top/gtmvirdbbs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dianchejie.cn/gtjocpmehk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.haohaochexian.top/gtoynonjil.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yanxiufei.cn/gteqndkhed.html

TS:   // 手写 Map<string, number>
来源：http://hz.yanxiufei.cn/gtxlwcmfjt.html

Java: // 手写 HashMap
来源：http://hz.yueranfly.top/gtrdiwgial.html

Go:   // 手写 map[int]int
来源：http://hz.hysaishi.cn/gttlbdtxoy.html

Ruby: // 手写 Hash
来源：http://hz.yuxming.cn/gtqecfajiu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxinkj.top/gtepmlydbs.html

[N08] 生成全排列
来源：http://hz.c1oappe.top/gtpuwsmttf.html

Py:   itertools.permutations(arr)
来源：http://hz.daria6918.cn/gtdgvjzldd.html

PHP:  // 手写递归交换
来源：http://hz.daria6918.cn/gtcsgplhta.html

JS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtkbthpoxi.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtvravrnyd.html

Java: // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtcriybcdl.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtqfriitnx.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258.top/gtjjusbhcp.html

C#:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtmrjbsznz.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gtyrmxppsq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj202588.top/gttkxqduju.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.feifeiyinyue.top/gtsgpbpyxb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtyzjaxamt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xylfe.cn/gtwnzmjmes.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daria6918.cn/gtmssctgcs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dianchejie.cn/gtnnihuptb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtmamojpsn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.haohaochexian.top/gtbfuoffbk.html

[N10] 链表节点定义
来源：http://hz.yangfankeji.com/gtjgnkrqxv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.9152youxi.cn/gtggydtyji.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuetiantiany.cn/gtyjyqkdli.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigfzy.top/gtroluzrki.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gtggrbcpge.html

Java: class Node { int v; Node next; }
来源：http://hz.zhoulong.xyz/gtyylhyioq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hfpthk.cn/gtbyzgcrxp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gtpnoyrbip.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aibaodan.cn/gtobpizwdu.html

[N11] 二叉树中序遍历
来源：http://hz.zhengqikj.top/gturtoimov.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aizwys.cn/gtlvdacxby.html

PHP:  // 手写递归函数
来源：http://hz.tianlin.xyz/gtgavlglyr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gtinrmxbah.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtenosgwtx.html

Java: // 手写递归
来源：http://hz.feifeiyinyue.top/gtsvvbexsj.html

Go:   // 手写递归
来源：http://hz.yongpay.top/gtztyanezv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gttdqrgzbk.html

C#:   // 手写递归
来源：http://hz.jqgfzy.top/gtloffrsgd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tanke756.top/gtipywgjsf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigfzy.top/gtmcsvrwiz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sweek.top/gtuxirqmed.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtmmoknfbw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtmjcniecu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtnwxpeyig.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.quarkkingdee.top/gtfutdjpwj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinyuanbaomall.cn/gtzcikaxrk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtporxmyvj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtftnlujdx.html

O. 并发与异步
来源：http://hz.yuxming.cn/gtrymhxxcl.html

================================================================================
来源：http://hz.xinyue.icu/gtkmmyxith.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gtrspnuvmk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.iojbl.cn/gtclguboff.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jqgfzy.top/gtrahjeeec.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tanke756.top/gtdnrztdxd.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gtksscrqmn.html

Java: new Thread(() -> f()).start()
来源：http://hz.tian-w.cn/gtuygehurq.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtbseqzkkg.html

Ruby: Thread.new { f }
来源：http://hz.daria6918.cn/gtgcpohiaa.html

C#:   Task.Run(() => F());
来源：http://hz.hywenlv.cn/gtsopjufct.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gttylpvccx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cheryme.top/gtdcnjhtam.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigufen.top/gtxtrzxasl.html

JS:   // worker_threads 线程池
来源：http://hz.52xcode.cn/gtbvxwoklp.html

TS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtlmeucahq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangkeji.top/gtmzyyllsg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtylylnopw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhixingplan.top/gtqwuvzeyf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gtvvxujvbw.html

[O03] 加锁保护共享数据
来源：http://hz.hysaishi.cn/gtfgwebpwy.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtvzqhalvz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenzaomai.com/gtikjgggmp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj20258.top/gtkcgvznkp.html

TS:   // 同 JS
来源：http://hz.ppjwa.cn/gtjawubnck.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenzaomai.com/gtwbeupewf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuanzx.com/gtpyejuikr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj202588.top/gtcizapvru.html

C#:   lock (gate) { shared++; }
来源：http://hz.zdqjudy.top/gtagzfgctk.html

[O04] 定义异步函数并等待
来源：http://hz.ydzc1.top/gthrenplsf.html

Py:   async def f():⏎    await g()
来源：http://hz.hfpthk.cn/gtfxdikqgp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daria6918.cn/gtfdhiufna.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtycvsusmw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuanzhike.top/gtlmrfurth.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daria6918.cn/gtwfxfaccs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yueranfly.top/gtsefcaftk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.andypj.xyz/gtpawochum.html

C#:   async Task F() { await G(); }
来源：http://hz.yj20258.top/gtjwlqqnjj.html

[O05] 并发执行并等待全部完成
来源：http://hz.svipenyu.cn/gtebrafbzq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gogol.net.cn/gtqrldspbe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sweek.top/gtholibigd.html

JS:   await Promise.all(tasks)
来源：http://hz.pengpengdd.cyou/gtxqubtqyj.html

TS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gtxmqtcsxv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtmdsnofog.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jiagoushi.top/gtucqdcskb.html

Ruby: threads.map(&:join)
来源：http://hz.yvedp.cn/gtnkyogpcj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigfzy.top/gtbrjpwipx.html

[O06] 使用进程池
来源：http://hz.sufxvd.cn/gtxjvuebsh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shzxlz.cn/gtlsmxfvsl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cheryme.top/gtddpridca.html

JS:   // child_process / cluster 模块
来源：http://hz.vqdsnc.cn/gtqbpcqugu.html

TS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gtzcglifhz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yangfankeji.com/gtlgbjnsrv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinghuilouyu.cn/gttbbqzgro.html

Ruby: // fork 块
来源：http://hz.ydzc1.top/gtpamnnqez.html

C#:   Parallel.For
来源：http://hz.iojbl.cn/gtubzpzapg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwucdevno.html

P. 常用工具函数
来源：http://hz.jinyuanbaomall.cn/gtwxtielfm.html

================================================================================
来源：http://hz.yuanzhike.top/gteldhlqck.html

[P01] 生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtzwaeyeec.html

Py:   str(uuid.uuid4())
来源：http://hz.chenzaomai.com/gtmanfnszq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nwbrower.top/gtukjlecnx.html

JS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gtuzqtqauv.html

TS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtqnizgedu.html

Java: UUID.randomUUID().toString()
来源：http://hz.havefunace.top/gtvlorwtqz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gtdaeyymnf.html

Ruby: SecureRandom.uuid
来源：http://hz.sxryk.cn/gtfsmncrco.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.316326.xyz/gtcvrkxyux.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtdflxxwrs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shzxlz.cn/gtpzjrfbme.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtxoandcmg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shzxlz.cn/gtrpljqpah.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hongshengwenyu.top/gtoyzyshgp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ivvv.top/gtmwluevlr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gtjswqexaw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jiagoushi.top/gtpiaqwxnn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.feifeiyinyue.top/gtylpfadui.html

[P03] 生成短随机字符串
来源：http://hz.zhaomingkeji.xyz/gtohdqooia.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.guannengcc.top/gtvnaamoqo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhixingplan.top/gthssimbkq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pengpengdd.cyou/gtzraffdju.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtptevwuen.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhiwuduotai.top/gtywcoizwk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinyuanbaomall.cn/gtyhbjmwqu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.316326.xyz/gtoxsolldm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangkeji.top/gtsczbzgoh.html

[P04] 求长度
来源：http://hz.jianghu66.top/gtvefnedkm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.mhx1999.top/gtmsekgohh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtzdezmzup.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtrppfiaon.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtxjxywsrm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daria6918.cn/gtjogacnve.html

Go:   len(arr);  len(m)
来源：http://hz.jqgufenzy.top/gtusvbyjpy.html

Ruby: x.length;  x.size
来源：http://hz.zhongyouzk.top/gtifzdeccq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhijiandao.cn/gtyerrjcyq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgufenzy.top/gtpikbxvjt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangshuangyany.cn/gtmewkslso.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.9152youxi.cn/gtjecxjgbc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgufenzy.top/gtkqbebrjx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhijiandao.cn/gteunculon.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jlsjyb.cn/gtbplmfkto.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yueranfly.top/gtibggyrmy.html

Ruby: a == b
来源：http://hz.yj20258888.top/gtebotcmrp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.0kj1m.cn/gtusazuzak.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.havefunace.top/gtgcyrmmeh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gotoacloud.top/gtztpiuhwd.html

PHP:  if (empty($x)) {}
来源：http://hz.sweek.top/gtseevlmel.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cdnleiting.top/gtwypzgucd.html

TS:   if (x == null) {}
来源：http://hz.cashguo.top/gtylanexvd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.mhx1999.top/gtfyzfwmvh.html

Go:   if x == nil {}
来源：http://hz.zdqjudy.top/gtiwdvcdpp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gtzffovsrv.html

C#:   if (x is null) {}
来源：http://hz.haohaochexian.top/gtpyamtlzx.html

[P07] 防抖与节流
来源：http://hz.yj20258888.top/gtvxgcswda.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.iojbl.cn/gttxapnlex.html


<!-- 参考信息 -->