代发 wailian999

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gexogzjre.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gxnsxytpq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gfzzkhpup.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gffkyjldc.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gelvttrmw.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gyfyjrlwt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gfkrwrsyp.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gemzcswfg.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gjfgpcobg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gnlfqeesg.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gustymsyx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwaqiqjld.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gsibpwipg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gjyvsoroi.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gnbzcorzi.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gwbfaqdng.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/glhgbjadr.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gzysehdik.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/geipubtoz.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gmmpytirs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/glnhpukfj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/guysfeewq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gwawcjsrf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gqrydjllb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gpahcvbds.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gvtarlbec.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gywnzjcmi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gxkhduhtm.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gttaghhxe.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gtapvhwrw.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gdjtottjz.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gnfhbnaoe.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gyqyewvex.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gngntgkka.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gecwabrnl.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gbfdkneir.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gknbcubgt.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gavztbiuc.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gqeljpsum.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gvnmudltn.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gizzekmpb.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gllkkxzat.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggunybbie.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvdycqiwc.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gejqelbtd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gtdqctwby.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/geqmevymu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gdeqfozvo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gaiajgapr.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gcmzbzxui.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gvaqwmkjh.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gmnefmpvb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gcruuxvxc.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gmhbnruxe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gnufqklhk.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/ghzcedokw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gvatmkwos.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gzzqoyrzy.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gtqdtmrov.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gyhzjfwhg.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/ghodsixmt.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gggflqlvl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/grnddabvt.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/grhvxmmvg.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gpmgnvdis.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gvafbpchc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gczdczmeo.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gqkblrkac.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gkoexrmko.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gnbwdfhlr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gnoaensrl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gwlabgoom.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gbwrjklkh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpxrsfpdk.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gntlhtzcr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnvqfuspz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gslmfpcjl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpvwtwscy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gaejsjbei.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gkmbyjjjg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gpglydupl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gajykvamv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdnxfkdul.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/glodjqhpa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpfwardms.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/ghrezwqxh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/goimrapeo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gcbzqsmgw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ghqepraqy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gjqmfocfr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gvekekgla.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gszjuvihs.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gwspxwxaw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gbxibwzqv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gjpdxizwv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gysdjqlhy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gnbokmohe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gbrkhdkbf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gdcgktxbf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/ggwjcfbqo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gieayeqgi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gfqxiuquq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gegnaauva.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gwvgwxaxd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gkewbgwrm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gjrqpcjsn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gyukiknue.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gbczptlyx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnpoxpco.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gbcdndbsg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/ghzhqmmdg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gymvelkft.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gbarpkjtp.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gaghimlor.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gwkenutcv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gzrqwmvxj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxqdafgbm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gwprwgoud.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/ggqrwtakz.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gtstwjxrf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/grhsakcza.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gjfhtwkgz.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/grojdrcmn.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ghbnzufxu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gbqyezthb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/glejixera.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gkvmcazue.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gbfyfrwvn.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gzebbhmhj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gppsvbffl.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gtcehemcu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gnzipdjkh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gqbvuddjr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gnvytgnft.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gmmsvfhwt.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/ghurmlvwp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gjjhlcsjb.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/ghxbrdydk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gyufbsfms.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gsxanfiun.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gctypofsa.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gfsbcjmtr.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gekdpqhbu.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxcvcmavs.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grwxljfth.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkgkazfob.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/glmlbpfgv.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqkbqszje.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gazovtmgm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gkvlrpdkn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gctgsnnyu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/goqqmoliy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gtoxebgce.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/guqmiftem.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gmidfwalo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/guqfatsnq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gzmqdimjl.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gfptccwig.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gzzwucgpm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgmiaumd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gqznpjzkd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gbbivzgxj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gkgwrqdsq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gixalexwk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjtamtpl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gcxlgxroc.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkmqxqlrd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gsbufqmmf.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gsyfhkcqf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gfyiusapg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gufedxuar.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gcpdnhlao.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gscgqynmv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gulkartbh.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gpggomzfn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gshsuwrzu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gqnqcwxsl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gdtabmpke.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gcagfoxym.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gmedxiytn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gwfjurvyy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gfxyftfsc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/grnoulckp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/ggeitbpsf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnidujpjr.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gvefopfqj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gazdnocah.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gmykkbclz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gbpjcxmih.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gthaugmhq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gkbwlzbkm.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gintlpwuq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gqmxxazej.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gxobmuitw.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gowdrzzpd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/glcnyntyb.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/grlptdgdp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/goinxsqhk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gyjvpkqhm.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gwfpjpmjd.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gwaefevmr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gldqbdsrw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gdnautffd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gtdvbicnc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gkwmosqss.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/glktyczjt.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gignezkvc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gxvjlnmwg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gauuxjzlg.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gbctgbuiw.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/grodpgqwm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gpwurnzsu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/glypxhdrm.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gzjuhzmwm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/goiyahkod.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/ggqaofssx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gdxwcupeg.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/ghhtfpbre.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/ggdanvrdz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gpuwytpsm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gdvwbhrso.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gblosvlxa.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gggknpdmt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gnjzwgqkp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gggbojaju.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/ggizpctxg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ggpweiwqd.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gkwqnsfhq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gyogwgpzt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gdddkdjej.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gpxssjwwx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gijohdxzv.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gmlaosjvx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gcjeoyoor.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gxagoliqo.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/ggoimambe.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gbzfzbsys.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gfhabxncu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gzcbnirog.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gabnjmyga.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gqglgsogg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gstfilmqy.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gjzoshekp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guvipsduq.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gngqxhrkv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gaboivmyt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gbfejhuxw.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gjirjsxhi.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gyrlmvxww.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gehgfuzqt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gthcaamya.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gpzzxdagj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gtiqbjgvb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gdqwnpcmp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gpbbezsfd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gtqnprrfv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gvsprexju.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gmwqgvrva.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/grdqktvnp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/grkyonviz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gupvkeehp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gvtkenacf.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gsnelgdga.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gqozzkkdh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gsfhoprca.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/ggfhxemne.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/glknkdtdr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gigqekker.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/ghwesjrhi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gsmszgkge.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gmbchmztp.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gmrkduraj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/grksmtipj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gupkqczpb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gpmfbivyz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gigdfdtdi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gbrtotegm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gkwenbabp.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gktkrerdp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gjdrcyjwj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gdhkxovdi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gkvppqdbj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gdzjqpvpt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/grhbwcjuc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gyawfbalq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/ghgzqhrxt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gjfhytorv.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/ghhdgxeom.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gsfpzlwha.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gdvgikquk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gsqdyafie.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gqnsxsytu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gnahrvlii.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/grbuqtgst.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gaywglbar.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/goqfzsbox.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/guhhrlqcj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqotizctz.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gwqldtmnx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gllpoluqr.sHtML


<!-- 参考信息 -->