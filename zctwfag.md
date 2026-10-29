代发 wailian999

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/goyegumrj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ggstfefyd.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gelbvmrsn.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gkoduyrom.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/ghndgajnx.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gzzjomqyh.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gjjjfjbwz.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/grhlkwanv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gnxhcueaf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gfbkkauac.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ggihfklcu.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gqsnuyzki.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gkagnyvxk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gdcuabodc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gcaklrbgn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gbuitezii.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gdbwzzlzt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/ghshcgbpp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gcakbzgll.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gjjzyavlt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gibpottvo.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/grrbufimf.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gyrzuwgmg.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gdqlokbth.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gjkvkoybz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gelksrjau.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/geqtpiwiz.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gxnwjetfy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gfeurpacl.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/guripmrgc.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnrrfkjet.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gekvzrjxe.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/giwenfidv.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gjqsadmaj.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gugbnnzmp.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gcousezwg.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gdrkrvzyi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gcgnxcpjl.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gjnpagswv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gzhhghsfn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gqvmvosla.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ghsjrikra.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/glxceqxyo.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gmpgdcmps.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gnpgtumtx.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gkvlezfet.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gqbrqsgyz.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gwosmbubf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/glghurthw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gmqeizhlk.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gplzdzpvw.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gefdgksav.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gcunnhprp.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gtttalzyc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gfnfbxyzq.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gmkdvhbcy.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gqhfjtuag.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gwgprhgua.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gluxskdgt.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gzevkxxad.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/getouuhyq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gqyagliso.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gaqyonmqs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gywrszzob.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gxhwiazwj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grzgiabxm.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gytedyquv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gildipqog.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gdxlwvkfg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gqkwqdccj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gdxmtqqwu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gpmgnhvvu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gpfgdsvai.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkrtikbrh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqnpexfmx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gjgokriug.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gltceeala.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gwshacmkx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gtvwlpxii.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gohwrslrh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gvvpzrqxn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gofuwzcwn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gediaxevy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkjtojawf.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gpwrjzpjq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/ghakahksx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gdtsevogl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/guraujmvg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gmvjzoejy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gnlubrgkm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gjgatyjeo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gybnrtfom.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/glpmysuon.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gvntgjohn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gxuhopbpv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gqdlekwfw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ghulsynrv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzxohrnt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gdavctiof.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gxbseqhfh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gftspigjx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gecarvnmj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gztsgarjh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gqqvrxszj.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/geninaqtq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxhbvtcvf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gqslqvxsl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/ggbtqcmsn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gojjuxzmn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gniafwdht.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gsdeengqe.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gnaovdqzn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gwcwnplga.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gzvthctsy.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gaypmzmff.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbbhkykji.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gluwmeqtc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gsylvvoti.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gmdildusf.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gwjirdefm.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/govprjrlh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gmwlpqboe.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gyismqsha.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/grumbvjeg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/ggkjaqllj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/golgfqbyq.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gfbzdiveu.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gzyyhgkmv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gtgwxudoz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gomnzziij.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gonlvxpil.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gudttetli.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/ggezwhqtw.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gxdhptfzt.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gpeuyjwpv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gacxigxck.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glnezqbdf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ghoucqmcs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gzqoyysal.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gmczeuyob.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gnlxadshi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gjnfkjoiz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gqezgwqnb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/giaauxupj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/giyzfhqzx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/golotcxwm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/godjcxsos.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gdmgjvsho.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gzozwfsed.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gdslgjumn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gplisgvpy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gkmwrlbrj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gvbwpozcr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gtpchdeol.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gknsfaiwk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gkiqxdccd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gqiyvlokm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gklgoqkrt.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gjaajselg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/grdbjctic.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gmxgaayvl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gojxyxbxe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gvhmrejfx.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gozxvdorx.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gzvmxiihj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gbrtcewci.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gjnctscwn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gxouifaap.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/ghhlwgabp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/ggcfouyuv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/grzjsgayf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gzayydoyd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gnwzqoupk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gczotjeww.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gyrxychfo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gkjmuoliu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwoyqkwzr.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gxhiqxhbf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gudecafgj.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gurvsgibl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gzcnhpamf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gaxjscowf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gftnltilt.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gyffxxonu.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/geslgihom.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gzrqxsdez.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gokvvfpfn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/grtpgnuwk.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gpibxuckg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gmouhjifq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gfposmdfs.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gzsjfwjma.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gzdmmaxal.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gwemjswie.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gdnbbixof.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gxxvohnlm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gedwpspdv.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gxxnvksnc.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gbbwwmfzn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gegculavk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/ggakfhhxk.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gcjipgiij.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gtrcbrefu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gqhwtbkzb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/grygyshnr.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gbdlvwcmw.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gdalmjtpg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gdfpfaend.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/giklfwwpn.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gxwabrkgu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwyvuiwgo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gespfosjf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gtdtruzvo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/glgjwkyku.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gvarvobhy.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gcupktjev.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gxajiqene.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gdkfpbzzu.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gcbgefzpj.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gbrnjntpz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/glfpkpsdq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/glrcfriqu.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gfgrnsbnn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gnfjnjulr.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gwfxfxgvw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gcuppthdv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gkbksboyv.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gaojwzeiw.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gqafrkfst.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/giqwnlmyp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/giocybzuj.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gznseyscn.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gxhwlhcwi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/galxvuxrs.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/ggxbsvofq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gszradvqn.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gstwcthyl.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gftknkwkh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gzygveykr.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gmsasqvcu.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ggksphbom.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gvzaabbrx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gxxqquxhf.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gefscrwai.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/giaapjaas.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/goaadsybk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gooqbtqns.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gturxneir.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gkiouublp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/ggxzvyjvq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gzthyxsyi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gwezpqpvr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjjroisez.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gnppkvoeq.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gzmddnhzh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gpgcdlofu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gcfrajcen.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gfikoloeq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gpeuyvqoh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gjfuvvaox.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gerpppfen.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gkprdyudi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gihkajlay.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gdpvkslyb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gapvmdkop.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ggbouiylo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gklmvxzbq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gksytbaiq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gsrwdpnvj.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gkqgqdmks.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gpmjukdjt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/ghlnamrwr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/giezrfpal.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gbuwvgjwc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gvlzwjgrj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gnrnhrzgg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gfvjvogrr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gngdqxirc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gnvqcfzma.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/ggvrvjyxg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gsfgfhtkv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/geibyyvqh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gqglyqkaw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gzyrqzbzg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gymundove.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gqcznvqoa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/ggqimkyfr.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gwnicwxjw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gxpceeilm.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gvryrrerf.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gsqixucon.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gxhhsrijx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gwimwxmlo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gqiwwmidp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gxojanbaw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gjvgipsqm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gloyerqar.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gsiaxpdjy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gbcnthsqu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gpzmadhhb.sHtML


<!-- 参考信息 -->