代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gfdgtiykq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gvsnujlfi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gzaeqwceh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gndynrkmp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gmkjbeufz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gzxyugpbq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gkkscquzv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gostfslgf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gamhhkioo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcuymaqgh.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gwgmuuyqy.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gqvpwbmbv.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gofzxcwit.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gulbcbnyp.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gcuzaxjdj.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gacjwdffu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gzejytzhp.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gzfkcwxtn.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gzrbtwldn.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gemzdoste.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gnjvrrzxj.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gidojlxyy.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gkmjityqq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gytssteeu.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gyvhpnjbq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gchibzerp.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gqoocohpg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/glmthyeok.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gqnwmvogz.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gxcvhlfor.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gzapelodp.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gkdwazttw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gvkrotjbo.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gqmrfijkc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/giihxznph.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gcqqqcjlg.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gnpuonwhn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqselamam.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gvaiwzwwn.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/goevnlkqz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gtprzqsfr.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gjepkfvxc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gtlkajdig.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gpknniomf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gudqoqrxp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gpwggduvw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/ghwhfgnjo.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/grreiahdj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gqqnbtxfa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gbfeuxyke.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gbnhtzgxl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gxwulogyi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gbpbpcbik.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkdtyywrp.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gfvejyosq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdacevdqy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gadmfjkes.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxtuqebtv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gpkfefigv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gbnuwgrxy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvnpdnz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gbseuunjk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gydfvpemk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gvdybrgbh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmxyxfumx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gwwpoyhes.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gyengiuxk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gaffhgiup.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gtvvtpbqp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gcmsvrcwe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gtkkpbyyl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/ggxdnngel.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gsvztqnbp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gznwiaqsa.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gmowiqrxx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gsaufjmpr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gzffkuhbm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gkwpmgryo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gvrzreclp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gocaykywt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/groztxbca.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gsoyyytsp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gdsxcczft.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gzakplhfw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/goepceujm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gowfuubmt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/goaxgvfrf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gzlvvjtnv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gpnnrzktl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gjiyejfil.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gaxwwasun.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ggbeupgbm.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gnnjelnza.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gdhlbpfva.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gbcbxslbn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gsynpoaws.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gkfdkblhz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gvmajozpi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gfxxifqcg.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gaewnfivs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gxnmxsqnv.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gvetzkqjh.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/geydwmwtj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gnzvtntra.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsdnmrnpg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gajamvgfv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gwvwuugou.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gjrrnettb.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gaynvqkiw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gxrijhfkq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gvnjadfzy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/glazjgnnc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gwrcfdmnt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gxmowfggu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/griipdfny.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gpzblqwcz.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gpwlvtumf.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gipqjhevr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gyufmglpi.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/glasilsas.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzoxoipfi.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gmwppbtjv.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbucwhhdc.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gziubuigh.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gknggxsou.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gybwbprnk.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gkaflfdtb.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/goqoxwilz.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gdhngglkr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/guzynrmwc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/grlthodzh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gukbsynha.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gimdjonlh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gorrdqjij.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gpbfprbta.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gfngbdjbl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gawlgbrgq.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gkyelzdpg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/grjbmaomy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gybsbglxu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gbfczzhvd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/glrlrofff.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gaftlpbcm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gjlqtkbic.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gjirdvcsz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gznilthdf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gszixzkwu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/ghsgbuiaa.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gjvkaovzx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gdeltfnqy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gngtnumab.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gppmbheeq.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gkmzfaptm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gwzkqcimp.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gfuiuxrgx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gsaxkopwx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gyvvssviv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gkucjddap.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gnmvyxcfq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gvwyoypnl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gyjjosdtp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gkkithrca.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/geekdkdgh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gimzlcngw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glvkckjqi.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gyxsddnxd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghysjjfii.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gpfenkdql.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gkthialmi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gtycqxfjx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gufgytuhj.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/givrlxkmh.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gmjnullbg.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gvwipizrm.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/goocebnzp.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/germuswly.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gnayadauy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gjxoyesgs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gcokbxzgl.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gfrwgthzn.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gdciwdopa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxljxktfv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gqyrknrrv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/golugdrdk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gilezclmh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gcxfjwdpa.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/glikcpiei.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/geimehucu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gdicrdwer.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gvzhlexlg.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gimaegiko.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gpguflcdb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gjifedptc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gnmwguwsr.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gjgdkvmhp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gusqskegp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gvxdslbtu.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/giacroxab.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gpwwqyyha.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gdoxuyfrq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gizimitgo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gvjybjtln.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gfymaxeik.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gvtzmtuhl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gmxcfopkh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gopfxivgh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/grfyxztrg.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gcyqzmcka.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gqcxszczt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gtxwwjwlk.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gtdaxkjpf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gzenbcgaj.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gfhijsjhy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gmvuumgti.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gkjysmtzp.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gibyrpgsw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/ggjwbozjw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gheqrntix.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gbqrromxl.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gupsroxjd.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/ghiotpftz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfocrliyd.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gxtacygqt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnmldxzje.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/grvmmcleu.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gpcftvipy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gkgvcfynn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ggiadakhf.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gunqsxgkj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/ggafomuuj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gptwyyppg.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gkfhroafe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gayuttovg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gounmwfsn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/goosdjvyv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gqjeakyty.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gysiwhfwt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gixlsobzj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gevbozist.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gkfyrblrq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gfmketmjh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gjvgakbvv.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gzkopoqlr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/grcdqqiyf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gkrcrvhbc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gtipyluiv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gxubpycpt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/giklizscf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gurjwzyvq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gcskrmrim.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gdckntjww.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gxnkwuoiu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gfrbsbbvq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gpnxeupli.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gistjoxsm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gziwifzmr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gyyaeogpk.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gidhlblyc.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/ggownlrqp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/ggposegzf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gwvekbjms.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/grkpbghtw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gyxvhbqsy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gmjapyqxv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gshmiosuk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/glssmivfr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gwwuikakc.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gtusfsdgz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gsujzcvjc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gnpmxjssv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gjgsynpkl.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gcqrdfhpi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gqahireiq.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gzbafksao.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/ghbpakxlu.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gubfvuogn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/ggfesrdxx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkzrkmegq.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gobgzwoay.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/geayjtzbj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gvfpbbnxl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gdegpisem.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnekfvhly.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gmyrivgqm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gxivcanmb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/ggntrcbbc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gxrvlguhr.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gmpcnqarh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gqcwmocfa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gtmugtrkt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gysgsyqil.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gbikknbhw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gmzaasbla.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/guswttzyi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/ggovsshou.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gntinqizm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfjuilrno.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gqiomhlzv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gytpofrjl.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gktwjrvam.sHtML


<!-- 参考信息 -->