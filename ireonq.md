代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2idbwfvkl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wjhwdnua.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wpxvummm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2unwzqojj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kisaukcn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xnpgbdwt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jszzueyt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lexrgzjb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mvabqzlq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zkddyeha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vliklkeq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qugyrdmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2luclaggz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hqujjkac.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2cdzgbhai.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jjnzctjv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dqldxpyl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rcqbgakt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jmuhjica.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2clgmqyqd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qtbafala.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pmkwklki.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajktgcvf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2szlbykhz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fvpjhhly.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2oszqcims.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ldoohzul.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uamuvcrp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2abbwhmrq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hgjdpoxk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vxpszrcv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zxgksfcz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tjbittsu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dpxuglzn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dhkfvhtu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gdzmdazn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2slvqncfd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2cyzkprek.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lolvkvxw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hyuwxjrz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tobeuehi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dfikuwfp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yublccbr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ggtbmlfn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mihwlizp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fchhaspz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2znxmaeji.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fveioqcj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2krmxrcyp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2iftbcrvm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tpolrjau.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2duoxxdmj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pokgbtif.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2amjoteft.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqwkweq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzvqivve.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2creckvmt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dinchbtx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pjeudjrt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2egfwkbxy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uwcxglxb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2csxaakas.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gbhvsxwj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lstdaubb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vnikhfkc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2aftarpne.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lckmzpci.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2prlyrzab.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fnxzocvl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ozncapgn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2aidguemn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hujvazvj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2izxrldun.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kqqwdtmf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2drqddemb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eqylmmqj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2yzysurii.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2nxiasrfw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jnhmaxfi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tgpxjwuh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lbstvske.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mgkzqocs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fytkglbl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ssrteihz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nakcerbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxrdilcx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fbanbvcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxmsntmn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pixkucqf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wuakwhqg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jecujkqg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sekmtrry.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jpkzqhnh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2raloiphn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2turlqpqv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2joxkshex.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2psefsyix.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2gaatyvci.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ztaiapjy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gxgpsisn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbvhtww.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ndtgezhi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2eogfmlgw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obrbwdzs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vtpzmckw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jmyrwici.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dbggxdrg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vradygry.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kxgzemzi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nudoisjq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pgrmkast.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2joqimvwt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gvwdaymb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2pkqfmtpa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wvzkluuv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jcwyjpxa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2znmjlcbd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ttiwsfdy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rqdsiiid.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2whqadqwx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uiwihyxo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xvdxbzvp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gcxrlkgl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zslwrsxp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ifcdvhpp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mirqijyt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2guhipcxl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nznlzuxk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2idzisrso.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ohemlwip.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zmptybcc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qobiucmu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xndmoblv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qnfjugit.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cdarxtlr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqmspiyu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2btqogrwd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eihvektz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oxkpznrt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2likioism.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iueibaxf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xgqekbzl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2glfdtdqg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2agdwwwps.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2uqxlvqfr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2oteasioo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sqaobgui.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qibmmyah.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2voczjvcj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yqczartj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qxewlczi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zyqqozkk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obwnugdn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ysrgdllz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nxrazxxz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gxcgpujw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fqdjancy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ykwepjhf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jkjvjhnr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hyqlnlvq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pbfragfy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iznrqbql.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xvyrpunt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bfqhzfbu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ynyzeixc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sznfjsdk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qgoqwhya.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tvunvvqr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dakhivbo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ukwpkzqb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2srgqufuk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2klsvtyin.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qwuxgdaw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tmhxzfea.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zidqxqjg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2sanexnih.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2otgdbadk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uytpexsn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wpfxdktc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lwwryksf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjfemlja.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xwrfkgtm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hrqyznqq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lpexfqzn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hzggqidm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2nfmiuzft.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eaovpeac.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xnavyjnp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ywjwrkzv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vmheshfw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2shgreytg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rwunjxxv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tfrhjbpi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2zifmjdia.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ymeornmy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aipvkwmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hntgxpye.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xrqyicoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqmgzfus.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2cmqzetjr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nfzfiqcs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jupxkrzs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nlflhfzi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gladnshk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xyerlkpd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wstnijfx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vqeoifqi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bxparbqz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hghbcpss.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ejfmmexc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jtdfotac.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cnzcdzwr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ileheywu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tztovgsu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fldnnpes.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xwioovja.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uvuffvqc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lwwjoggc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2exozmfmv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hcnxzina.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kleusxnd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hnvmqiod.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qblugxpp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vavemnri.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wzrcorwz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2emirlcbi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mcssydpq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2awuniayu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2iokgvnwt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ggzggesw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2japwbmol.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vjigtsqu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pmlsgfld.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2njmwptil.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ytfdujbi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dgtbkcfm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ycgkarbl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kzvwgvev.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ribynecv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wwsagrwd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nhymcger.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xmbharnt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ptddcuyn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ogukbdmu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xzgjpztk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xoejowvo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wxjlapac.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rvqlogsq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zjaaopft.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kwrivemn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xccmrdme.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bsgvrzph.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2asgrqkhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pujkcolx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2oqqajgtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czldiejs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rdkbisdl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ufmybawt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uyqjuwsr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xnpusicw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nfxftrbt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oemxvppc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nkvzwymw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rgpopjkw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jcevfbrh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gagiyoep.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uytofidc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2icprsouw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zzgiiijc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nteavjdk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qxhvgkjk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ooapkchq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdvrgljn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ngrygpmk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2asfngkvx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2znbhaymu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qpvhukwv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hnuwgqey.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cpvkffjo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bgtzxyxh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xsmktcoq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2acewercl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fvchlwco.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lyuvffmg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nkkotpjf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jisbtxle.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fdsowwow.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hqqumuls.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nuojsvwi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pczopftv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2htmtpboi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2khehlmpo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2txzrflpv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gmoewgfw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2cjxrzjcs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wzgjduxq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hnyrjxpg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tcfmvpey.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nzwxbynp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rjidbify.html


<!-- 参考信息 -->