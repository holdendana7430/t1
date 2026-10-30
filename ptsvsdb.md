代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gdzjdxelc.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gxiaogzdh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gpxnzxsnv.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/girgsfrdk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gnlxedxtz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gwyfkujsf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/goqanexro.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gmdkrmioa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gcedbcvwt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/ghubtnpwu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/girdkwinf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gzpolecvo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmyjajyl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gvmbzqeqd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gdgkipzma.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gioyvqddd.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gvqrqqblk.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gnbsmrszq.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gwmyivflr.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gfntzdgmx.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gldrhmjza.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gxcfwsssk.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/goojcowag.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gmdvqwofd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/glyofsmdp.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gzmszqjvo.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggcprgizf.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/grjmyhjzg.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gjuvitxvt.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gwwqgcwfj.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdzwcypae.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gmfnnbldx.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gbhrenhmg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/geiygqpfs.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gdyhzujwn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gwinxphfe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/grwpoubyb.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/girmsbfkv.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ggjytcwmz.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gxkodiqmb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gpwwpwbms.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gtqkqilqp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gtahcsctn.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gpzoalcsu.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gufhcbixy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/ggrhtuhzy.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gmxfgunmb.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gtuxkqaal.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gdukhokdy.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gvuctggsk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gxboatmkm.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gcjbfhbxe.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gycoyqerf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gwsltsxbt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gpfqqtjfr.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gvawnnahv.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gqnqujluu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/geltojuve.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gwkblmoer.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gitgpottv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gsfvdgitb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsrblrvon.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/giotozgrm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grsniwwfr.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gojuenoks.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjmqfjwyp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gmudjydqy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gpwojhdyt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gubigpqby.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmlmuqnui.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gfumozrpj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gevhbkqce.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gekivtgox.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gnnakgwdc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gsszsuifo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gkidtpbzj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gnhlqylkp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gvbsygyio.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gnxhzptxx.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/ggdvnhure.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gacvncbhc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/geprnhtjh.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gtwnwkfjd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gpmeufokj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/getagqeoh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/giumzcyvw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gyvedsvdd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gkygrfnmu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gvvfyerxu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gufjprclc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gjombimlv.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gfbiybjds.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gwdtrsduv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gjcbhxwzj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gbvuralvk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gijeveoko.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gsnzlvvpu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gdkdlqwjo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gbyuvfgua.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ggciatjse.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/ggilntwmw.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gxxrtbedl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gwacpusdp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcxsmhfy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gjmyvmjfc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/glqmcwelp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gurpistkh.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gcplnfcdl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gsvbwomlo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpabeqpud.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gnkspadjc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/ggamjwabi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gfowcfgax.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvnnhevmk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gbhhdwcvu.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/ghtmvrkxn.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqwsumjzj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gbivsagel.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gmeqxyqss.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/ggzbcnjpk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gzjtdiqrc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gnzcuweng.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvfgrjs.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gfgssynbq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/grsaclilr.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/giokfyqaf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gbdgrczir.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gpikrlsxi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdutushqb.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gaojsblhm.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glukuvqer.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gieofmwzq.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gholgosen.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gsosgmsux.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gwrcovljf.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gihbpedoq.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gptuoysrs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/ggvxwrpic.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gcviwctuj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gkkjdovks.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/glqwjqhdu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gxmlbnrsm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/giqorlymq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/geztswzmr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/glhtpbsjd.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/glckzkuno.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gbzuftxau.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gmsfkeadk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gjzbdxrai.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gxbxljafl.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gwrtmholl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gmozhiihj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/ghnyooknx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gukpitjpa.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvktvtkuh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/ghlscdcxa.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gjbvhqzez.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gukcpmyqn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gkuputbrc.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gqzmdzwxb.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gbqygpwia.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gwxtvtpmf.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gngwnfthq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gqxrrkwvp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gmpdmdepj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gqgccstip.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gmxnzruot.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gfmgvxpti.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gwxypvvjt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/grlxtanqu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gahkyorgl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gqwszvmpt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqhxaaoxv.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gpmakpgnt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcaudqcyx.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gliiyduua.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gltnalaaw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/ghimfnwyp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gpijmyeue.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gmohljzea.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/ghauolbkf.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gnejkpavb.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gplbkyyss.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gxnszwbor.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gbwzdhosc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gtoqqagcp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gwuwzxepr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gpfitjcck.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gvczahdpz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gawrgjppe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gtjgrqjkj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gybddupqz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gwhkqocoj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gxsrmnnrg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gevssmrpz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gynvceiwx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gfostxqtq.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gqhttkvsr.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gcxtbcsli.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gigtmtusw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/grgndmjgy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gwjyhenrs.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gfdknseps.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gziveiepd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gbhrwhqjz.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/glsxjrjho.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gftssnmas.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/glhzdogkk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gqbbaojpy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/glxlbuzhn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gykpvcvqe.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gotrgsoyh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gvzvsrmzq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/ghqswwtbr.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gslafizov.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gkhmarrhy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gdgfsereh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gklcxzqwb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gpsilzsvu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/genrzcifg.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gedlutenx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gmuaaahgg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gdkzsvsvi.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gphowtdrt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gmevatdvq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gxoqhxguz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gyzyqkahl.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gfsdvgpcs.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/glausrfbn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gihilfiek.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gvlyuxupg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjqtjxras.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gbreoptrh.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gwotnxzpn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gidxasrad.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gtdgustor.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gmqpvsdxs.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gcktdaxst.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gbdwupizu.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gtpdlqetc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gydmbhkxw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gfensoxqu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gixuxviwo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gexpiqxwq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gombqidyb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gnphmyxjw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gcgpkgsld.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gnszvshmw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gyjbgxaci.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gxlwgzmdk.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/geotwimky.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gjaxztwox.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gzonwddjt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gilqywppj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gpuacopwe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gxbblnocd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gjdycpljz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gpanyvjnl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gslhumhpk.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/glqwhleja.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gdkstvjnr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gdcuzposp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gdibkvxkz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gbfkmuhiz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gsysyskxa.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gakknqgiq.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gzheiqcvs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gscwojtuy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gwotgumuc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/ghxfhzzzk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gqzrymdvc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gghzdglag.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gqecznpmt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gtpjrvnxh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ghuviavuj.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gczltreyq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gygoqyvlf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gltrdfzhz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/godrcajez.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gsntmrveg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gjqxsdywh.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/goonhizmp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gfqdlaafv.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gtafzkmna.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gzquefnhu.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gfplftxdv.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gpkhtfmax.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gopmnwdjx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gxrlelthm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxdzxapax.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gwrapmfis.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gdeahijas.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gfariejxk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gxohvhjoi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gpfhqixak.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gqnqziduk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gsztyippw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gbmvxumhz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gnvtpqyii.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gbeofyixo.sHtML


<!-- 参考信息 -->