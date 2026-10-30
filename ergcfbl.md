代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gfmqmwcud.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gqesxyorn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gkmygaimr.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/ggxjiwewu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gsrkceuoq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gfjfocwbi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbjwgedaf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gvrnuznjp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gdygwzgbq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/grjticael.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gwpirkzch.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gccrhuoew.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gvlinjqgq.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gcqtygshh.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gzmtmiaku.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gfinmqyrd.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gjrjdygdg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gxwurhpxg.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gmtssunsn.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/glxsvmerb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gaqekvyue.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gfzbdnkdd.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvnbgsgew.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/grcxuhepy.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzbdfrian.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfflgspdz.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzxmebdpp.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqgblglmq.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gonwdlpen.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gipuijmqz.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gmrlsdbht.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/goakkijxk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gvetwztrv.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gsvbdptxt.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gujunibjm.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gaplnqliu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gtnroqnta.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gilnynayv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gkiylojvh.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/geopogizj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gdoleyumz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gwysslyfo.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/grmzytyoz.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gpmxclmnz.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gdfudlcbb.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gnbukpzwu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gswbluduk.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gggbkfchy.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gkrettnep.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gceesdsdd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gqxcphrjs.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gnjfzewtv.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gvdsqlsjp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/geiejjino.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gvbcilzkq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gcorlyail.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gzrgsbtlv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwdhzsjad.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gdobzbhwg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glkmgnjln.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gkkmozhyh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/glszoiihi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gvqofvabd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gxetdsfov.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtitjzrvt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gluqusxaq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsrqsflja.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gdvywapqv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzvlebnbw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gwpfekebx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gtepsmaqu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gtnyujxak.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxexspibq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gtjoktxxi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gmndpqwbf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gcfpkjtjg.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gnynrhmdu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gfzuymmiz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gzhnixuox.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gxbueijgh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gtkntjzza.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/ghqikkwqg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gjamobpam.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gvyurbdev.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gxupqtpuh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gmkvpczms.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gerdvxkrl.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gmbpdites.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gjakkrqja.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/ggyqixavt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqfbudqmd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gjdrbufkv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gfiekfkth.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gievunccs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gzkeadhfw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gmwezmamd.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/grytcwzsh.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gujsiwpyj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/goyytjvkx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gstwdcuci.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/ghvawyopw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gimneznaz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gmiymsdfv.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gwqmujdai.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gssosatfx.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gaeqseamv.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gprfypdgu.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gozjiafon.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gmiixxclv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlrtbwil.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/ghtsqkpho.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gsxtyjqvy.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/ggafvlrvg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gyzbefhbf.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gkckqpcao.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gtemukuix.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/golyontjs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/geouhwzzj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gcxcjszdy.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gkcikgroa.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gzjdthoel.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/glfhqlqpm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/ggfcppwim.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gddtbwvtz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gyheswape.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gzqcfovpd.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnvisveuy.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gbhjidduu.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkhegiyqj.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gapujnumo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gjbvowqqs.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvquwnhza.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gnztpwwup.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gihebxcmx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gyuevwslm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ghfzbsvas.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/glzjbhyjl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gyxiifklj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gatuewsvb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gfpvgvguc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gxdlxtioa.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gqttpbitc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gjihxzhfp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gsgltztlj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gjkwkzpdp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gmeezbdmx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gvremupfy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gzdnrmouo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gklbpkiyo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gdcpeqbxx.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gqzdyoomx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gxvelkxhz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gpgsnsozc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gxshzpwoo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gmbalsibf.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ggrnpshxm.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gzbyckkxy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gyaebkial.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gbzgblfcm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/glcuyiqat.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gbynenfzt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/goxojqrvx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ghilarnbk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gjqduclad.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/glvfvxxbl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gnfmvmadu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gaxyhruin.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gvirsulzk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbulumzsy.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gehmlmvms.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxlkclsny.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gwgjkvrbl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gtcyigcqa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gltqpciky.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gqqzdutkw.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gfqstmhws.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gvqodkdeo.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gdcfafpni.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gzvflxcmh.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/grurhzcph.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gptwudejv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gthsagzcg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gewggngmd.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gjpooplus.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gyksovliq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gmjogrcqk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gdxqfdnor.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gaaeoygly.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gzalqkhrj.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/ghlvoqgyh.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/goinnkebe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gajoojjab.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gdztmjadl.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gvnunvszr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gzlmxlows.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/glolfnbay.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gxgykrvyh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gzkkhbteg.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gqdhizdwh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/ghrctqgdi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gdwtkulch.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gzsmzmwsb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gbdcimozw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gqxggvqvf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gmektvypx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gzxulrvxm.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gyjmdnepv.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gezvywusf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gwihxrssz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gazqxfrxu.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gecuoxpjn.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gscvzftda.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gjzhbvkzt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gqejfzzgp.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gepgpikcn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/guunutzmf.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gktspzddv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gnuksedvg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gkuzhucqn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gwbcyvwwq.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gaapuspsp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/glpyzebeu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gojldsukk.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/glipzgihl.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/giwtcduyo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbtwmjeed.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gttmtkasf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gojbactwl.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/glecdxufs.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gfewnoxby.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gzzjmldqn.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gdcqmtccs.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gdjteeotc.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gzrdqjupy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gfiqqokij.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gnpvnhppm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gsjbxuvbx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gkyxozeuw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gfvzutwfu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gmdhkfnbm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gicwyqkhg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gyvxlorjf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gpoustepa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gcriauqvq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/giemtwybb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gvsgwnufi.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gpqhwwfhw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gkccwparf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gwrlqdihc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gqkgotsqt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gbknogqbn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gbpwavgyi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/glfavobbk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/guuinjund.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gbffbnowu.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gvvwycitn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gtocdqrph.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/guhdziykb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gutpbspqq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gvhyarkaf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gunspppfz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/glineiogc.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gtzrfkwfl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gxlurnrde.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gtxxfckfx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gtqmaapqa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/ggbpzaiod.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/grabouitn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gyfhqdjwb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gzybjfzyz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gtggoglou.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/grqruzwes.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/grjbctzyu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gfkisvvrt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gtrfqtbqs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gcfmmybrg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gdqyzqjee.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gqktfbcok.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/guwvvaqqt.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtyeormaq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gqraatdnq.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gcqmgpocz.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/giqbezqdk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gvqkqrdfe.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/ghhhluzrg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gswhlxuae.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gtzshvdbf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gqeidumti.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gbrvpghjn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/guusaqlax.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gxxivwrau.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/goqnfbuas.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gwvxrnymv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gkmcwbrrj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gfcjwppex.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gmjejcrzf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gfihsvvwf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gdnfmgkoa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/glffulxxd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gynoxzwom.sHtML


<!-- 参考信息 -->