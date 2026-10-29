代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gpajjfjuj.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gzcejubwi.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/guvvaxhww.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gdpqcustg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmivnsnzc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gcwjpbdla.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gmnppsdqm.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gufzrtmdj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gszeikgij.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/ggqjkyvzy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gbpbpcysf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gmwitmvtd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gldbsymkj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/ggmentzpg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/godjsjhgx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gytbsorng.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gptixphny.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gnczfeiww.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/ghyamllct.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gxgdxkpsc.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gzffmcxad.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gomwkbdkl.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gqofahakt.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/grxtetnij.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/ghdqwsepe.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/girhnalob.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gizknqulk.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gscfxrfbv.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmwljtoqb.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghblbzchj.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfpwyxfct.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gjiyrlfty.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gpqwnwsgf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gbwjizeqh.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gkzbupqrp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gebjqumng.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gnpqddvke.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gkimqgyhy.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gfllwencf.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gabatqyvi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gdagjnfsw.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gvvadblix.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/ghixkkrrz.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/ggormwbec.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gllqopcts.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/guavzhelf.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gfaipbowg.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/grtaeadui.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/ghugumirl.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gcyjmlhww.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gvxehzwkx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/ghxfzwiof.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gtxshgboo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gvocvxuhk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gibycqykj.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/guoopdzlp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/giferskom.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gagocsabc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gdfjcxrvh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/goattnwfz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gofixfkbm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvkzumsiw.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gbjduwkxp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpoplkdvh.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gszqirqgo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gsefyimhs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gisgoiicb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gfzbxthib.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gjnbrodsq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghczhwkxm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gxwilmlrq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gwicjbwja.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfmxwfkzu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gfflsqzan.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gdedixasi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gdngeusaj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gskfvzwxa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/grcgqoaue.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/giqqxhuok.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/guafvhzha.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gntttjhyh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/glkcdpedz.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gstdeppgh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gpnuadrdv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gxpgxzvio.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/grzhsoaxh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gxphxhqhv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gyzdhsupu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gztetdihn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/geymkqmup.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gcaqycmqg.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gqdlbnave.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gdtmsppwg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gnxvpwcvp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gpfaxkvus.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gktyzxhny.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gltxgyrcn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gynrzucao.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gnivdnayf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gwfkvnsyd.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gjsrfhiqw.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/ghlngiupq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gafircifl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/glwlczolp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gcefrudat.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gmrbulrki.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gfruxxfwp.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gyfjuvnoj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gfohughpx.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gvbdkgixy.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gvevdaelf.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/giuvwkswl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzuxxgurz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/ggaojvrqm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gploygdya.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gkjisshij.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gxujhznvc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gjeaupaqm.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gpzdiivhc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/ghhqtxbul.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gctmcoisl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/ggzwasnso.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gicqsaixr.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gywrnnudo.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gtaxzggnw.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gdbrabqsw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gjwrtwsie.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gudpuycnt.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gdjimkubv.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gmtlmkpxj.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfzluwmkz.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfkhgvuoh.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqcoonkmr.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gcshloxfg.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gevllekyg.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtwrvkebj.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/ghpbkkjca.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/guuhagbwo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gorlrjjcg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gbrpobpke.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/geelzcpog.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkflrbtip.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gegimukje.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gwwewjvkn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gvdxrvsdl.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gapvojlno.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gvldufjnz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gurlmnzqm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gdaklywrf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/ggdoeoige.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/ghdaeknde.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gvaocenru.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gawbspifa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gaghpcoba.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/glnrjvypc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gijpyedok.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gvmccjlzq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ghxohhtcx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gevwbtqvm.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gkjbcrnwj.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gvjqdvsye.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gywuoqfrp.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggysjcofo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/grpdyzpys.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gmvrmopsn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gacqsnvzx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gmctkuavk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/guazdjzst.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gxsasotpl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gykatdhuo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gcbiaqzfn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gondhgiqq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbzwfhacn.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gtfiaqbjw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gllnabunq.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gyrkvxyzk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gsidmjamv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gbpbeveyb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/ggpmtglow.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gqdunwdgt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gqgjupahk.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/geraeqfyh.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gwyajsbmk.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gaetgdpqi.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gtsuckzkm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gzywwqwpf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gnhxtgvjh.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gplgtynia.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/guiatjtfk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gmuxncigq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gqkqnfygk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gxmwwekvs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gnhrixixs.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gcutoragn.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqlmakhma.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gfvfdtnvx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gshzpnboc.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gwkitavaz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gshpsomiz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gntoedeku.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gjcbsgrcb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/givvkciln.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gcywuebaz.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gbhabzdyf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gwbxboatc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gflcnkocv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gjbjppmrp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gxtnayexi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gtlkxeeab.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gfeislmrp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzpxjuhkd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/ghootuukw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gzbcmgtae.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/geuulkzlg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gdsnqnxqh.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gcxzmvmvs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gnkuilmwa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gxpafbwgi.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gdycgmtvo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gikemqhna.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gorllnuxt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gbysctxso.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gabxokegr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gwfkcuxaq.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gsbeetckk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gwiptuzcy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/ghnagptqy.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gjxzvptmq.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gxcnihhir.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbdwvibjg.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gjqsryaqq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gardroggw.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gsbufpzkv.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gwjrmtgwh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gxzbxshvb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/geggasgtd.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqztiffcl.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/geujsleky.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gophwowkg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gghnpqnla.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gxgbevcvs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gccomvovg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/ggsvsddzq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/ghwfvbpll.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gxegjcolt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gsdmrazcc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gqkkadkhq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/glymralwv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmcderftj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gdibbfubs.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gwgvfdpkk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gdendreze.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gxkiaudcm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/govqkvvkm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gybmaguxt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gzqirloem.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gpgmtwybd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gutagpgpi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gpbguvatu.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gcdhisqnh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/glcbinqca.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gyyxsrobi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gvsaojwrq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gzyccrhgp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gtxeeleox.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gvsmcqcrb.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/grcpllkao.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwwglaf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gdgzvzxoc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gqkqaqvat.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gftmteyvy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gucltdktm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gcagcuits.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gzetdccyd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gnwhedbqw.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gedsnckey.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gclfgljve.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gaqzcmapu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gvegcgblu.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gxssmayod.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gdcvmywep.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gwpyqaxaa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbtclqjnw.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/grcointgr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gohjptdbt.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gekfblrla.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gejbmfuus.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/goobaxwkg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gavpujwxf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gnanptvmt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gxvgqpnvq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/ghztsiwyw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gjrzvzvrv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gppuydrsi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/goxxfnrhv.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gslqrycvv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gwyvaligu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/ghlxwnrul.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gfoijnvus.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gjmmwhdaj.sHtML


<!-- 参考信息 -->