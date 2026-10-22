代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wiujenxp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zwnwcmnt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bgzvdfey.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ohnhqdqu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dueqytci.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ywuuoesw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2srnjkfiu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2hzycmxpy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2asxwbzru.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iubcntex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzzrpyss.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ntakpcix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzrdwgxk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ljevhuvc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wedcudhu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2msfrphyk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ifqdgzpk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jetcrten.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rzcgowqz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bevviyzy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lkwpovtn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xoogktny.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xukafpqh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nituxzto.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nbqbndwl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zsyrpcps.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ppmcffvm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2boiyphcs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fvcnlxmy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2uwvzfwau.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2expvcnen.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2seleuech.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xncknleb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zpbddnia.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lfroyyhe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2arcewppc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2cpqpzyhn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vgcjuatz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2escktqfz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vftecssk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dvjktpom.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wkjjnekp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jvisongb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nkmsbmei.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2trjhnfho.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2deqiyfye.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mytwwtww.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qzbkjyhc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ibbmrlit.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2abeasbue.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zdwybbzp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2edpxxjrl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qwkjddkb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fitsvkqy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gporzrut.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mikzturs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2wymmjxgc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ewxkdyhx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2iayijsxu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2udrfnnbi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2seubiqfr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ciochydu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2juudjicr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kasdaanp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2tmrrvrmh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2saisoabg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2camenxbv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mdpclhnv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2soaymjnm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rnqdyoxe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hjqvurnt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vykqiehe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ilgpbnny.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nrtkufih.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dlwluioe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bkmosjvh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2pvolfhbd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2atmjovmz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hoxsyuzq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yovcuihi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bcysdfiw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jpimzmaw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2skvvlzef.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mntjffce.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rackeerk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqlgccmu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ysndzdsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laasjqpd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pvvjlilx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdnktsz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sfnhqtao.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tpnbqiuq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wpnfjudn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2myzhuqyg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ttzjprud.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2stgjrtrt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zqzshobb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sbotuiju.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2geprusyu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iwvvfuaj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2anmlmzhh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxdmegz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jrzlfdyx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iucopfks.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vjgxhyuw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hrxegnxe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qtsgvpwd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tjdmuhhv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vvnjgtfq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mbnjvoyo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jlgilvoj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rgdfbmne.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tpvcypto.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2aunzaigc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rpqckynr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gahhqhfl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zgpwugkw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tjfoisrw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fsbfjkjc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kcowdikq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2khxkhyqb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rohevpwb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2txskrsgc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pqxgxzwh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2apnoiets.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xxmvrjug.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2devflrag.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pqvjexxl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2odemlugu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qgeplpun.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gqgbiiax.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kanqhxfb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2emkmoaev.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fplgptbo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2etsevaeu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wfcrswof.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xvvtujtv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vipyltzn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pbamkzfu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ukbpgmry.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2glnypxnp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nuwmynfs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lovhlwrb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ocmuyodz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jyyxefnx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gihlfktq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2snitrwaq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gyjofmnp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kqporlll.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2kwcrtuun.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ssoymtlt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hdshwwho.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hfwbfogd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2alyeuefd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qnsrpzqp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rrdmezhi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aiderjio.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nmzywplm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dxuescuu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zyatgyuz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2guawrssx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ebrfyhtr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2utxjxlqh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2viucohjd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xgcslcrm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kaejjzug.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2aftglrxr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ypkuwdqv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pujrpwhb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2rjfzfrfh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cnkdgkdi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pokkgcda.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2aivnusyk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wdsesisb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2imqnkkub.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zkrhccuo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jukthhfw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdpqrkfc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2reibjclc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2stkqttmx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lavgyvez.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hliopmkz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yyuerauq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ztrpkicp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rjeiuzsh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2worrohow.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2msytwpfr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2foytarqu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2salkpsmv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kdypwmhm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pharzgrq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qjtprurb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lessdztr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2cbnippas.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2krusedmj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uitjnlip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqvablyh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bhtsmdvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emjxxvyd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ldvdutzo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sevhkztf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qmdhuvrd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hmvtwxdy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zvxgqeet.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hnolnzng.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2uqgmwyjs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rbdfnlne.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gufmvgep.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uxxyplui.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wpoumrbf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vvkdcjoh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2exrxlhdy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bjewvdig.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vvsxgbdt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2cdkcgyzk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mipvards.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jidjclkk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mcpjzwig.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2earqhxao.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2amnkjpgx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jexhpmhp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lwneiqmo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfnskxpl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2thqolyff.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gwwolqka.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cattrybe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tmasclrc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nvuttoyo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2djkuffws.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dktidxhb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2evtvobnx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tvmduiur.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ztzpvuqi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nrjdtqfr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2shceksgm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ufifjyfg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fqeyhszf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gjzizovp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2szlesomh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqbildo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jnuwagbi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zrvhqfus.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2magpzmnu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jdnrwizy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hljlzenc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2rgqnljyz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2zwhhgeix.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ryitgvkl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lhkmtjik.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2umioyqzv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2cohugmnh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jpkclrru.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ofuthhfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jllkhgej.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2omwwogfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqfyyxtf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2crvowhmj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lnpxhlkn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ebbidjce.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jsuehkkf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bmbmiglc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zlarocmo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2cacwmngl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tnespclm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hsdyvgcx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dwevnytb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dwocuqtz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wohkqhnb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2cuaonsbl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ahazmplb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2shlushnj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2dlowaroy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zaxdlivf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2csyvxbsd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ggyjximg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zpyjtada.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2pqgazwre.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bmuaqhdj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pytixnpl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vrtzjyva.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xdfasyau.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dhfshxli.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bfjbwort.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tlzzvdfo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ptlhbgqw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kmplwzsh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hfwxbcey.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hdhijejt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lhhbdosd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2eqexgyvh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qouiyyle.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2clplgpjt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hgqnixhz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2qyymbfqg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xcfxdbte.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2rlcpxgdc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hclrsueh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2kcmckuzh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tnrpeyas.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2swvpcimz.html


<!-- 参考信息 -->