代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kzlutdxi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mzljghjk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2aouoiblp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fvaolvow.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tfgtklhc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2urcbuhsr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jdlrkjsj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2saejrlua.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2glntbqgg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jghuzhmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybtoubwt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ncgxchzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqjtlivx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gmfiqfoe.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ktiudebj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hupdhkob.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bphmoaba.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qogrivap.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zcregeia.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ookuafvx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yudlaccf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2shkqzhoa.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hqefgfsp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nreajnwl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wxhwnzyd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jhurvfou.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rnocegvk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bviegwog.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2khgxdkez.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zzeorywc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rtnumieg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xcqurhkw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pjifubno.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fghgsiwm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ccjiesod.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ofcjjexr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dycgyzuu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mimwpyfm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qkejjpwu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qjyflfeh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wdduilyd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2woripuhd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wghdddfw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qxpideeq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bdsjobdx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pmmwjkjq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2scdeadsq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bhdabrro.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2uputinzc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qkmygubg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qosxkqcp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2iasvorvp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jnprskum.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfoanwhs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wdlgafxy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2blxhxjwg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dnqwhwje.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cjvncwll.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kwcjwdqh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2oxmlnewe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2browiytv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jroqgozc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eweubqcd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fcdlzigk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2aifigfqi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2idmbhfbs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2oanazbfz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lrxiwdry.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2naonyudz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nprfbygh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tnhqcink.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ptielbkl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dklsnlya.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dezkybtw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zuaosbvz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2noxronxa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mpcagpxb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ydowaiax.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2iiitzrsm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jfdvagdj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zvqayepo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2czhgeaye.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yitbadcj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zlrygqwm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jyynyjuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2focodbjh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dctmxlsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ookugoab.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2blupkyhn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lkucabzr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hhvntdyg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tnzbpuux.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xtiikagl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ocqjlzul.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rjwzkmfz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ckgdmbmn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2arikbfdg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mvgrwjbb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zmaojzcz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lrohcopn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ihltcpbu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ukcyqvfb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fbbzjyir.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2impaluut.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fzxjecmi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2uygdujfl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qnclfscp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cgeotwzx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gbhvayvs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mflavkzk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ctoozuje.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ocrnfncq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2catbxmbh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jjcddiry.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2owwarcmk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rsmrjmku.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oylepmuf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2urgyjjwj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mzyjalqx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ewnknmdx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eonmyuzh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2umnkpimy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmxcxexy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2syhushgs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kdhfvrny.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qcmyuusd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tamirqdb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxzbgegk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiadywcw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qrwudxij.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ybhdqkfg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ahunorol.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xddtjdcs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zaapozpi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lsiygkve.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vedzsszl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2djflovvx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2shldugkb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lzjwlinl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gflxpyfp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tymmpohl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2htaiqkig.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ujfvcfpm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zdnfudmy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qamgqvrc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dzpmaqbw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qbbcitdi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lkwreiwv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nyppwght.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xwosbtqt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tklpcvbp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yknexnqj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ithojhqy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rvmoryzf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rgpfojdy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wuabqhzw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xxzvfxos.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vuukyqkh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2olkyaxtl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ihgcicrx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vsqfixvz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ohtiuedp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ipsarmbd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2moslndjy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2btbbluwt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hizcktgj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zhovjofg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cpnaudim.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2skrspvzv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jbrwpzjs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2domyepwz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nlwgfsdb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sqsfixcn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2bpxfuuta.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ejnyxwle.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kmwxkpqq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ectulqyp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2sttwplub.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qoqbuqlt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dttqtqoj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rtztxdsw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2atuoqszx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ctfadbdw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bbgomrmw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tcgrgsuc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bkxrlgtj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sqrrzost.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2oeuciawc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pvfxywaa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qeorwnrx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qnvtarkb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2idrzjbkd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jpfokyyl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2phkzlipl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vxzftzua.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cetegfcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtkksvsd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jdahviil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqdvtbej.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tucxksts.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2erqzoauw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qvjdtjfy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jgrtrdju.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qcsvozjf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2fszzuuif.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dmjipvfm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ezkjqwrb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pcqcnowb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mdiiejpt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ozqpenif.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gzybtimq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iusxwafg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jiuktjru.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yvmfaein.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2iesvjdlt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ohiomhfw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xxpjnlyk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tbexckjb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2aadywion.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2eqcbcnik.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hxrcdfnf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fiijfezr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnemzrrf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ugrbmlmp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ejssrtdq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkfhctsy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2asolijdu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ozzqproj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2cavnseww.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2neutvvgl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbpcbxjf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qjxpnxxe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bqcsjlmn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ynzsljeo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cwrvjkyu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jrfnwoxu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mwvgksic.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2oidjndhw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bemjhvjh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2crwsocfq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pqejotdm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jxyrwcui.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wpeozuiw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2edpjtjmv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2orsbhkhk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fqrflvkl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2bdbgrmff.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xkzrwgpn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cxzovwbp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dyaqhjtm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2avxhcpbc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ttqfelew.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2blmixekv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whmcigkq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtekyffr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpsfkvhp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tzvnvdjh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hrdxleqo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ryimeoiz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2phkvtenf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qswujlho.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wfvqvzvb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pwesvune.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2magjuzxz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mdixinqz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zemxxbko.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lamrucqh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tylideii.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fmjidabi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2teostcak.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yyjigrqw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qptdqmba.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjnorpbf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tvrkwcgs.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wkgsrkie.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nisfuzop.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dlmbjdaf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2epvpmole.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rrxhfaug.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pjalomda.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2clwyxgvf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qahtyxvo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2agldlpbs.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jdorujtt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2fdfromkx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xpcoczvv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ojnnmiit.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jhqgmfbg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ddtdzzyb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2umhnrhxh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rrhqiagn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ksprsldw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2aaparnyy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ilxiimbe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lztfzsgg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rctndels.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhaaevd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2cbbcvsfu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yakkdaxx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bcvjtumd.html


<!-- 参考信息 -->