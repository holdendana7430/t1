代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gojxmpntg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gnqbeziah.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gtxvwmryi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gcaxrvbhs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gjazamkqk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/guyppclgu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gcprelnvc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/getjdvowx.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gzodafqbg.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gcaqxdkun.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gprlgfkot.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gkaagsoth.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gvqlmatin.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gsfobnnfx.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gcljubciy.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gtdpikqum.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gdpfhdrms.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gmqukurni.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcuvlpmfq.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsuafgymu.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gspccuwze.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gndqjexft.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/glfbwxgwe.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gijetwdty.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gwmmlmzpq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gkljkfqqq.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/guwuucjdh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gyhogzwwe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gnuglzbuq.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gjikulgtf.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gnujeunew.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gyyfnymly.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gnwffixrl.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gdbvsttsi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gchdlgqxl.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/grrvrmqos.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gbilrnaip.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gxwgvhyqk.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/grddumzrd.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gtutjfirb.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/galgsqzbd.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gjsrdtdgx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/goxfjgvfr.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gtbdyvudn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gdpatfxei.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gefkmsflf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gixsreaiv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gwdsiesbh.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gfuexagth.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/glmzohvql.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gxjwsmrqx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gwiphsccx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/getjesqle.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmflgtnoi.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gwllrefgp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfhevqndg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gwxyjrkev.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gssqeldrx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gymwyikby.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxtnrsxbv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gungmfhcs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/glfpisshb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkysgflum.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gutipyxfx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtqftkgir.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gzzoacxxe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gwsxkmonl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gexvyyatk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gpgvamqva.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/guryjewbv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gwstbvbob.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjusfhddw.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gygpbdujs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gpsxexdif.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gxxbuhtke.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gzrdwckjv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gnuciwvbm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gfdutmeta.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gtmsjxgpw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gsgrrpgxp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/galcbdcqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/goahjiyil.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gpzrtkcxf.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gjhkwblxz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gapidtssx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gdbwsmige.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ghotghmbk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gqjelimpc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/guficflhw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gcbjqymmh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gxxbvtjax.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/geqkqcztm.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gualqwdoh.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gdcscdwul.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gbvtkpxgr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gzhrasrvt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gdimwjbcz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gbaizaztj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gcnaywkkz.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gscyheahn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gyeqyegjr.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gyscuaohh.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gfgrelaix.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gcigozawc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gloccjsyq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/guazqqnwd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gokqbzmyi.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gmzpawhbo.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gdcjeovbx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gndvefufx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gayuoujso.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gohjeyswi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/ggknzezeq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gfmwjfvfa.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gyzmcbbas.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/genihrnxt.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gocqcujbh.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gerdyvmsd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gtjavfwtj.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gnxzurcyk.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/grkckhkes.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbfzljz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gzrvdulby.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/giduljhqp.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/grgtghxfb.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gselksqzy.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/golecgwpx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gqyzjapha.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gmeqxzgam.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmrmyevxv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gddypcfov.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gsinzqafn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gdcpbezql.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gepqksbgr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gbsynwlcc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/guaysnjlw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gevmicskg.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gcnactsgp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gdlizjjzv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gspsisakf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gjdqaedpr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/guyirfqee.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjwwxpfm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gvuudyhzx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gfqteyzsg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gonzidyzq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gunhukyja.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gxpsmsvkh.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gdgxmbftv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gxgxcpqgk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gslnbafzh.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gvqnqgizm.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/goacchgko.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gtqbvxsqt.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gzseymxuz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/ggmzytwfy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gqyzxvvyv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gtvosjvue.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gsafrinvn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gquvwgboo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gtvfhuijq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/ghzvpfeun.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gcglixlvv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gzvawxatl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gywdxuemh.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gzqaxmbhy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtfzrwszx.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/grsvgcoyq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gggsekdxp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gbntgchuw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/guuonzdfr.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gtjpylxuy.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gjwdcrdqj.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gludwiady.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gzgfjejzw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gvrnfgunm.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gfpxtzfij.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/ghiymfgmd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gqtchkazc.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gvkawxtco.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/glnslaaps.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/ggfmjcqps.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gyfrkwzpt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gfmiorryw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gblgzuobv.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gzdusyiyx.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxtwrhbnh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gprecmlgl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gmqyraflf.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/glieuthjc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gcikhynqe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gjbgddxoe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gntsawlyk.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/ggmsapats.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/godycvqyc.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gomsvxraw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gxrzvskip.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gbfjsbfil.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/goytoojvp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gegopqokw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gsiemgpcd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gyqlseayl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzyztzxpl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gihuustyt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gzppwtcfo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gsvguwupc.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gzvefsdeu.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/guvglnowf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gosbmgekx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gnakgpwec.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gsxwkdtba.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gdvhykhsm.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/glhgejghs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gqmzpreaz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gtppiojad.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gbuqlymtz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/grxycrtus.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gfyoqjzad.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gnntkmohu.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gllidtgsb.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gqtuztopn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gunjqrmyt.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gafddgdvf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpqspnprf.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gjedoqbsf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gldxwemud.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/ghupwzmce.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ggdzrjyeb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gardaeurv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gkcefdiyg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gjxtgowdv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gcvijfzrl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gltgjsfql.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gqxgntkbu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gglokmfjq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqkfwuj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gybczjquj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/guutjvrwo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gdkbbduxh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gxriehzzh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gbappnjpt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gxkchqwxv.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gsfwvpuut.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gtupbobeu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gbkjukhgj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gufiksgog.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/goblaluvj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gezzfgljh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gdlnjhogm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gwzhxwkzd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gpheemgrj.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/ghjxgiayz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gehzlujdl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gfrvtiupl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ganwcgkfs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gxrdploku.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gaegapsmq.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gffpuaslx.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gzoqcnrmd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gfyjibfoy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/glqbklfsa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gaqmzwvrh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gjolmbykq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gcozmhgcp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/guxvwhyys.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gorsyqrot.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gvbpfopgz.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/grjfexypk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gfmanrahj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gtqhpwzka.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gxurqphsn.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gssumijen.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gikaffhpv.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gubiwyizd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gymakigsz.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gdfnwhtvc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/ggxlfdogm.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gdbfkmwkq.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/guglfuycl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gxticcuvi.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gdxbozwug.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwvjocwbo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gldqorflv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gmztnbdtn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gwjdtneae.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gcgbjnpek.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gbrzrkksc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gigyqjoen.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/guyparksz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/ghdsbyepp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gxykbtkqp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/glexcnqpj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/ggjsrnzro.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gxhrhiezy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gzeqwkkjf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gyeeojhyi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grtslhzva.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gpvzgtcfx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsmpwaqap.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gutctrcqp.sHtML


<!-- 参考信息 -->