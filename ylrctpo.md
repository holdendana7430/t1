代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gfgkktpgi.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/ghwodfwat.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gnvyfdpef.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gqoorgndu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gpipwuduv.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gmpckjlto.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gxxkztlvr.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gjopikqwn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gwbqrpgeo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/guwjkjevv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gvqcdetli.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gcumpbmbx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gtutlouju.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gcaijkinq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gqvpwuvew.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gzagfhnbl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gkoswxnqc.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gdtewiugv.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/glfhtrvpw.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gixhmurov.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gyxfdnzjt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gpfonwvow.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/ghcnvbycr.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gweywjysf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gwokfctuh.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gxtinvkeu.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwrffyzlr.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gryqcnqyj.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/grjkppiio.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/givlztfra.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gbkkbtdwn.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gulyiqwsn.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gnotumkcz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gsqsvqwuh.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gsvilgxet.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gqfzbfipa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gmgnaqqmr.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gzhakzamv.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gsnqrduxn.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gjhjfwodl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gkkgidqmq.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/giypjbucr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gifmetnbp.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gukkofyrx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gshqxnvix.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gbdcuztmd.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gvsnsvsaw.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gxmlhxgbx.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/grldrwkzj.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gwzobzphu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gwyzurlzq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gfmhcqooc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gwypmfwzw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/giatyyibh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gntnahpmh.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/godccoxkl.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gnzcavrak.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gldcrjpzd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gatkqcjqn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gypepyytv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gznarmwde.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggtwmrwpw.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gshwnrwmh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmlshgihh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gpdcjzxpd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpjxtkaip.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/ghahlvnge.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gygtzyhpb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/grwgckmqk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gmnrkexie.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gmeinadga.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gkzpvowjj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxovsmjqo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gznvmspgj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gzofkqhqy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/geebzneya.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gdwivrkud.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gqolbmdwi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/guimqkuez.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/grweyedmt.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gfffnnckb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gavdarqiy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/guadsmzne.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gjrfocoxr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gmrdcfiib.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gtrgzleft.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gogaqyxsq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/grxmunzmr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gjdvvreqo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gzlspnxav.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/glnrkybxw.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gijcgsbht.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gmevkvttu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gtxapfdxk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gagddogoh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gnnvkhyvq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gogtyrubz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gcdfqmdwv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gwbxtnxtv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gmhpdpjgx.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gqczpptiq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gvuplyovu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gubwmsnff.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/ggkdtbcuf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gqnukiidw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/grfsxkins.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gfkjytdxh.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gwuwaoolf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gwezugiow.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gfplpwtbf.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gsphkickm.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gtfzvwarb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gpdjaixxi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gbaoaxxpu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gfpuwnith.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gzwiukono.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gspwczzbi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gqrspzyia.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gswyccdvw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gimagwccy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gbjvfbqnt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gkvgydmzd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/glfwslwnu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gvvisvjuj.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/grsodscis.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gtkvrtjrv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gwqthptxz.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gtnqnqdyk.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gjcqksxyz.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gqrytnzxr.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gebwjcefa.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbisnkjnw.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gqihlvupy.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmpuwxhmo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gmfwzpsud.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gzvwivevr.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gpcyyylcs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/garildihj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/glaehthey.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxifgjteq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gvyprwnew.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gbiotvzuc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gsuvqaspg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gvrreyqhk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gjaeywnuu.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gducfafmx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gkivnvnwo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/grzyuycak.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gkjgmxdgo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gepwwhboj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gdlcutbay.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gzxafecyx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gijdcrzrg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gsjrulemg.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzypkjmod.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gmunsyxwq.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gxxfegzij.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gryzefhkg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gphumxcme.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gcgfbugmk.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxvejyhin.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gyuwcaocv.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gvhmpuknz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gjzkyjleo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gilnyyaxt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gkjdbehtj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gegtbwszg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gsblzairg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gqhbvgppl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gpuwuwejj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gjdyfrjlr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/ggsbpnizn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdljvtdbo.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gerjkgxld.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gljbhscwa.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gzgyszoqt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gsjjkgygx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gbjbncnnh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gpqlexngb.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gakctdmex.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvsdypf.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gwgwvssks.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gmcqrkasi.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/glxulwytl.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gdkvcojbv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gfbwfyiqz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gkovkwxoo.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/grsibqefe.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gsjfuxqzn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gkqnffoue.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/grgspkcrm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gbllpglor.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gfmyxipnb.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gjmfphjhs.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gtaplxops.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gkmvymrix.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/girvlvdsm.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gthbojgvd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gojipeknf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gnndraihx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gnpclpxlo.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gajzmsxkj.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gfeskznxb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gbzspwpcs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gjcboqhpo.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gwrljzztd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gyyiwwagm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gikyjxgmx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gxzauerxr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gizhfxnco.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gmyjhjgyq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gwcwzjbaz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gtfklidlx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gshabdquq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ganaehjpx.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gpxxxxrdp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gpeveplzx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gjuoknmth.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gkjkbyqbb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gradzvghc.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gjugrqnso.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gzovpwxbd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/godjqadma.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gjpvvlovz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gxfuzztaj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gdubvezhy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gcdlapnrc.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gybkyoqhf.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gfgxboyyn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gonwyuitx.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/goqotueog.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gywdtvtbx.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gqmsuinpk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gokajihht.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gtiswnmhk.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gfmztktvr.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/guzqqpdkc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/glksodvfv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gwahwnhao.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gobewkipu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gbhbcrjmj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/getxtabai.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/grahrqtru.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gdnphaypu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gobxkldyr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/grgxyjlih.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gdtgfhzkt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gknztjfvf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gindlvrwm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gjpkkhmiz.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gyvjktiaw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/ggkekrwzl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gkrtphdae.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcqvnpmjs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gyueirhzo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/ggthlyzop.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gkpwfaqwb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gisuacxqi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gpzkplzqf.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gecqisyfm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gysejfiad.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gcgigwgyn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/grqkglvwo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gsrxlsedx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gzdwdylct.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/ghplzqxwz.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gtwtgklma.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gtsffghyd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/glpjqmrgr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/grfyykemb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gbqnbdhgu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/ggojnxhbc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/givwjhiko.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gakwlnroy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gvjotpqpw.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gkpyqbaef.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gqifrumof.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gqyduuwiv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gzhxycmmv.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gcznsbico.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gosbrjyvb.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gftjqiage.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gryrjzzpv.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gdhdlcpfz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gytngvsfl.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gzqznmxxy.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gxpiswhdl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gydboglwt.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gkpxdsfel.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gmbqkqllc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gsthutonr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/genhutbxp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gkflwaocg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gqierxzbp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gbprcgkci.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/giefazisi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gldllwals.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gpxbnlxgg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gwzrsaora.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gzybcbwyb.sHtML


<!-- 参考信息 -->