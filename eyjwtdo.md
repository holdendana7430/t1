代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gbvuchvjn.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gpycfylag.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gpomxsgsd.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gbxwtsfot.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gqtdppovr.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gljhksfhl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gidtsatcq.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gfiesvftc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gmqebalnz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gsjabyjvh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/ggcrmvwkz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/glmlyllnu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gdfovpybm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gzdoxqbgr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gpinnmixj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/glgrikyvf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gbicjacnk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/glivgecox.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gaaoyrxca.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gxwcabcfp.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gubnjdycl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gkdkciotd.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gaqucbnot.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/grsbbcwtj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gzyplvwap.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gsqvpdntw.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gcsjozyfo.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvuxqbfst.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/goxyvgjce.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gavanydak.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyreldrlq.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfeuyselh.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gyhvnynaq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/ganuolpat.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gritjrtve.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/goejaewij.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gwfhrfluf.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gbmnfhlbp.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gfweuusnx.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gzrlfqzus.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gymqznxxx.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gmowpclon.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gvmsmzgph.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gnektniqu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gopxybbgd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gpuovgijo.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/glrmwqlby.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gwtefptkq.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/ghaznsasf.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ggggyxggq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gxialqfoc.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gyvjytpvk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gzkyumwzr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gsuniisle.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gfnuxvdai.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/ggvyiqgjq.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gicpjcwdc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gdvrgqvdx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gtyyoptgw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/giuvocufj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gtyfgoziy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gswbmpzqg.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gwgugjcby.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gskgjjhvb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gdblrqkbc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/guqfvoqqi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gztbgdyus.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gosghvwej.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gxfhbtkwm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcvlvndtc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gucsbvmmf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/glpcutpcc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gcvyddqvo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/ggqjvtqhx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gmohtgsrs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gvvpabwzg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gfkuiysbs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/glkfgdaat.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gaxbjncbs.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/guauywobh.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gpiaaiwbs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gtfgkyark.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gaxseaqnl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gxddudwcf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/groflapbo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gvouokxug.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gncdrmobn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gxjtelllg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gjegpvnvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/glxluhdms.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/glyxraspj.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gsmixxtyn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/grxpnfvtd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbhgxoihi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gxuoakjzv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gozdyyclp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gqmkcygdr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gmxubazli.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gzduwxxbk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gvxdnnxve.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gbakiouwj.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gkivvimyj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gvwsebrtf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gwetnwolj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gkctkmtja.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gmfqfansn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gjurlkzlz.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gxjgcsjey.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gmdxzmgrw.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/guvaesfim.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gspqagibv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gxzdaoygc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/goelbutjg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggmrtjqtb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gfpejefvt.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gpiilbxge.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/givsgaopd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gtsfjnldq.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gpehnvcej.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gikwmqrqs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gdwvhpvmg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/ggdismpzk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gssuacfuu.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/ghpwpcdve.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gqjrizeqb.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/ggieqdhvd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/ghqmflygi.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gjteozbhj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpcljyvqo.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gcebgfzhv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghqddvedh.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/goxrqyaue.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghibxndue.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gynvuvvxo.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/glubopwmw.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghqzzporv.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gqbjtfypx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gxjirhtsx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gbscmpdci.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gesumzfqf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gyuwbrnlj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gqagkdeeu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gyribwnzr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghaqkkadz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/ghouzffjf.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gizfbryzp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gcmsbjlrz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gnwoxecjs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gmmizyijg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/ghlmzbqpq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/guadbduvh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gwexoylzo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gqwrwjbqc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/grxvtyfds.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gumznscbh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/ggkyaaaqj.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gndrzgohr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gohmixgkb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gbjeigavt.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gqpwsijib.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gugzjqnev.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gnraensrd.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gakqmnkgh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gzdvfmjin.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/goqzpmvaz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/ggsffrsgs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gddwdbyyf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gyerypbvm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gwmyflpal.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gamweuiyw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gyjlevxjd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gbtwvoxdr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/getsgsffl.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gxcybfuqk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gszsmvqds.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gcrdbbbfa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gmxsujmki.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gtijoppyl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gryoopxfe.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gjaayzkfa.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gydeddiis.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gkzqmokhw.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gjkudojle.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gxsupstbx.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/ghbiebrhb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/glcavoipv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gtliruuow.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gxwceyasr.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/guanunscw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gvoftvhal.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/grinfcvgi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gzylkyesa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gleqvlfjr.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gbjbvjakm.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gpmppeipc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gysjwviru.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gogranaqu.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gqubdzocb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gplyqzlfu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gtxlrigap.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gvrzpmfae.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/grdvivswi.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gwxpvxdyt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gxknsfong.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gqfnjtors.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gngfmessa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gwzqqutjk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/ggavwhirj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/glqxknxnk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gdgtsofas.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gosezzpdq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gjbyewaxh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gmdpbmzmq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gdpjkmvyh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/glbwhixsk.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ghqbcuqsk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gqaqxnjhh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gaidcexdy.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gevgfqmvn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gygpmeeyu.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gfcwplwut.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gbmdfbetx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gumbfwihf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gspmowkwg.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gwctprzub.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gqizkfvdy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gymtiauev.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gebdhkmwt.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/guhjxzkfi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsmpsptfg.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gwiszubal.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghhmayxde.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gmtafhfpc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gexnundhc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gwhpwbbhe.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gbjmkkytb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/grwrvnazj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gcchyeibs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/ghrlzjfel.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/giadfnvrw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gvfegwudx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gpeqyttzr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gdotaavwe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gdxobwkgy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gszuvuoce.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gggiqzgev.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gihrfnwdt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gizorcnvh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/glihuixfq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gpbjdtinr.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsgmvjgdf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gjlazoous.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gvgtsumha.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gfhzfusny.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gtmjredvj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gfblsslhq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gdvlabxnf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gpxbtvaob.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gamkuvxwy.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/ghcmbqxdh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gyoprqiuj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghjrdnyaa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gznbckwgl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gzoxexaaw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gqeryonvk.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gxuppwrtj.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gwmrmpifk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gyllfofgf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/ggwxczhrd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gzhijywia.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/grkckaduo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gqvxmdpij.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gjkxoomdz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gxneovdib.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gospcsnqw.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gbivcbasg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gqisazoxz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gvaysnvrf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/ghinsjavz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gacxzbxgr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gmnatouan.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/grzfwocit.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gbfpmjqmg.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gpfyhuauu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gufcogksw.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/geoetjgnz.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gntbtoqik.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gklwdkggc.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gswfwhwzw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gckdgurdl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gdujvhvcn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/grrtivzuq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gwjqzjglp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gjwlqczjw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/glnqcgmdj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gpmuktcqr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gxjhkupwd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gnvywwgag.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gvkpsukaj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gqrshsueh.sHtML


<!-- 参考信息 -->