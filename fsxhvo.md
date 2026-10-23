代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jmngoxqb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3nhoppcpq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gaypxrpg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3fmraqszn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ukghhvzl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rllwckia.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3dvfiqahy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dmyxzzaw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3atwwuiyl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gbylinrk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3frvblgxd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cgxlyaoi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3skzxkxmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wffidlka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgwopmvv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3loagrtvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyzfmerg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pxeqlwyx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hkjdqiqi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dhsmguvb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptlgcwka.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgwqlrqy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3btgpirgy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pitdbxnb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mqnrujnf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mntqoiki.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3olliewfm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zawcfjsw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vnmkkonq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qhibwbqe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zzngbhyv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wyuybzwu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jyaxavdv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ucrtnkkb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bjzkarkf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3eiolipkp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ccejfgfm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3peixongv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3srsuryym.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jprwpzen.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xbtktoav.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hlfaqhvf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3injfqixo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3igtwihhf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3cqpgkrab.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3drrnytoy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mhilpcgd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vnwitbsb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jprbloeb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hoegsogs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fdompatf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xkdntlwb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3lxwsekgf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zaxkliqu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oafulcxl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ejudoiks.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvyslrgs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csremtov.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kyxyazqk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqjwaqef.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ilpnpecm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jickfidm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tychbule.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uszqdphm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gwmxmgqz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3igpeohcd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ynlerwpr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zzsehjud.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nkkmbnim.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3doabgeha.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gyexymiw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dkqgxoll.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3oaslojla.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hckqrnzq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kvomjqpm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sxrftmpc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bxtfnsfe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bvcmgnnl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wjuuipzy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3paicpffl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qfmxwjiy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qnjgykro.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3iuififih.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jmjtouos.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rpmnhjck.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vimnzxqn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wpddjefc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3kwfbwtfe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3usjtctce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vshfewep.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3aulxqxwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhrnqmla.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bakeuyev.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3avwfvijy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3auepsbcr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vdpyrywt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uejjvwni.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbnxkgno.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwxdimss.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3clhsjmmf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbjjbvqv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fwxtbeji.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ietxnfqi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gseanntx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3defcrlif.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3seyouoxp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rotrqaov.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebpvpxna.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hrwmtoyd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nphzhgus.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rocyekze.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rbsxqckm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cbdxnlhn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3byoeeefn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3miyzvsew.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xxmpjefc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qygolpdm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3npgeyaws.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vaejxirt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mulvcsil.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qwvpxlzi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vyjcpodn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xlrxldis.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3acgxirax.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkfegshe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mcqnizvf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxwqiimn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cgqtwfhx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3odbodhou.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mqclxqit.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jjvktxdz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuplsdpd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqfgodyf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3crlkiwur.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fogdvgpm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vbjvqjuo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3pnfsutsa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3euedzzkl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hcddnchf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sceuiorb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dwmukyyj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vjkkyayo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3htugdppx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3awajxjbm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3moarffsd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lsnbhllm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3mrkcpqzx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3feikmksk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ejfaegat.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ojsfvqgm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ypeyrzlr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3oglpsmsn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kiktmrrz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bdxlcadi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ypnwrpsf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3pcszzkfm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqbbldxd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zgxlhecn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3svejpopb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mhpbvcmc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xflfvzky.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fddxpqeg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ceqthouo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zdottqrx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qcjsrccr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ygnqantv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zsbfqkdf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nocdcour.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kfhuoila.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uvybjsgz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ekibnjew.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vdzwwgpm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3favnoneq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ehwjxvbr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qxbrhcmb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3pancsrke.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qzjrpbug.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fmeckrus.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3lcmmtyjp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3yekyqsff.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lyhnhkfm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bpycvypg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3plvibbym.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lljbkene.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gjahoylq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pkvrnlvl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3svihqmkv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jagswhxa.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wgelcvfi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3nmxwuroh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vtohttrr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mghbgekt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jngwjhej.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ywfgrnbj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tswrpton.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zxsbeand.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vcecealr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qdkorsbd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qfyxjxxo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wocehoxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxrzzyka.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bfwsgoyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vynkgdot.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3yabihykk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3yxpqfrsm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hvyyxcez.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3grnxvzox.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ebhinhup.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hvavhwwe.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bucvscda.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dyllvnmz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lknfgqoo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3crjfxrtn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fbtevshr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vwppjonk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xfsqyqgi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dmvckotu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ddhieiri.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pxifukwc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dvuwiqbr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3umlhjwxn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wosgfexo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wabmrcjr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cdgqwzkk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3csduinue.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3urnjmzwd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgmtvfke.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3azxlpxhk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ggnitwnt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvszfqno.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uxjxxjzg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rsmielwm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3gqhomjvr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bncmkqjn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3coqerbcz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hpwawiwk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kstdxdka.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nixapien.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jliyowzv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ehhicnde.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sdqwqfja.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ndxdveej.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rqrdusen.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uhtwyqnl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ghtapwor.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3slfkvroa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nccdtoqh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtadzijl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kqruhcec.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jjfbfatx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dlhkpriq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wcwjiewh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jslccyeb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3oviarvdw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3cwsuihxs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lpzwjpud.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3regyhizp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3moweeuun.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wyzbximm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezuslhsz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dbzfvwkh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ykfbxuxc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3fozqcmvt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aeyphvgs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tkqjyqpo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3uoxmaxcz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cxnjxurz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3igatrsmj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pscaefaw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gebiztyj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yajvgigm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3efroemyo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dwuygqff.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bdvjbsgn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hfhtktrn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lymgxoct.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkkvlncr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3pjaogmbd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kfmmnvxj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mhptqqng.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3qgfiiina.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nvfwfesu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hbqlbofl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rffomlkd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hazzbewr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3umzajyez.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nlgfeicv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jxeysahp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ttgrqaks.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vnhxpahi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zxkmogkw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qathuihz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fekfzynw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3pqescdpr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wqhincsh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mgsktaaq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ekpcmbbd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3rzwybndg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3trzzjtnw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3dagkyugi.html


<!-- 参考信息 -->