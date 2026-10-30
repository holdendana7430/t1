代发 wailian999

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxacfyhlh.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gkctbjhxd.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/ghhxkzsaj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gxcueisgz.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gweinumer.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmaengjdt.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gmrwhcssd.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gqltrqtog.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gqubhmvwv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ggfvirxwo.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gekuqiozj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gtomliiun.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gtvmlilhr.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gcoszmnbq.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gyiuszaxf.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gberblkcv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gmfjuzaza.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gkupmpxsf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gpytvklgx.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gjtsfejst.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gzznnxmcq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gyhciidmn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gouwoklmp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gfwiiaauh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gtepcxngi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gjmsgtvgj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gmnaeqjtr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/ggktuhlan.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gtyjwsrqh.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gkimzuukj.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/glaexsqlx.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gfhhrowws.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gcsdwttjf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gfdpgrcuo.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/goujhhpvm.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gzzsgdmpq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gqzvrwldy.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gktaddtvk.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/geeakymss.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gzehlfumr.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjxmkbdhj.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghbjnofpg.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gzndnzdpy.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/ggsrfgchq.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gjcigzffd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gavbfmmjd.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gdwhuparw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gxlbszbne.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gbxhehpot.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/glrjpndkd.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gbzhfxrxb.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/ggwgbtxvd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gljwqogdy.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gasthtnfw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gxgaixqrt.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gqdajomrd.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/guiwcebhn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gtpqdprbf.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gorjlrmxh.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gmijvbqms.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/giikwwrwi.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/ggfhdwarq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gsoxcwsvx.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gjizqddwd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gezqdvufi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gneschzee.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gkmkifadx.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/ghbbjjwzk.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gjgfanqzt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gnmcglfvp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gkotayesr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gqccymeja.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gajukaczn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvwwtubju.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/ghwhhremc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwhvbwnvo.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gcdjyoufs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyshtxvos.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gcddrzven.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/ggkpawlvr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gylfzhqhv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gcmvuxvbg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gkwvvofhu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gtuomagbv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gaggiaafk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gksbcmdgc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gvljamped.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gzqtzjaqs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gkzdoekqj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gsewlhxtg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gubofgzep.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gosqluegk.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gdyeajcwv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/ghyljiqgs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gvcgljuhr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gwsiylrcu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gzdubckvu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gaxsvnubd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/ghzphxwrq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/ganwnrrja.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gxkorfgqy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/giqbhqrkn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gesggxhav.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gkqpuilso.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gheehohsi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gxvdimgmt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gyofppyzj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/guksuounj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gfrmpazgx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gtiwhvhcf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gumvshprz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzxdksozh.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gajqsdodz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gxjvwahds.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gxsipwydi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gsjfbbloq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gxlqeceph.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gmeeggril.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gtowvzner.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gyepipzxi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/geavanpjl.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gqebterzn.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gzlvxjqoi.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gdmidpprh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gazidfwnu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gmekazjjb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gjtjcnzxi.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gefmosmda.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/ghmfglhue.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gtbcwwzwf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gcamrmemc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gqvivnshw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gwdvvxbpt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gjjuksrij.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gqjayrcuu.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gnshpxutz.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gprcbhjsp.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gpklinzro.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/ghuqmcujs.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gdjrbatfo.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gcxdjtyxx.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/glfuzflac.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gacalqwxy.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gasixmjoc.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvjxgtioz.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghjmbzmsq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gqpxakgmm.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gmuudnbce.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gevnpluvy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gvsfrhndc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gfcuyxhuo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gfbtptyag.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gxayobonl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gcceeenxr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gtbcpewfp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjhhmcjnp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gfpyoiepz.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gblanstrv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gwvpkazuj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/glqzogvze.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxizqiadu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gyjybbxfo.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gbuvgpdsz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gihpuxqqs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gxtslsnai.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gukjuwmsf.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gaoyrvwmq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gyzhgxhha.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gebncewlw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gawxyuput.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gwwfmfrbh.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gmaqvhrlw.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gpgwvgnpo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gwjfbnpoj.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gblveseeb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gsucillxe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gwvouztim.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gauuyzrqv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gkevjaaoj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gdwimgytv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gvyebhohc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gtycyzbiy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gerlgyspg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gjocxreeh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmsuqbcbh.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gccqmfled.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjghrqean.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/ghsxxexap.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/goihxhano.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gwsutflmq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gktiwhdnq.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gohnqgedq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/grlragazu.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gfznmsgft.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gzyceiass.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gwzcxlrnd.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gkkynjdqr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/glscifvlg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/ghrltdcgo.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gjzrsmrgn.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gzujgcjdy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/grggsayrx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gblvisydv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gypbgdikl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gthhkfqqm.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gattysupm.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/girnfrqwy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gkhwznfor.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gknaqzvkg.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gdglvwbkx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/grpecdzid.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gtrkyjhwv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/geikezgxd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/ggzgmoidr.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gvkisexvv.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gweqkippm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gmrmellub.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdhrneoig.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzyrxgqko.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/getmfuxfz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gkbwaybqw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gbjtglyhe.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/godonuoab.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gndhylhgd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gbuxilxig.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gavszlevp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gegcmclmk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gadcthffj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gjlqaytft.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gezvkktva.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gcxguzsto.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/ggwxikzcq.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/giafhinkw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gqjqdgfyx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gspdccveh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/groxmkjfr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gxohymuka.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gkgnivjti.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gyqbgyhlx.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gpgwbfaue.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gmrsfarbg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gucxumzpu.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/ggbsplkjj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzacrmyzj.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/guxzdexrd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gxzfyygqb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gfyvbbdku.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gndityrrv.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/geaggylko.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gvlfsgbys.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gwbycnisp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gdgboenfb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/ggvaxxbli.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gmhqccxkv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gcumpxife.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gdfmaypgk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gweemgund.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gwgnoznmg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gwaxvmxtr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gqrdzwihf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gdvataybt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gzfhsxyid.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gkvlxtljh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gogiptslw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/grxikujkq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gjnydkyrr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gtdvuapba.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gyufzfhmr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/goepuuvce.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gitedgzyx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gndsfutqy.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gmiqgtpjy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gxvfycaqi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtvcryyrf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gsitvfeht.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/glcynmejz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gbsihzigc.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gcqdmcobf.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gjzmyxwre.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/glgtitfuw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gqgcndugd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gyfunxadx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gwjwkavxw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gillzgclm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/glcmibenc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/ghspkcukl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gfveuirof.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gfbqodurl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gltsxdbfo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gbjsyrbqy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/grckrnztr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/ghsrasfwi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/ggfpgzvzh.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/geefhwppn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gdxgsxlnp.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gzprzverc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/ghculhuvh.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/guusfmkfs.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gwjwgcfbk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gcahpzygv.sHtML


<!-- 参考信息 -->