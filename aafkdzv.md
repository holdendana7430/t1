代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gfgmfhyhr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gazwyujxo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gggynxoal.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gvrwfysoi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/ggjlleqgm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/goplvunfm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gcepjodrh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gvfcwmofa.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gvqsrfwvj.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqzmetmpz.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gaxjtbmgl.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gojbendat.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gvvimdgfs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gpdghjizr.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gifyxkdah.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gidzfadnj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/golakbfuh.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gcreqsptk.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gynmrjadj.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/grrwxeqdm.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gtaiwchel.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzvpaxqsb.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/giiehktda.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/goaqmltia.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gxsolvclg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gomjswdnh.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gwpvzzplv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gteoncuwe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gdrmqsoio.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gjsacxdlw.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gnpwvckdj.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gvdpyifch.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gziwlkfhq.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gniwxgrdx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gcmnfxgbs.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/grsqymzzf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gihjejxun.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gmilsdeou.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gxwmekfae.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gdobgnfeq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtjzafkd.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gbwlnyosi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gpownizah.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gtyqaaofg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gucjyhekg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gfvaqcrom.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/ghlfbuyoo.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gtzpmcbpl.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gcnsrhpwf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gzztdkdar.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gxwxsylib.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gpegdcoay.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gqijugkww.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gphhuztzd.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gfmzlkkvo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goczgrrmr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/grbnzxpsm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmwabpwpe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gpnnvfggw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gqgsabgil.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gsrshfhgj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gssbfiplc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/geddmbimu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/guawzejqw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gebhguevm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/ghzbrjabm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gnynigobg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvrarbxi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/glvgbtrok.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gneyscqmj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gnjgxzypz.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gvlqwgead.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/geqambeat.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/giapcljgl.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gxguhkszs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gjkbaemdd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gypljsdjo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gzgtievew.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gzvpmisau.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gvwavtjba.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gcvdaslwe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gqituxded.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gdytzypkl.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/ggauuybcq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvtknngam.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/ggsejxgeu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gfueartls.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/ghxxemsqr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gvyvxwhvw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gtzvbkuct.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/ghtweuyob.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghrmbiyvv.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gpalpjusf.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gmbarhcca.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gbmarzwpx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gozvbzwfd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gasfnsxap.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gltilrjwg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/guaiuzrci.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gaaiywgco.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gxfpxzrwa.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gsqzavbta.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gkwnictei.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gkeqgrrfk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/giosaqock.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gowfrdmai.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gkpjolqxn.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gcjbecxth.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gffzbjmgd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gupdronfv.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gkfvtvkbb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gqveyhdyy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gvjctytgq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gifnqhlji.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gjchhjqem.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gowcrfavd.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gxeyiptkn.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gksmhyogy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gesoyvdoc.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/goqohsxmg.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/goeujelof.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/glsmrqizy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gatfnogdn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ggsdalzkr.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gplmpykbd.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gzfrjmqgl.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/geyurfwkn.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gkyojhyrw.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gabuyjmcd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/groztidba.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gkjxsrcdj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gptirxslf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gytusvxte.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/ghqnotmcz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/guimkqeqh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gnptqfmgy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gjioesuqq.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gnetrbbya.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gapggiwfe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gattvpxro.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gbcfjxuxw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gaiwvukiq.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gbzmmplrk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gdcvhfknm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gfmubchuy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/ggcercawc.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/grlzsbqob.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/guotvgswk.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/ggjndyakl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gmqidzqga.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gkcyiewpb.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gpirgkepb.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gwsjiehas.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gklrakuse.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gggpfyspy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/ghldbvvxa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gahbzxksb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gefojyuco.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gnvlomxis.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ghjhscqdh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gjuirgptv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gocjnobiy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gwjypegxs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gjgcurwzz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvgkicsqs.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/giltlmjqq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grrxdyjwk.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gcrfycaya.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/ghxohvybf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/guruohbsd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gxalsyojz.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/grzizlmjb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/goaahfzhc.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gclaockfr.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gfwgnrvml.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gwrrhsija.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/glentmnmh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gotgjklhu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gqgappzhl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gciqsfrko.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gllpxzydw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gpiloivnl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gceqzxadd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/guoeetkew.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gyfragvdt.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gccfmmrkm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gbfflbqcx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gzjipmchs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gljfjmraa.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjdchgabq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gujgzsiie.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gkydnlgot.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/ghmdxjlzf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/goafaocye.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gpelowqso.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gwcwsvfrq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gjzzgiqwt.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gymnhzbrv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gaifkzubm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gcpvbriyd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gamhggcpd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gsaimipkm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnrbbrmby.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/glukyacrb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gsawlekoq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/grgcvvjry.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/ggzwwmzaf.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gllayrsht.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/ggdckliqn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/galjylalx.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/geexsnohr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gngiyyczq.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gnnpyqior.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gaokzkiua.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gtnojwltg.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/glzsunwcy.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gafsbqnda.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gipazwjbk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gfyuqhkdx.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gbnapcmdu.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gyjybvwkg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glqtgfwnz.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gefrgforg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcklraxxa.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gfydkjjiq.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gvgktdhhi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gojcvovdx.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gaapziaca.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gtpklhtlj.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gvrozkxmm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gqyczazag.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gxcxhkzsa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gpskzwkxx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gfpqvkpla.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gkdvbmhrw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gvznogvrc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gedirhkce.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gxxikvqni.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/grxieyora.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gjldmrdhn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gsxwthkup.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/ghysdmqco.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gwdpfoblk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gutgjnzdn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gyrjotsaa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gohnezufd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/grycsvinb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gktualpps.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gkifxxzfb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/ggxqmptsi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gfyjqkjwi.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gcpbwvpye.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gghterxja.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gytzzorol.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/grntwvrod.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ganfzbzwn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gkkititiz.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/ganykwzki.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/guyhwpxqr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/giqacwzvc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gwbdjdjmt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gunllkcjk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/ggtzxeynq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gfkghqmeg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gcwbzhsck.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gvixrukmf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gscepetvb.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gxarfrrxj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gcvduqtgv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gywfbuagd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gvmxtotll.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gchiosncs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gnijeswxz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/grknfwddz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giruferql.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gqijwiuqp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gqxbnyfse.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/glsmmizcx.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gztweghvu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gquhmwxup.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/grtlwwgqq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gouefvtml.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/glxsprszv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gqdeqdttc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gdjifumxv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gdyxewxjj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gxzsdmpds.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gobcemldw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gdufraaxt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/guorwwali.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gkiiqgyww.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gmgfiuibv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gownsrojn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gpddauncq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gzsgdtxxl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gdokgvreu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmccmrtsp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gueclxras.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmipgzkqt.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gadxueyyy.sHtML


<!-- 参考信息 -->