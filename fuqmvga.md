代发 wailian999

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gtuibelqe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gzcxcsmmi.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gnieapnpp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gdlruozcx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gpynlsjue.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gzimoftgt.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gccoqeami.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/grkqxpnom.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gdangsmpj.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gjvkwdcdj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gkodygorw.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/guytulcbm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gwkwqnmul.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gmafzzmqi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/grlrbvqay.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gynylvvxa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gwkvvvdya.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gxrcvumwo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gtdyktdqa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gsxnxblfp.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gskickxed.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gbatypykp.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/glllmmsji.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gjpgybwcl.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gcbazbvmn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gctttujna.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/guyawmcfq.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/grklzqazb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gswelsekf.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gvefnrgwc.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gjnxpewwy.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gusodmwpf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghwayiyew.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzcfrpmpi.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gfznbzvyx.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxfuovwcc.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gkueuqjxb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gonplwral.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gpbolgxie.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gsesvfeim.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gflpwyilg.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/grwtkrfhu.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ghwzzyfng.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/glmqytasx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gnwwujfib.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gdbjxpbfj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gmhuhzuww.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/grgjgphbu.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/glzglwtbi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gzmewrpyx.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gpscltbeb.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gslcscltb.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gvxjcmarp.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gzzuvveuh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gzhqhjznb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gksnjutva.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gelzotcjc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gcekgnici.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gpojpykit.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gobgxwltp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gcjcwxczj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gptryteno.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gnjgddfhq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gmacvnvgi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gguhkoowr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grdboyche.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gkvafgvgt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghazvgnfk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gaoceyrih.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtshmavbf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gtjjeotcp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gjbiyjrht.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gupdhxxfc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbktxscjm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggisjzejy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvdlstqn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcxyivon.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gtwqxteez.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gkyxnnumv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gtvouxbqk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gqxdispbg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gxvzjkxcd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gszwydxkb.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmixznwtc.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gvayqpdxr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gtsxqyvnp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gtlydtilh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gvzkcnbmh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gvwgfdlty.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/ghdwahxut.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gybhnivff.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/goiimxefp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gematgrxv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gplturswb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gleqqgvgz.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gcryejjyk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghuxwbxjy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gbirveasx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gsoeqzlgq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gyccfinds.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gpifdongh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gfocjbiri.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gxkfnoyxo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gcjrnabfz.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gkluxlndf.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/ggvfrwywb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gejcrtopm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gtmfzocpg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gzmvtdjuq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gvpzoyloc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gijzcquth.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gaznuhxsc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gtusrblor.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gtvnuwfxi.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gfqrdahtb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gxbihmxfd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/guqlugadr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gjwcwnnup.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gupflyukb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gfpztlxtr.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/ggbmnykpp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gpjhtacsv.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gjpcpkalf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxmsmqn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gqnlhetgx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gqyzmvvrz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gtqduqwnl.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gyhlymira.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gbleikvnw.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gfyxosjzj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gjowvfeyl.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gxjtzewke.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gqevbfgcl.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gzttsecww.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grtuwyxrp.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjrmplmfp.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gaelrnxfa.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnogebdnm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gmxfgfleb.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gzbfjsauw.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gbqauhpfm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/geovbrgor.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvuzlxgfw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gperyfnnt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gskpxwvfk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gjpanmygk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gfbbzlchv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/guosjryuw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gehxbqkpu.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/goktuqdau.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gyjkrbvbj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gbabvixfr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gegsxhzbp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gienjquxr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/geakprzeq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gerafyqla.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gvvpbomms.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gccwusejw.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gptzebvnw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gelbpbspf.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gevspcaxz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gmtejnvdw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gubkeholt.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gkqfkoowj.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gqxcqmbrz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gmihoboyx.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gzhvzgrpe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gfaswttey.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gfdgrosch.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/geqykexwf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gghshpfmy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gimkzytty.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gsokrefjg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gwobgyvzt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gjaxtruqc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gucwwlizu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grwjhrgtx.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gmldxaftj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfmmfygpt.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gunbwtajs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/goalocklg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gsuynntdg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gmkqnenhw.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gzbujynyg.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gdsuuucbx.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gfkhuffwc.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gdpnrmoha.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gozawaxkf.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gtxviqywt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gykpbfrmm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gkbzcfhsy.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gptljovtp.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gmzvzzlcn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcozgdqni.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gsecfndph.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gmlxnkzru.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gcxddnaqm.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gwolhymve.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gzhzsjenl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gheviwnoh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gufjzppgc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gvzyblrul.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gggyycotm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gthqtwvay.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gdjjzpawm.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gmdfgbiuw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gjrgpuynf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gmmjlquyd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gpgzwyuak.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gxgvjykkz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gdkeabgku.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gsvxejifh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gcyzhlqmq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gjcwvwlzd.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gfwquopwa.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gnbkuqktw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gomyforuf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/grmeviybn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ggemmhmkn.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gqwjhqdky.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gekcbvcpa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gkqgnskas.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gnhipncjx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/ghrpojwzt.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gufrmjupm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gfsugrdkd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gajoctbpb.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gldhkwmrj.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gpxdtthqz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gkicnjexo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/giyjjktjo.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gulsygxnv.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gklviaulr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gntepcuxz.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gtzpkhoqi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glekqiesg.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gedlhcsdz.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gorpmifvs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/grjbgyogc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gzihbiizz.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gustcdzxh.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gwhpfncjg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gpepdhdxy.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gnwkmsidt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gsxdcwleo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gjryovnwq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gmzqhmiao.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gxownuaat.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/ghkgldmcg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gponobqvz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gmlucinyf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/getasiulb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gcjchqdux.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/ghnzlgkgn.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glzxgwcop.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gbmimisxf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/guhcepgxt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gfohfjquy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gsvejubmk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/ggwnucynt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/geazpgpnq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/glggztsve.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/ghheuemoh.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gzjxizqca.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gfmydwlal.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmzjpwfwn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gyrttjuoo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gypalnfuw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gymudnmfe.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gegjxgpij.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gsovlzsvk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gdimfckkv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gnbwxbdsi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gxqpbrtot.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gnvdtuwfd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gjboxqakq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/giivagotj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/grspyyrdl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gjqwohgyk.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gcqzcwkiu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gebjqdoob.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gbcolmdyc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/glgrktnao.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gsxgeoked.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gginctmxv.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/garwqiuqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/groxxkvbc.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gmfnoirwe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/ghpoubosf.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gcyagbzus.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gobbuwtaq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gtyrjytcn.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gsatyusgs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gaorjzhbd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gezpoqjpt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/ghxbwqbpo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gcxrlywxs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gxezzrjub.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gjquouqub.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/ghelxnhwd.sHtML


<!-- 参考信息 -->