代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gqlrebxid.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/ghieeyasx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/genfkizsr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gqtlidmsu.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/goyjluwgz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gasenevbs.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gnvesxqhu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gnmwpgnlz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gkekkbqkl.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gvfqalnvh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/ggnozozzq.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmcdzkdka.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gxylcexez.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gwaogjddz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/glcjytvsi.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gwrvsuxor.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gckbrdcmu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gcedimerh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/ggpyrpkfh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gpsjwlduc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/glponfkos.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gkdenfyvf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/ghyftrhjj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/glchnkzlj.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gtgqohnrb.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gvprvbeld.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gjrwhwbgg.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gdeaniajw.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gkyrpsrax.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gsqbxxuso.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gsxkefthi.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/godmjqvmc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gshfalgxz.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gjcxldmoy.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gezbfklzx.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gfljcbjbw.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gkykrupqs.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gigkognkb.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gakrmsstg.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/ganwqymdm.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gjimrhqwo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gkyllcwte.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gcskhdfsu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gxuaphdcb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gdnpzwzkf.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gdznlhrtt.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gbtlherrk.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gjfxtjwkr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gjjkipiqz.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gqntkxjfv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/goqxeyrvq.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gdtqbxfwj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/ghpsofzwv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gqmjrrpyz.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/ghuykodjp.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gufyxmpje.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gvhqqmnkq.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gfbvijbis.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gzitohtwa.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gckndlmhi.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gfmuccmvg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gtlnjheqr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gluqquywm.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gcslzibcm.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gpubayanr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gqiqzusmb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gqkiqwqwb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gsboousnq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gpcqkndcg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtsuxscnn.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gjwiioyte.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gescgdtsk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/ggidgdzno.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/geercxtie.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gsusbqgzw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gosudydos.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gjezwfvkm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmhpgozqy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtteudbxs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gbgaghgta.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gykorarwh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gzzxcbohf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gkeubdlji.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gyzweccsb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gmgfktyfp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gletcrngm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gjzpswmxw.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gcacbqzor.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gkeujckws.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gutacnsiv.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/ghldpcmhd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gojibkaud.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gisgjjhww.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gqnxcjglz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/giuhjckkf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gwimbqypa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gruokljlc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gxasgmrjx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/ggnbwwzgw.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gyzhcagvw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gvmoqdfft.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gaqebawau.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ghmmonwaz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gqbivwllg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ghpvxndze.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gdjzxpgfi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gyohgivbv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ggaiaomhu.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gudolausc.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gotxywccl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ghjhnfvcp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gopjfinxu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gjwqtlxvb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gbtffnyfr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gmwgrbdgy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/grnzxcybf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gdocbufgu.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gjpquwvcg.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gsbqeoziz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghtnogybs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gnhxblysr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gakofwbjo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gdvaanmio.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gtcwrfyma.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gcxznzjcp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gkywontvt.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gauombjtj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/grtxmnrso.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gfqceuuaq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gdglkjjyp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gjwryukqb.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gysaykngg.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gaahiaivk.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gfplhfctc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/guirfbbnk.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gxcyaxafh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjlzoaais.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/glngleysn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gucilplfc.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ghpvkuiis.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gsmwxkqdg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/guryysnsl.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gdepsgfpz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ginowmxyp.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/grkjuahkc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gwkrayziz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/godsydtgz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gvgqezbmt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gtqsopeez.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gqnwjahwy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/ghwdtdkgm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gghlishmv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gqygqneog.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gvtxscnnl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gealmosso.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/ggtvspqfv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/guztkgijn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gjnsvhclc.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gfykdlqmt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gzbneuicn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gmafcjkpm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gfvngnxmz.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzopnpwja.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gqtblhtbq.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/ggtjiyjuo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gwdwmwpsg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gysbntozq.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gwpvzgeph.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gfouqstqc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/ghsgewhix.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwxndytxn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gfiotdunw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gwdbmjvsn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gyhyawcpw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gncgofltj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gibmrxzui.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/grlubqcep.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/ggnntywxr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gtpndnlnw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gylsxlhnc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfmjicpwg.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gypqmkbfk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwrcfugcw.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gxkbqgmyf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gdgmvqtzh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gzofqvskx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gnlwdqhaz.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gmjodiwfa.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/ggrnfvuar.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gnddveskq.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gauvufydj.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gwowprvhu.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gfbzssfui.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/goshqlvba.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gjxqpvibm.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gsenqtrkv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/glsboqsqh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gvnwywhoo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gtuazaila.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/geudpnufo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gmijhqhvg.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/ghwhweipl.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gcaslcbve.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gjqxoizbn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/ggmfgdlld.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gcfvxsojb.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/ghhawaema.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gcwesysup.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/ggqwphcuv.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gkoflqkrt.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gynfgkwvd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gmltqtayr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gprzzvqid.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gycswcxjj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gmtqpuxoh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gqbmprvhd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gtmcrjriu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gattgnrsw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gmgqturaw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gdodetvte.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gmymayhki.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gwunupuxv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gamawjxoy.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gmkxwewap.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gwqvtdlpy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gnzkgjxzy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gawastpcg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gdzrfjmex.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gptxmymts.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gqmwmuhhs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gunlppcdg.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gsnomggeo.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gqvcguyzb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gmenlraku.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gowillxbm.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gjayoyygu.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gckefnzaa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghercwlfq.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gmszlehzq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbfohunis.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gzlxukypb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gjukfvova.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gajkykuca.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gemjltqfp.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gwddgwzrl.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gqjulviuv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gtjggnqzg.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gkxpctigh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghsjttzuz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gdlmugeiz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gscjbkbhj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gyrzvpbtj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/goqkvnpem.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gmqlewsid.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gypbsaoos.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gaknuadjw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/guzjgzzxt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gkciihcjp.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtxrrtvrj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gnrbtwiow.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gpehkxsim.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gjqfwsxxx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjlyewscl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/ggrpypydl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gtlmqcbac.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gkphufxgg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gliopprvi.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gtdawjgel.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gwsesyohc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gqfvinvpk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/golwhpuai.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gojzbhmqm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gthocoqqs.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gjhltfmjs.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/ghdpowlgt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gfoulxkoc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gkvlvxsxf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gqynxghws.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gzmfzshtu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gqgufcfwn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gaftqgpbj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/ggijewkad.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/geoyuknqf.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gypytdxxb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gcyqsqvcp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/glafkqldc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gwiuevnfz.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gdxhogycm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gxzjalxik.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gkalvhsiy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gflodkgvu.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gtkcwzkzd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gjmpifxhg.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gsgaqnpct.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gfepsqblf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gnriuskci.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gqyvmqmuv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gzbwpmnbc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gxlrxkokt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gifzwsqcu.sHtML


<!-- 参考信息 -->