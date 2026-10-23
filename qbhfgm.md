代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hkpauyen.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lzxuixwd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3wsfxaihb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gpawbvqz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3svtjgmng.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3odhcvgni.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zfickjpo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pnmczodf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rruzfstw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vqkjkkwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbgaogoz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mippxdlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghbwsecp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mplqmhgc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cluutzlj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3clxbrojt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wurbxmbo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3izlldjhu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gjuyjiyi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uwiyhjuk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3isamcibm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rshnaftr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3aulahfes.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xcvmxmcx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vvrrzque.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qhzynkdk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bjxazriy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uahdqnjj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dkjlxrie.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rmdkwiuh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3efppeizy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dqyrxalb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3tikngolm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yrucigcm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cnkxgbqw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3elaqqgbb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3khblkqcd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vwgisdcv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tbkwebsx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ripdfmum.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3pqeoqgpq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dkyvogsk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lcciqvka.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tbqfcijz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mynfacix.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qpoodkor.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vpokfjpd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cxbubznr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3odppfeme.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3swuhfdxw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bktnltyg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ximxbkut.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktqxvnjf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njmacasw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ddootweu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3idbwwnli.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3weaargjv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3auvqyomy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bduyeibh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mwvcjfeq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3zxkfhwrb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qcapniik.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hkdjfvgj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zzpppedp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3spmxouus.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3llxjudnn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3exxebhzm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fvawkgdb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qzwwyfem.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dztehzti.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3icrlbiyk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mggxuixn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sqgjahdq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ptuqlskb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dsqzlldf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kpwvuner.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ruaxwfeg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kbphqabm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3glagqlgt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ctmrrpvj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bbqizaak.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mdysocvz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3uaftrqza.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vlufrgon.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cylyioiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vimrfhnt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mfpaftzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bczdrsji.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fqpkrqep.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3htosnkdg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zwhzkwhi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bkdxkuca.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dceaiwlb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xwhrlero.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sqtfccvm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rvpadwpo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkwxjovb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wlbsvisq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fuprzqkc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gnlnirox.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rwmeenhx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3almkojep.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kwihpkol.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3klgrhase.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lkobnegh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nkayzbbp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jiipsglr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3reopfpaf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pamnnvaz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nhltewez.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ghhkvbvk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3scdvkxiy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hrdhizfc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3obbftbua.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ppokercr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ujybnpdz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hubcpnfw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fgxzegxu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gmdikvkt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qraecgki.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hbxxwpxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3shhofarc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukygsqeh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iutppial.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ppalhzgh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ohjtmgda.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptxfboju.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3abatlydb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhtzysno.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3smrkgjbh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kjvmymsg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wpibfvmm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlgfxwkh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zqqbahim.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qvmrirll.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kygaxtjg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jtxgtzyk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3twbulpzr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ghywwrvt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hlneorle.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wbcumnyd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ijudxnlt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3drsfmtgp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fppcgcbt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ibbkzsam.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hqkmtijn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ehddlwut.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cjtvnner.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vcngbbrp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qkovreit.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vaepyyng.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3smenijnx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xksnnydr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3chvxamir.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jurnezsn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nioxaihs.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3peelcnlf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pykezzpq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nwscimke.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3itrqdfro.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pmfwknxt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eajlgkiy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zxmxixop.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fldawdfi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bmafzfen.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pextobpm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3krnffida.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ctnkivau.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nhpoqief.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3shjpwuoq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zpexjkbj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmtfldfp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mlxlqttv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gpjmzfgw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3bgcqdeeu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hhshblzm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dsqdbfwd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyxctyoz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mvcbzskb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3paaegzss.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3tqkodzfb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zbymaouu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jfdqbqmd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mleyhvrp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gukzzudu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3pumrupce.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fpgvtqje.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3aenbuayo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vtyzyxmi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rnhfjpzm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3szcffion.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cxmvzzrq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hfkqpvyw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3pubuahna.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fawbzvan.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3aqtqnhzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oaxtlsxg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3yxhyodju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzhlbztg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kuvxtyps.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wmrjwjvq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3knnndpvz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wzlzjoqo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wvsobeix.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3acvrfxmi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dmclcrxj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3tsngwpey.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pyutlrmu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3glhpjsub.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yqdtdomu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kslrunku.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3upbnegve.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qupezsyr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eaxlhnew.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nwyzhgyr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cgkzfdxy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3poynmdtd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3smepqnpc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3zmggmhye.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xpvqjzta.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3odpoehsm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cekbijjg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rejelxeb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3alzzxyqp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yesralvf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbsgadut.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3afbxtomn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hiogidim.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3huismbeu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tpmxplto.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iiippyac.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3cslpjgba.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fnjaplto.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ocqvktlc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjneomaa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ljubpccy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3szmbhznh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mwbsujgk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3susenyke.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qcvwcnzu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bajhagyd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zhvayeev.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wdlohzgx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bdrkudyi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nssqjwba.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jhdpxkgb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vwfkkcbn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gekialyt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lqzmjvfm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kocbdxjh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bllqumxx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3klznsvet.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3okewlcle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgmmumlz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmamofvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfeiftro.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ifpccabb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3urssjcph.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bjrfpdei.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ebqnhieo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gvpdscmt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3eaybyisf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hjsbiugb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3otbvuvrl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bndnjjox.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hjxwwoyu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3trjslvud.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qjvhkcgo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3oojbcwif.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qszujwrb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wcgvweec.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3apguomtm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gknauzla.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3rytflved.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3whurmwxu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3sghihicn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xzyzvmav.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3swwhnbtz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cdmoenrr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3sggligbs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3itszotuz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lmyrevld.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3zcdveryn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3naxviyzn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3uujxkfeu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xylhncst.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dmdgyeef.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sayztppz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ksvvnwmo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gxhxoeof.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3udwpjheu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ehspbloq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3utpsxyic.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3znreodmd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ivirzlyh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wxfacgvl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ijnkmtlj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hnmtcmft.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gpxjcjug.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kcmeicpw.html


<!-- 参考信息 -->