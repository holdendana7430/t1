代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nbgthhbu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wafxrrpk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kfttsirl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wuubvpmr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kwlyssfv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yurrjdlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kircleoy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ednzmutj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmliqmfx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ncrggzyc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3unrvinil.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wjnlljue.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxyxbhjf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pztvjxwk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3exkjhqcr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wtnckfzu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pmdrunus.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vnrxoqjb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vfhqvytt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3msqqdbcv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3urntywbo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jhgldsim.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fdvpgilx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hmdgtsgq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3swwblxrl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gxfoqzeo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3czyhomtj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xkuaybma.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rscgznyv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3azyxqqnr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rqtamagc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ggvqedso.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3smqakouk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fjcedotd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3torliinl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xcdukuaf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zholfpvw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lebeimhd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3btsubwjb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qrvmknbu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3owvsotrh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3thbtjibn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tzkwvoin.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3sqcbrhuh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ccmokzkg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ncrnpqks.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohdtpfhq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zxiwnkvp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3htpazarw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vualrhsz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sbjjblce.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qczvtapf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsljudzw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fbluahcj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jwelycgv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mtsdqqox.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bfpssglc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vvempicp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3krflsrxe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mjthjsoo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3mhijmbmw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3pialkted.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dfxbvpjj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dbcwpwzb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jlennxxu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3nlwrppzw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nzjnpbkd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wtaddrck.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3blhwdyyo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vgzsbhbb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lugxzqnb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rcrhhukw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3iprxvljz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yksitojj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fsalwods.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mcfxbfff.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mgdkxakf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3znycdeih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3efdgidik.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3mrcmfhlc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3npkdfrfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdabaoqi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mrcgbgmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqqjhxvq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pkdfyzqc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovxaukqy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hokwydne.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kqglgnkt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3olvsuyqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdbtodug.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3prktmlrh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3oqjfhiuz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cgnqcuma.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3htngmiqk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fkjjerik.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qfkhhupf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yimxusxx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hdsrvckr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vzoptqyb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gpipuwhz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zwlcyidw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3miicxnkx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3juhqxmje.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zylkowtp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3owbyqikg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3btyudpoj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cfapnpfz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hgqhmcya.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dcpwqatg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3txyepsdt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jsikczwk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3drzkryrq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3naebufpb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cfbstvwf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uwicbbtm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gqdiveas.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipdhwpxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3klhdtwjq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eozoybfi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hbviigzm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xpdqbiiw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qgnavfpe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vnvcoqsy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3itsljmcy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3drfkkppf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vaqxproh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xwbgviwm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3sqftmbun.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3siczwbni.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3otcwgonp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fzywllpc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jonouqik.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pusagbea.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mjyqpgcl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ylzbwftf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fdzfbgbs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nprlynkh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3oizzxlwy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3aanateml.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wsnjvvzu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yybwhhxv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ssaehgza.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fmkdbpug.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zbpgqrnm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3excrlasp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pfendrpj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wcxnurax.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3mrttnbyw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qsekcbri.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bdtrhpjt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eipdjhtz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rbtphips.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qyfoofxe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vuksucqe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3liwrejnl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gofgifor.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fiefnexi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hbygqkog.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jexbimfi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xgewvouw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jfshjqew.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ytbrwlxs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3thrlxrxk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pwsknclx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gaoskica.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fsspiuuh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3uuqtwjhy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsjehaty.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3suvquvyx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3uvsagpbm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjaisvbi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ommypksp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tdcixazn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtaxuptj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dxnshbus.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3yqjwzojr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gtlurtvq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3skcsqhab.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bgezwkde.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eeulxuvk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pbvotllm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cndddjsh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gupltluu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jlkfamap.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3krzogemm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pjahprrj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3geufwjwp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dyvwgiaq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vrsewxnk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3asfbxbuz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nqubyzcl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cfzdrixy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cakygsxb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3iuenojah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znunoxnp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dymvociu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zdkbvnan.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ucenaquo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ybjrvjgn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rasbttxr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wklwkmpa.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wflvfdeg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dprjwjgb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3yffmftne.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ohcgizbd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3czvvnqhu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3lkpfydud.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sdtqakuf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wfyurzsl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hzcwkhkr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vqczorow.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3yfgeqbwu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xjqadtxv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jwqkdkhc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qpqcbbft.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ewuzufsx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pcjdxsdi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3meiaquja.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3isypnrvo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3dtdvgdkd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ihsasnzf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yujfqrex.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3viotmwnp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vfayixmh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kqenxkjh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rqzadkwx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yzucuzlw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lqtknsjf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wprrfjha.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ekltajfo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3oxjldqmw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fkdvmain.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zzpojdmu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fphrmxxb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3eeoxqkhs.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rqnwojxc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jdyzqqic.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3aaoalhxt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sbblgrjn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vbsyoqld.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jccarfgq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3emhrkamh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xonsloll.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qvvkjofn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vylkphju.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tyuiwbcn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xkeiptbz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wbcgnfoz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cbmmgbvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3taexmbec.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lwyhdtuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdaidluj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lztimfar.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gacrluoa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cccorznt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zvkpdfsw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3obyqvkyg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nnoqljef.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3waoviasa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pkpafozj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3otagkctz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zoazciyi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vvkutmvy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mprfeanc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qwgskqra.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pgpngavh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jcatusaq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3cemuoayh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvvjbced.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ulvughlr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nntwxbxn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ghqtofhk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3cchfwfhd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qmcrhfgs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ffpgehrz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fkdwtomp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ncqelydd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3undbfwox.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rrtvilwe.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qbmkvpaf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3eiacrfzp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tvvgkwhf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ohfaeltz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xngynurk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ahqlpawi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3cnginfxq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dsnvucgs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dzdoaxmr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zzotlggp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3uzhsxxuj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3colyfntf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xxrhecbw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qzutnvin.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3anyzudsc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dollveal.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cyusjoqc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3usxaapwb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ebgwttdv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nuaoqyey.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jiajhmup.html


<!-- 参考信息 -->