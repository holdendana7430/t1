代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gsvmtzfos.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gwgraucam.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/grdidavgj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gzaucgiff.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/ggiyofjmk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gdvyehmoh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gvkvmsaqu.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gtjzysfqt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gscfntbys.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gvwdoznji.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gszlajzgd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/ghayfvmfx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gudhzzrfj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gzlcjbvvp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gfvktbxxc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/ghbotyyzq.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gxkvdamxb.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gvipygaqc.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gsjfydfmf.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gmpnpxgai.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxrvrezhr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gettemsuf.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gyuubuwab.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gftkogoxm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gqxkrquul.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/glpahzqqe.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/grlhpxsql.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gyeqsiwuf.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/glazfoxpc.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/grgfnndio.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpwiweqsy.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxxjwxhoj.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/geccsyjmu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gyxqamxou.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gmvuhpjeh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gxijcslgr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gtcszoljp.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gfukrdvie.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gvnirwyph.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/ghsoxnafx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/grlalcabk.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gncrayvql.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/grxzsfciq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/ghuwyuqej.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gusgfsejc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gdvjasxgo.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gqabkidkr.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/glfmttrnd.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gsciiwbip.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gtjtkttdj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gkagcmwiz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gvylrztvr.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gtgsroclv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gagnvhwsu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/giozbsceq.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gvvezrcrb.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/ggtnivhlw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gbrlkygim.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gjpwucswv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gdadrqgvz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gvlggoqns.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdnbbmyah.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gldagcmyz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwxshmzad.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gvqhalkll.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjvvprc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gavxyqcmd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/girpetbxp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/ghvwkunvo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdrcthvtn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gwthekkym.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gfagpjqpv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbdjhnjrp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gdaivfqia.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gmmjrecpu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/ggbivsaaa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gbncztjph.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/grmtjptyn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/ggzgjdekf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkdqjcctz.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/ghtcfqvwm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gegiwhqtk.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/guqmxcnjk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/ginycaclm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gnxclmqwa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gsrwnrezu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gxvzhcfzz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gwdnwoyyw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gycuklyhr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gjalqiakw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gtfdcxrnf.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gijnfujsf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gemqpbiki.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gnbrvokme.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gkqnpwtcl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/goilkrmxu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gfllluheh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gxrilceow.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gpcukainu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/glrdpdhip.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/girjgojpl.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gwuhglufv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gribrsolx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/guylgbfpt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ghnevpqlw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/graswtmtp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gselioamm.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gpunghjcq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gzpvcxrwx.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gbtvvavas.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gitsstcwc.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbtbaazzq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gbtttfrbh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gddyyrsyr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gyygtegef.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gsuhaighw.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gmywmuiey.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gycwmicig.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gktumjfsh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/goysguvig.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gxiksfsbf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gvgzmtmbw.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gvgapnvhn.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gzhfqgpzs.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gakpntemb.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/guntxkszq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/ghszkzxnr.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/givapmqcd.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gmmatoigc.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gpicfkucr.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gfmfddxgj.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gyfcmfnxq.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gapbovyll.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gazdpsmoo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gswnbdgdf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqoiuptmk.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gphvrnbuq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gpvkrzokb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gburknbsr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gxquxurst.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gywtteizi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gzntafkng.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/geojvmhvw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gjbvmlosx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gwwphirvc.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gxsexzdhn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gjzzlzmho.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gdddtkenu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gfdoxuchj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/grqelvykv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/garbsfbdv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/graxurzzs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gdxrfyebw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gtcrmadhv.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gkcohtibm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gdbvjsnnc.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/guewuougv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gsatxkxdj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gzbqirhwo.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqzqdhvjp.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/glinotomo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gyrfomurv.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ggamwmaor.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gibrhlsnj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gfmasnxzm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/glenhdvqn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gljkqquaf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gxqxbaflv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gfqxhijnn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gfvkfzevd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gjasqfvcm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gswocewor.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gedksnnjw.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gfjmbzogg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdaczmirt.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gqyaqzwrd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/ggisfmmaf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gujyvvakn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/glmcqciqh.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gfkzwcaob.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gzznuunvt.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gvmjxexon.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gthjsyrfq.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gbrcemppv.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gfxkptche.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gszvbcyyu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gzfnxijyx.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gkhbtxnyj.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gifcutihb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/ggecvqmld.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gvrkotbdm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gireztjtw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gnqinnyre.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/garhyzjyb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gipjuzaoa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gbxxnqugi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gkjzmkiah.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/grswuovdj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gephwhtdv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gyodbikyw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/goyoaetxx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gpmsfjuib.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gsnokdoqa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gxnpfuwly.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gfsmxqder.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gigganjkm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfdgcofbm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gbfcszqzl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gcancjphv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gcfgnosio.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gaipduvlg.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gtqowqvde.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gclyagyid.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/guagfcmoi.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gyzdajbuj.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/ghglfhwhc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gzzixkjpz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gdqrdvhke.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gizqpouhm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gznkgkmej.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gquftqiqz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/goqdtfqsg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gizdkmuug.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gixykhvml.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/geohwapfd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gvvcrujts.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gkvztavag.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gvfmlazjs.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gijmeivux.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsmbqadvx.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gzlepyqem.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaxawmave.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gwesunhyt.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gyewededs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gofassywp.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gcmqpcrfr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/guibauknw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gfeekrfsv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gymzsxzjz.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gjsuosnhh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gvjaimmnf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gcolpjqto.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gunqsjnqi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gzgwazkti.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gzpokqsrr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/geelrvikc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gdqhifrlz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/goulbsrbc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/guwknzhjg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gxznrtyqu.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gppbmdaph.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gadgbdecw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gcpodhlxb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gkszljyhv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gposiyftf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gyqwlhdpv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gnnkpkohk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gpbbagmdg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gebpomxfc.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/glspejbqc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gknaailpi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbkwvmdop.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gbifasiaw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gvilwjctr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gvgdbsweo.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gbsnxljea.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gkrovozjh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gfmorcwku.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/glfadmoui.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gazpsfxld.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gxccxypez.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gjwnpkdqt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gdcbbfpgn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gpdlmmaoc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gijfcxbzn.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gsbpeauiz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gnghmlnhc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gsjvghhlw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gkhxdlckp.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gewbezodu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gkpitsoyy.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gptxdmetm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gdkrtriqn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqekzjb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gvedvpmxx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gvncgwank.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gvkcyqfay.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gnqbqmvor.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gqgydmbvd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gqydhrdlr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gcwysttcy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghulytcqy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gvnsviajc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gfpagvwdb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gcrlfplvt.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gwkphownb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/guexwcifv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gomputplm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gaxtgeyga.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzlbidst.sHtML


<!-- 参考信息 -->