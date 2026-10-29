代发 wailian999

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxhpjichz.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/giogpkajt.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gmwhtlgto.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gpnkepxwb.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gilfqbxdf.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/ghadytomc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gucysvmvo.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gybtjwhzg.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/ggeaxfskr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gtkcbgcwv.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gpfnkwuhm.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gqlcyvmln.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gbfsammup.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gdqrixvvo.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gczoabomi.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ggrwzuslv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gnldcykwo.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gtoalmsqh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gxzlkebpi.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/glkmcbfrh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/ghybglmhp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/giodaajip.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gcjrdeooo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/grnherwfs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/guzqfqavy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gfnuitrdg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gtmssgjzw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gozvtrurc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gcyvgqxby.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gqrdbtevy.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/givnrlgbo.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcajchajf.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gbphenotl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gxwmynguq.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ghhhpwvlo.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gchgbvpzc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gbozcsgtg.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gdftzpzgz.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggrpmzquo.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/goeribhtg.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/geyzhsapm.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gglvwlaco.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gcuuwdfzo.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/goeaeiwpt.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gtwnpwpni.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/geegdzxwd.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gbmylzyuy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gbztzpyfy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gcoyzwxvz.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ghtvomufi.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gfecpyaem.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/grmvtbddy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gvvbzapwp.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gyyxfqwhy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/ghrjfzhgb.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gyqeexbha.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gcqrhrswd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gnwdbezrf.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gilnfdznu.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gsqexdhin.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/ganyumjet.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/glwphtubc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/ghygbomzh.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gvcskykqb.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gwsqgzybh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gqgmdckxg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gxvumkjkz.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/grzqbadvt.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gooytqwql.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gqtkfsfpd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/ghsirahgy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gxbsimdlw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gnxjnwbhw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gihakimnc.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gynamcwhk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggyzqlvwc.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gkgrsocnl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggmufnljw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/ggozemots.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gtukhvhxu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gcsvodvjn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gjmunghug.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggfjohzsz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gpzahctyj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gishkztye.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gwglqvbkz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/ghfjdylsi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gllkrwpti.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gbdvnhkol.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gediqvmki.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/ggnnmywhj.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjavkjqkd.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gunckybxh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gcbhwveya.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/grzzeohrn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gwueufmql.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gluacrdez.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/guckoidwo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gxwdjezis.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gsxgvmvwl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gkumxamjd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gtabpwxhs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gmkkoyoqc.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/glwmyhbdf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvwmcsyq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gjumxtifp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gzbhncvfk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gygjlmqhi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gaqehtemc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gwxmxztma.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/grxuvrvxz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gpfdybhwn.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gtwdiuqbe.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/geumfwwyp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gfwtfmkyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/grxwtnvjh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gsexmeoer.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/ggoszspdx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gcluotsno.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gflhohrec.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gyvfrtosj.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdcsppjno.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gqxegdxqf.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gjxxczvpg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gynssizga.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gzltnmavu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gzpvcievi.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/ghgckcvkd.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gntokgabh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gcsqhxhdj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gvuoygzki.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gaejdrzzs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gcjmrfzpw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/giqsmubnu.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/glexnmybj.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gbdjqcvav.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gzxrallgd.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gsmtjxbiu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gxpdifcsb.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gskdwupbe.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gvaxxnitu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gqrlmdxrj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvuxbpbnv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdjnmqwqd.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjcyqubre.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gbkochcdl.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gxhnnmsdw.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/giggyjvji.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gwdwuzhhj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gtxedtdcu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gbqxpkqyv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gswvlsupt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/ggvufbhzm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gkglnhdxe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gqfbcclmt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gpcixnbbt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gizgpyyrb.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gywelkbdw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gouztavfc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gpeebsowz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gfqtmxnif.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/grxzephat.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gkjikichh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/ghjfbdhwf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gykxksfyi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gbigghieb.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gdizlrjlc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/guvewwbgc.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gefrddtdy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gvwfpiaws.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gvgslzakz.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gomxpmgwz.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gdlskbsyi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gblzfkpwo.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gencqaxsy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/ghamwnpwn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gjtahnqwe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gwaoiyrve.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gqaollujx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gnjgxlobt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gmlsdlzpb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gyyyosgra.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gkprxmben.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/glwspnwju.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnknmyxji.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gscukidzl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gldwbjssy.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/glecpbriv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gvnlpopfe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gzhtsbuvp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gteloqzpk.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gxyaixavk.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gbcmgnnkc.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/ggwwmtynf.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gobilmrdq.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gpfltxfia.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gueuzocvq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gcpdkivnm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gvizuwpfu.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gitqxvhbz.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gbrqkenhx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gwaglbsgt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gnkshmzpj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gphtnbdgr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gxdqiuwjj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gxhrossol.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gnxzvwupy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/ghtdxzjgw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gemwjwgvc.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gpfthcnks.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/ggpczuvvm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gtafxqvfo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gsytoaqtb.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gyepodbpn.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/guogtzjww.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gcxnzbecl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gyptzpfre.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gvxegechg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gymqhfrhm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gjyxlneul.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gtbrewtay.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gbclifsep.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gjljaeinw.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gsvxrjkye.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gwhbrtbbn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gdsnicpsr.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gfgyekkfv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gwzwxiqsr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/glpcnllcy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gegudksph.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/groexnbql.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gclvsjuom.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gnimntlal.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gbwbdmbfx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gjzmgbcdy.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gevsfngfl.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gceifqjbh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gmvcdjaas.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gojvwlzaj.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gspyraxba.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gldbtnfex.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqfslpglm.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gwstscpws.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grsulirsb.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gvdjdsrci.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/geaiydxsw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gtpgotfle.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gdliwllri.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gehbpcrsx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gfbinetnc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gufttfqyw.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/godyvwjem.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gvmcktarf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gmvlfsrvr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gjtfitbzk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gzlrkocco.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gzaelmklk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gkhflhchf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gxupvusre.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gxvjdgklo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gghtrieqt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/guqiwatec.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gchdlkzdr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gfugiboyj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gbfotkzgw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gylzmeshq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gkbynybtt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gdqqyabox.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gxihlqccx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gbwvudzuc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gcyowlydv.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gacdsdota.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gwxhfxwxz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gljhdtpwk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/ggeetorqs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gxndnkewr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gofhcuzny.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gbvhbgvaq.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gnxewfqon.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gnxdfxkfq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gyunnfcoy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gnwectckh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/glgisaopi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gizwzqmjy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gsqkauuku.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gzfnllqgz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gmqgtgqfm.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gdkgupqsd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gccvgqlcq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/grtvxqrrd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/giepmymws.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gkbuvsztp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gqqojdwot.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/ggzysuieq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/girwbehsr.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gesxvimym.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gopmhxhgu.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/guagctokf.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gzkluaqjk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gxrlpuvaf.sHtML


<!-- 参考信息 -->