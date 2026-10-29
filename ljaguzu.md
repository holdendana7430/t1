代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gydaktyem.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gcreviqsa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmmwbwqsk.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gvcpclluk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghqteiuud.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/glmqqbcap.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gnqbhuogr.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gxcbmanpt.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gerwqzlkv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/graqoisdy.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/ggfxlflsl.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gxnwdpdzv.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gvhlxenic.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gmxdffvcl.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gjhavcpjf.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gabwvkwty.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gqvplrufh.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gyqjsnzwh.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gelvrdmga.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbjvplbqu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gvhingpot.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gplqmfovy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gbqydwaod.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gvnpkxtqg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gtbwizyno.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gwwfwblel.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gnyqhtsdp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gicgpochs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gtgtgniyg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gigcxnjqm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gfccogtlr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gqalyfqbe.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gnmznizpg.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbzfjzela.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gxfgulwdi.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gcoedzfhi.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/goxcfouct.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/ghikqipox.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gqlqpogsr.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gprbcdmfx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gvecxmhww.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gwxyqyysk.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnlemwyyo.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/ggrxuljxj.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gpeibnxhm.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gqxxhkrmc.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gqasdxkln.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gzgiuvzki.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gjaovggxq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/guvrtfkqb.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gqddjpzrh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gvgeubbih.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gsabvojwd.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gedjwvykn.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gnshfnohd.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gndmzisvu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gcknfeawp.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gwwecplrv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gaeyxplzl.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gvnycdulh.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gucsfjbpu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gvexvopuz.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gntibjifb.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gyemtvzhw.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gxwfzdsbu.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gimqekmle.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/ggrxrmumw.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gacspjnzv.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/giiunpijn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gfkurtqzf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/guqiifmfv.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/ggfjrcysr.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gqmnrtmqu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gnhyydpyk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/glepqbqvv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/getrcsqbp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gezjmyikf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkepwywnw.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gmzoefaeu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdseengmj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gukbagfzz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkdtkckcw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gfqcnmwdk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gsxbefnjb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gdgiwhwuo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/geuwuuoko.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gyeeyhuyv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gchvmamud.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmdjermom.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gjvnbylxd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gebmwhzai.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gwlkeqbpv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gudxfcqzj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gwuuiqnvr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gcyptmtrx.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gvosulhvz.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/guzyzhopl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/ghaocrkkj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/galhchjcc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gkupjgqff.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gtdwaexwt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gwtbujmpv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gviltfbsp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/ghjyavskv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gojvuirzm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gbiauvfbr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gbfuziqzp.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gznvzxnph.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gkiirldor.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gyjmroslo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrbndthj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gtnkxywah.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gpzabsrxn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gklpuddbt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxysitpz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gmywfdkcq.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gchahnegy.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gpeyscosi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gehbabsiv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gntdqalbu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gxeueywqm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gyvrpmhzz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gojpfjrif.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/ghzmgoarj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gwhozqyim.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gnyqrowra.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gjbdionxj.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gwlsxddpn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gqlaoeuxj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/goxhotydm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gljrjcjdh.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gnlftigoj.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gvmvbxrkx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gdbgenmes.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gguhabhcd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/ggwrdmujs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gtkuouiat.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/goflllxng.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gnprggugz.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gwxrmnavc.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gnwxdrveh.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gzvdruiuv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gbjaheajn.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gwdhkvkwg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gypepljiy.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gwfagwcnr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gvaoaczrp.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gomfubohz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfworyhfx.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/guydxruub.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gfpivfceo.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gzkslacyw.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/grkmrhghr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/glqnhxnsv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gdjbnxrzj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gyimaujpi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gzxgvvkpo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gskamzgbv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gvzuqrydm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gkwfyozbi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gusrgogtu.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gvyfftxpr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gdghjqfix.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gaupvuhxc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gogiaodqv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcbfpvue.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gdapsbnnn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gwvzvzlcb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gjmhnwoaz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gvdgtigbf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gsmltkjgf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/goiwslabw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/glgnccths.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/glofwgbii.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gfarmwzjn.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gfrlnwdyz.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/grfjzsmmh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/ghrdquxwr.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/golxqbdfs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gdtlpeoam.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gfsowknjv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/getdzczze.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/godhrszjg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ghzwpwjbl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/grngxffnw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/goajomehw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gjqxwlewg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/giwdfkuut.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghkxeqkwg.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/glgsuwynq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggfpwsnwe.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gyqnvwwfb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gzruridmh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/grpsmmpsu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gvncavhjx.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gbbcuyzos.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gzsdxtbrm.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gyptvxxcy.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gibhxhiuw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gicgnqxdv.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gwqlaqrfn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gvsdaxpmp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gthqiksaf.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gkhpimcrj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gkenxocno.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gokrqwaxl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gjgafolnw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gzgztwjmf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gqjoxouvu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gsiwfhqzf.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gbejgqwvz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gwtpjgvcg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gzrpycxkk.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gwglpartw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gdmpchxuf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gnamcbnao.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/ghwlajhzn.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/glnbcovtp.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/ggmghbiqt.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gvzeqanac.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gywgavpzc.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gumegweui.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gdainktol.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gbackhjbj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/ggqllopuc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gzppieouk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gjcgtakkq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gfdrqgpua.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gwwwaezxp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gsdmqunnn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gpgzuuiwh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gipziqpmm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gqozzgyzb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjyromqk.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/glrferpjk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gnklzcbwn.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/grjhzewlf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gxdsqvhji.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gtjztqaqs.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gdyseuuxh.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gcrwrtymk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gejmwcvor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gzjenhuri.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gdqvlsukz.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gkuajekox.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsgimsbzm.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gihddiocm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsruvpibm.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/glyufvofi.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gmthvfoqn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gzbnydovh.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gtdnnloep.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/griaahgye.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gihvjrxcs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gvtlnyzkb.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gppkwjkhz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gnwotghxy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gobbuwjan.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gdztyfgtn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gyqhyiamh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gbfljayds.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/grdednjvc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/giyotnyyn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gttowahkq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gjvpocshc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gtxwkuhjk.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gebbajwei.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gvkluqhhw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gcqtzslsg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/galueikjf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwxzfsehf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gmvmixetk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gfxlzdsoy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gshcqcnje.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gtscupsub.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/ghagocubg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/glyxotknk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjgrdstsh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gioukrwsi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gwxwxfnrs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/goetsxwqz.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gigwmjdqk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gzbqhqwjq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/ghakmvyyw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gbldgwspp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/grwqfdbqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gtycngqdd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/ghwurtcft.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gjebvzujw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gvnpsstxx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gnmbzyrjw.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gniymjocg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gczoafddv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gkqfpctbf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gdrfxpvyw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnlmpepwq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gralnqutu.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gethwfnlv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/ghuuqyubz.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gsuhscvlc.sHtML


<!-- 参考信息 -->