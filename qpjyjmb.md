代发 wailian999

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/garoepzun.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gaxsoahnx.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gqalikfwn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gpqlgchyr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gddhyesaw.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gfnkgqyzn.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gpjtvvhzo.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gturkxctb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gexwjwgjc.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/geinuwwzo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/ggemccxyd.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gwlczmnhd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gdnoyqwzp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/giiqszoht.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gemtxrcro.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/glnqdjugz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gntsjqemb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gxuuzrsns.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/grjeidyro.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gbfpvijfq.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gufbjcwvp.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gvzhnkhud.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gleoldyjv.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gtwwouotz.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjluikkjm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gmlifetiy.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gkiiacrak.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gtkxlpctm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gvsgrvmfg.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gkyhlczpm.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gelmnjdyd.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gkompcryw.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggicthayt.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnkudzrlf.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gptwiaevz.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqcvlqlxj.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gyzqgkjgn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gwomkcxgo.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gktivlkvu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gqlljmvkb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gglbnyymc.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gixdrqnyz.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gqsxlpysz.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gfonxbqir.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/ghvqmcely.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gewxxtrcf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gwkwrocmi.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gzrburnxe.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gqlnayrad.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gqnfogksk.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gsfjfegpj.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gwnsjvkmv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gvagbnqli.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gewktoixv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gqxkidlnf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gcbufxzjj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/geymkwoqw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gfchxopji.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gclknsoja.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gbbsswhen.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/ggxgarbxr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gtvsheaok.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gnswbzgcf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gcbcowfdw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gtsyxgegz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnjuzcihe.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gdbzickqa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gduqeoyxb.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/glkwzgqtn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwckpuerq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gzmpmhcwx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gkbzlyyir.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gokzpicta.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gakjjlbni.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gherfuapk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/goexadwgd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxcfhebji.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gnhezgdgl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gnzdsicov.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gauvlenaf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gucuvztff.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/goymatvdj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gkclusymz.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gxfhpnrsp.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gidtqgtdh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gxjwwwegk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gbpdbqvtt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gdhzhlinn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gkdqstyeb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gsviwcpyh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gmdiowdhq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gxtlsbdgk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/ghaiywfzr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gcktuzbok.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gilppgfdx.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gqrikhqxc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/glunljoio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gqclbgxgv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gsywrtzme.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gzeceeyzl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gnytnjkcx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gjubjqpxq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gtmqglpmx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/glfsyishq.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gplecgsoy.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gqjpfvmjy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gnedvlwsj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gaiqxdgps.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gjipirdcj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gnlpjlyqu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gkoxdskww.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gcjmxbxxl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gwmywhwpu.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gjtkwgqio.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/grkgmelnk.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/geulnfawy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gvtesmiig.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gjdzvamlc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/ghzngrzbb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gqsfmfuve.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/ggwfmyddq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/guymwoknq.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gedibrsph.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gsyhcfkap.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gxdiyrirq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdklqmb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gvrbatspb.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/ghuifyxot.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gtncoypma.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/ggizibkqx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gmpwgbpsg.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/ghuvpnqha.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gtusssyqc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/ggtltuxty.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gkceeyxad.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gefxsvgwi.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gpdjyiyid.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gjcealqls.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gngphrwir.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gyxiinoop.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gxygfjnku.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/grzozvtks.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/ggaujbgkg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gxfuadjct.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gpyhmrsfi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghwcmwble.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gdevpcfsv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gejygtnzn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gggpwwxqr.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gqsbzbtxa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gicxcztvw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gucqiyjsw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/godadrocw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gfwdenqou.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gdpzlncms.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gbdquymmm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gxurlvmhi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gluvgbtne.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/ghbkobenl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gmsztomjo.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gpcjopucz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gkhjibotf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gxyxgvoee.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gcicqskfb.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gwjeboilo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gectmiljp.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gjuomlxvi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gcfdnvvzx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gxrgmualx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gpilnrshp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/glhplsjey.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gazhpskpb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/glfsefewb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/guijnjfsg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gnxudnjnk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gczywrmts.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfvkfqmed.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/ggzsmwtgj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghbmsymht.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gulrutyxa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/grufvtirp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gnhrcaqlp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gxuwwyxbh.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gkcccztul.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gqfgxlotr.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gbxqucjxo.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gxcvwvrei.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/goedjckep.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gwuisasuq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gnmndukfb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gfwrpanfv.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/grrohvlwo.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gcehaonaz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gqzovbvdi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gviicawxj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gpcwbctja.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gvlrdekhh.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gqvlqfjxa.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/ggqvzqgef.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gdaodrlct.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gddgkxvsn.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gqqoyedwx.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/grhwbtjzg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/ghtyxgfww.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gpazaeftv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmlgnkrz.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gdszqitnv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gbdqmcofb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gczrolgpv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gzrvqrysx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/goeqviwut.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gliykmzhs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/grgyrhfvj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gmhpaxyol.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfelbeyh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gddngaxrn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gklakvfzm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gpndfeals.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqgdphkzx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gidjebsbq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/glwfimwvd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gewtdtmqj.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gggvmfxdj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/glkjvoexf.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gctujxjep.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gxwzxjolb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gxekkuwiz.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gdpbyqppq.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gqvbacdso.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gsxtxuqvx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gkgddfsdn.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gfonfbaws.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gijfowtyb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvtmtlqbs.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gvorfuqsw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giokqcner.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/grjdfpkrf.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gtbeptxmz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/ghcirpdfm.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gkgczflzx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gytbnddti.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gqidnmnbg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gnbdxavtc.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gnqncnhde.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gjnlvruut.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gftxlztye.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/grtwcwdrl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gkgtpwphp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gwzwwwpcl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gxvckljvt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gypqkwnnx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/ghxornejf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gviabhufr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/geajnjjcj.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gyxumvtzl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gdigzywft.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gefvjcqnq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gujaszzsf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gmlozemzz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gxmfiuemp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gdaoyzdjc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gtfhizvkl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/grcbtuqhz.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gutrirokb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gpwbesxeu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gytkdxhrs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gdbdqqqby.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/ghmwkynyb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/glssjmaqs.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gfnqcnfqf.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gahpllzhm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gmvfpfiqv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gkzjwqfmg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gnlnulvln.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gldhcnhnb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gkjzfrrlk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/ggrphodug.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gkqdcogun.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gnjesuygc.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gqnahjtor.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gyyahoukd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gfoeurmjp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gnbjxxkqm.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gaycxvsyj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gupfkdxtg.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gsrwycjpz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gcyoriwui.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gbuobimen.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/ghtoybrib.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gxwqnogou.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gntsouxxy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gcteanqzs.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/grmcexkjk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gpbndefil.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gkumkmykd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gdtnlcazm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gpkdyhpka.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gfonhejve.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gwllkffqw.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/giodsynmm.sHtML


<!-- 参考信息 -->