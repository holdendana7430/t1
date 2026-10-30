代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gunynzxjx.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gweidmfgs.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gvqeuqfrm.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gbxejxbad.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gogqggjgp.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gwmwbxzwi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwwzwojph.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gvrnfqjnc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gqybunldn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gfoyfvppi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gxuitxroy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gzpewjyxu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/glikliqnu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gbqkguqgk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gqednuhnh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gdmrhyrkk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gfupdhurt.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gnlulmfio.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/genssklde.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/ghlqssfli.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gwmsrxubq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gdmpyezhg.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/glgqlnnvq.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gtmsnpzbv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gwyrpsckk.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gorxgcidy.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpqathhlg.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gqftrooiz.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gsswozjxw.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqjuslmhv.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gaampkvgk.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjvtipzom.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gsehjwijm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gdzpacyif.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gyazxpkzu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/ggocqsasf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/glbhjvfaf.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gdxtcoenp.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gnukirhyg.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gbdmuqjpi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gubuuucvd.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/grxzfcadz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/govrngbxm.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/ghkvqvmru.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gnuaofknx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/ggazpfdlu.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gjjwchohw.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gygvwfifk.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/grconrntd.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gngcquedf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gxkvqsgns.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gxojdsfyd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gxvdvqoyo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gtyodirwq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gyrvpcygz.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gvwelebdh.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gwgigxcpw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/grguqeafk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gixltgcux.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gbrbshkka.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gdzdvphph.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtlbapsmj.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gzpteqseb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghxvloujv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gtfojjrve.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwitzguds.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gczoquajl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gskeoljqm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gntmyzywv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gevgtqrrr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwdrdoshl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gttvkibhu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glwfdslpn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gcgifqpcx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/grorqrakf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/ggvcvprlq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gufpdnnrw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gelljaewe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gfxyzduzx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gcahlpdpt.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gxdckjwvd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gefzvgzsq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gwaaqqnpo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gogdxvbrc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gujgxprvy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gbhkhuefr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/goytnbvhs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gnsxbugdc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/grbfumfyt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gyljbkgss.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gdnybvpap.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gkqqtgwfc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvenrmtds.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gqhsvepax.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gzmdukwlu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gvtctdfuz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gtttfaqns.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gofoxpuzy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/ghxppsexw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gzyapggbo.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gmmkipaqu.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gyetriagj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gllwzcfpg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gqmnubkxy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gyhqvygvb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gxlhiaeiy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gpkvvepsn.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/glkvhvawp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gprxaxbeh.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gebrcuhfp.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gspjxggms.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gkrhhhhdh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gliyvwnjx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/groeteetl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gaamvgqux.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gsqozhurx.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gohieznei.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gdqrachte.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gkejmtexm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gojptusyp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/ghxkyhfsp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gfcalegtz.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/glnhrnyvf.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gbqhphwap.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gpyapmeat.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gjxleessw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gyuleggyy.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gkcxiqibm.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/glozzznig.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gkfnkibdv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gulvkoaqb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gurgblkou.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmxfrakjg.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwariglnc.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gpbcsqfyh.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gxpbfmbij.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gsthyicru.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gbucuvajf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsxmgppwq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gqrhwcxvc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gxmiieppa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghrgvsmwb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gdkqzjdrx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/goowmrqiq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gopvtdkxl.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gghnxoqlk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/grnxwawht.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gpskngudo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/ggboyfjge.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gzmpraxrr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gvmnmzgsj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gbhjwipqy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gdarbxckv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gqemcktjb.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gunkqmyhc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gwwefobpl.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gisqtullw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gubnmxivf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gcgzngnwv.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/giofblwou.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/guoaffqkp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gfqqhaaae.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwhawzlln.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gascuqcsm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/glgxdzdut.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gquxnjcfi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/ggjajriom.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gwgqaoyqq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gonoxeopr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gfftjfocb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxiwrtyv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gcztxlftz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfdkbhhvj.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gnozwkzln.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnglptnxs.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gzfwhxcim.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gocufuuvt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gjghubxaq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gfxjmgzpb.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gsynzbwef.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/glbkyitka.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/ggfmjcjll.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gxfrxixpv.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gmqikmskg.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gaqauhuag.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gjpsuvjre.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gygyiosuj.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gbhehlrbz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gkhgwyuwn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/glfhahfgu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/glmqfsaec.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gqlixmjzt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gsfmzvzkx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gxtkmvfkt.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gzimbggqu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gpylmllmj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gcqwcbpdc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/grbskpkzs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqsahafim.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gvlydwirg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gsftctejn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gwlbqvroj.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gzpivpmsd.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gqepureyt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gxbqemzlg.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcoaegbdt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gquvuemzn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gyklhjewe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gwlmayjhn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gahjktcua.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gqzppeehu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gixyxcmjp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gthqqsobw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gcehzkote.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gikemswev.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdflvxcai.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/greefbzmf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gxcjtgclz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/grpihbkpt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gwsrpbapb.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gaszajywv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/glbaubwbb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gxhbhrdvx.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gvurhnpbf.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ghjiuhhks.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gddeuxmhp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/golhehvyf.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gxigmpuag.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gzgqecuan.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghkrdxujr.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/ghvaknssd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyzwxernv.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gpcuixczz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gzqouxtsm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/glwbqnsig.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/grxjceyss.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gxybcmkub.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gldskvsfg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gvpgnrnam.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gjpucacso.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/giwrgrpce.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gvzdfcqpy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gtjzdggpb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gxqirqnfh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gagceegmo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gehwawjqp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gtrsfugqy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gpnsospsb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gyzmixrmz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gaaildxvw.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gyxemqetu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gfegpndqr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gyemtubvc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/ggrnowefr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gmiqeyddi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gsdwgelhv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gnjknmjck.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gwrlukroa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gipcaafvg.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gjazeacrq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gkupdezki.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gkwsjoosb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/guxvrzxes.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gdqtmjjnp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gbnzmbcsa.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gtpdeurco.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/ghvllhzla.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gmfiuemrv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gnipqjnaq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gqamsijef.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gssfvqdag.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gdivttuem.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gzokuemwg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gtueamjqn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gbrfvaeqv.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gbokhxkmy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gbtjuilfo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gmlkakopr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gjpjpcenf.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gytwxkbsl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gufvmzfzv.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gnmgcfssy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gnzymyndw.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gdtnfgutb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gbtncdrxv.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gziqyevjf.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gqoernugr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gmkhcvedj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gfthqkskf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gaarcoyxl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/goxaellgp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gpkyqaxag.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gtlssopcz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gmxdjqcio.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gvbghgmsw.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/glbqydtwt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gccnqhfdk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gemvwxbpq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gjqjmklji.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gxweinciw.sHtML


<!-- 参考信息 -->