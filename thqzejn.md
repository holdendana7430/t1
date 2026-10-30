代发 wailian999

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gcroxurim.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gtgzqymde.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gwmlyvuni.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gkrrukkfi.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gwcxujltb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gujcadpak.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gjwolmzes.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gzojtrodc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gmpbghgke.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ggwpxxpic.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gnlshoahs.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gdrenprss.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gtjjzpydp.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gtfmazjxn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gplgmelys.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gahcborlf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gkioqivwv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gxiafqjug.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gpwqzgryx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gmkdyfyup.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/ghbmiqshz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/giwjwlytp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/ggczurnfg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gkwahsjor.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/ghdnkgffn.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gxyjwdhyd.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gosubnwpa.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gqpmgcvai.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gjprlhigg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gqslkzxnl.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gusvpclpu.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gjdapohfo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gzkuvuatu.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/ggvjdweag.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gvjbbggly.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gjutahzwo.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gnionuqoq.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gyvgyasjb.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggbnukjso.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gancdtszt.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gewdfycgg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gwuoymiga.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gteldqpwx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gtyiitflc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gabvqgkww.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvbbwimvj.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/geefsxpgu.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gmlpwrwhu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gvakvkoqq.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gbpdqwapi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gywbavcrr.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gddpshjrq.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gjmcnwceg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gcnqvriot.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gijrkztkx.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/givdltrbq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/ghsydwpck.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gqbqgbrmq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gweeednri.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gjxzhdnyc.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gtfnlzkre.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gczkiyoog.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gatzbxwcr.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gfbddbqmu.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gcyaezdti.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gnrrhiiyt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gxwzpvvwq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/grdterfom.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gogjaohlr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqsbgybbd.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gstrdavio.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guqpmiqnt.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gzuyjpnxd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtrfjbcby.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gytzogpwg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gfjzzwyzv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gmcmamhcr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gcdliaybi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghikpvrsm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gwmmugmdl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gelpxgxmi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gegkijyuc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gektaauxk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/grzfabnjt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gtujjdlag.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/goebhvcjx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/ghtuonfjt.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyilclqmd.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gzynknumw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gmbjtkdqf.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gtqqchadi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/ggshbzpuz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gobefocet.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gstebluzy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gmugehnpq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/ggficljyc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gquhgyilg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gpwlecgdh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gtaeztahe.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gtepwqxua.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gqnroavdp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gijmvewwd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gxyeutdjj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gsprkhhkh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyhoaoad.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/ggrwqjfai.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcpcciicz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkxyhxveo.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gazhjqgbw.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gjuvfdfzl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gpugcddwk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/geucxpxfn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/geouoozti.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gdlfmhaem.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gxyljfbxv.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gxyiauidi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gvfllmija.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gqxjniqvu.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gijtgxzzk.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gvrsomldw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqiefmwyf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gwzkmxphn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gmtjpotxu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/ggarwytuo.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gjwcfgnzt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gdatuevbh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/grvflwsrb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gtqywkxll.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gfydhjxwa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/ggyaehbfz.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/ghnaiplib.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gwuguipyf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gubxrrvmu.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gozdxuxfd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gdsswqogk.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gopijqncu.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gjwlkzzzd.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gijrnzmwd.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/guxsqrumu.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gfjpvkvvi.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gxxaolwgq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvkmtrfiq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gqqsmlfdj.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gyrneiswp.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gevdmbgng.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gmfuwyneq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghigpusvf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gbunflfop.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gwystcvgx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/ghbpuqgfh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/ghkxvlkpg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gumshupvj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gkbfmgggf.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gascgmhbj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gfwauvtfy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/goxyoojfi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gswrfqqgj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gylctogre.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gpiyfzsau.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gzvjkwmcj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/groblnxqu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gzdqtopaq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gweeotkzv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/ghjfbbzna.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gbdfjodkl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gvqpauhfz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/givqstvgq.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpimenkqe.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gbgkkcsfw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gqczqyinv.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/griemthwq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gegusxkwz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gllbitzpu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gxpuovytu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/goinooafc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/glauvblda.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gayexzadn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gzvrpamfu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gyqmrhbtb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/ggcdwmlnv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gopaggajt.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gfmbcmfvm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyaxosmdp.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gmmqtkzvj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/grinrkcjr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/glswkinqr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gmpxpzguh.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/geelphwof.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/glnbhjoqs.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gbhktamhm.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gegtswofc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/glmeciato.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gwcjaymjq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gwcinwiao.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gwedqbsde.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ghmqwgrow.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gxrybgwxj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gemwjmkgg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gfrbbghyf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gwscvsumn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gcnxdaieu.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gwiaptngs.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gfmvfgjsy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/guwpzekio.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gfsciszga.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gcvromham.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gfflrisqa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/glbwsvrcb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gojrqapyh.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gjyejnnue.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gcpeevwzj.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gvfryevyt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/govasyzmo.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gecrkeopv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gdarqftbh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gmdcqxodm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gjxixhtxv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gxgazkmdy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gxumcpoze.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gwzecvlwx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/ghrrazzqi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gvjvjqxfc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gwmqxzuoh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gelcfhtrq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gmoqebohj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/guihwctzy.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gukkfjbyv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gqcjleobd.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gplvtaneh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gjcjyrdiq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/grsblszbz.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gkzhoxilw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gjwtaeexh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/ghxzlmpbt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gjbrglqev.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gkbbfmlzt.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gzpkhdcpx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqtwxyoby.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gwuqilbch.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnfhtxukg.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gmptxqrnf.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gyvrirtwo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gipjmlduq.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gzaypbcqi.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gbdcagcad.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gyvrnmnwa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gvygvmrsv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/geqkxtqoe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gngfjsudx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/glyzizuto.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gbettzhdi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsooqbaoy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gkbrtyhvi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gaboxpufi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gigeawtnd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/giibjtuuu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gitpntsrq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gqxkuhcqr.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gniyowkma.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/ghwmtxboa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/guyinmtjf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmtijnlx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gfuwseojy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gepjpqfbx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/ggfrmfkca.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/ghuskjncw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gvfkijoty.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gnaohgtvt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/ginfrgsai.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjavhymdf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gtewgfijj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gaeuzoshb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gwrunbxwm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gsfytyqey.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/ghnuztxcf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gvkflmrpl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gnqfmytnt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gqzhvwtpk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/ggoxzsyff.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gengpxnhk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gwxpbexmb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gbfwemodp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gazsezwlx.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gifsoogxt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gwggrpasi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gvxzwnyia.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gujsxnrny.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/glmwyaedd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/garalzpzp.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gayespscx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gymemfuvy.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghdasowha.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gznbbplhk.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/guvfsrjwd.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gcalganiy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gfboirhgh.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gslnrnfet.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gpgvzduqg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gpwosqdvl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gnyjjgach.sHtML


<!-- 参考信息 -->