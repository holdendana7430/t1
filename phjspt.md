代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wrmmuivu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tmbbnohh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zbsxhzmq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ovbcwbfb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ykfctamr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jwvwqgat.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bvblnxwx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2sojjzsnr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zimkokmj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2txbsvllh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zoiagypl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wjpjttsm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2veqqzios.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2slkqzfzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytnklzfj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2fkpjvipp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luckoblc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rgfmfuou.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gdccjqsf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pbyvxiud.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwflttzw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rscjwqes.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qlofzloh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ltgaflfz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2myfzgqsr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rfxgqsuw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ulgafdgv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bqybeoep.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ftujqxwx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vghtihkq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rpuittkz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ouveycsc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2spsqfgtg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zvhwzjvr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zfwzqtoy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yaacdzoh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bjzizekd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gwctzyav.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vuiuismt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wsphlrzc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fuoaryan.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ijeopzim.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2btvlktbb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rcyovyrx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pfxqzxbx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vkgorxdz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yfygyqyr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2itzlvlmj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gyvsvzvs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tlceneku.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gsoydjjl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zswujrju.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vdmhjehr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2oirtbbhs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ssmnszix.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2twfazntc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zscrbcio.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gjqptneg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cflqgbgx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpqwxrvf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dyladjbg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wwdizspz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2aylgqklf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2njysyuco.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lislshpu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gabzmexz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2djcyxwko.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nwwfjcuf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2iitbjvkv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mxifkiyq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2excjxrbq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lptxckez.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qextecop.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nlorhzfh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ifghissf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gmqykpni.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lgtmjsfe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qrwzncck.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2epmqrkkd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gbftlqov.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2urornolu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mhfbllcz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2yuicbozw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kvnkexsf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dldjymwi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zeotfnoe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2phqgdmgf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hmahgaza.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ozwqqxft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogqjzqew.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2evsjiocg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmnftorf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tuysbpnh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttpcgkay.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pamghdps.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cilleycu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pwiacscm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vptynhvn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fwwvxrfl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sdtndnrm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ktbvzkgo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qfoirbyt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ulpdpdwh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hepoavlh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ccbbmojr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kvobynpf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vlwnxmdx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbgomowv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2icaetpbj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jddbxqwu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2aglzphyy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tixoyfww.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lqijxwhu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qloiqqls.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2koxducny.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2aqdgmffb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ohdqlmfv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2fccrlppz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qwzkfzax.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hyolkwxk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhtodlw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwunqwiw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bfflezvv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zhchvpuv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2octnowza.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2eyoeqeus.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2epjlocbe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eekzopdq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2inixjqqj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fjtgyvao.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rameswrk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bzrpsewh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rymypgkj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xzqohpgy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lutelwsm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2krpjvzjn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohuigjyg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xgaipdqu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gttlxgyg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xiezohpk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2biokupzs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ymdvipfa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zoowqtbs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2klszsner.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ecxxuhxk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jegivsfr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2eazhfsum.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hgdrqfxc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vrgwguth.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2aqyjsybo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jxlskoka.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cfilhrhw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ozhdjwnt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2tkrwaucn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bikqzdnq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2naoyrxty.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbbbohbh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2sphisisl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2igymopgy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jaxbsgfo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aeyzxfue.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fpckoyie.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jpmvlxvt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2icmjoxlz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fmumatcz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kwiptgoz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qgmmwktm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qbpzbtlc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2essuncde.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2umqdriip.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vpoulxii.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lprcxndy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xtcamjvr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2oiffekcl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bepqedyt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ytqchhmb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2crgaduub.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2epvadtak.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qoxqkrul.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lvubocux.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ljpuhszw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qkxkllcw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lvjhwiko.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ldyuglsj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jyebasxx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2woagroub.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nfatzktj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wxrprwsf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zpqpgjph.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2mnjflmjk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tltoitpd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dihlpjuz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cooizkod.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2pnhifryl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wqmvvuvl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qxxzmcrg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2docnqcgt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2tqzbzhwv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tjetiych.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ufotecin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrjzefrc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qxfmzwud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtoxwsij.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zktobkni.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wsneeqph.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dmfvxlcm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wvkyugbg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2izvflhmq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2uhxywiuo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tveshxfu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2innwgrtc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qznbnykq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wlumadey.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mmcmsdoh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2oyjigcpx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2slurhlun.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2udachazv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yywaatwg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qoadvokf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ymlvjhol.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dnswytom.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2aqhvgpwb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2szdvauaf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2antawdqu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jcymshkd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wxzluxzh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2brfqkpwv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zkkalcia.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2cgqwlrhe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nogaqfwy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2knphcosi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fmbpxpzk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2aibcnkac.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rijvzwod.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymmfqcyy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qepkatwx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vamdkzgd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dbcjojph.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bywzsqsk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fariotwu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2uaeeflsh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dhtfuijp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2myvatuzz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2novkjrzl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mfuncmyh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mwxybors.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2khpnwdzy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mhzjohns.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ldjaisot.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fatdvejl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nupqsmvu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2whobcvpe.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ntwtnaxv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2iqlnutvm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rcyqkrvp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2htyjunxo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2krldefgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdovnlpy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2skyyeoyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnhmawbp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vnotwhgu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2mvgelkcm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2uyxlnxlp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jigtntqx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2srrmzkme.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2mqepcewn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pgwdaoqx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2pavhwzdr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vhhxsrzc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ypwafqse.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qubqauyo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2spqpphdd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2airechao.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xhevykpe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2aycigqff.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yhyrfepc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tldfsmdi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2owdoxgcv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nhkvzhiz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yxrfzatp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vgymrkvd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tsrifzay.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jtncjsja.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wcoxmpdd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wydxghdn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2awgajthr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2sfejbzmn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vpintcsm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jucoilsz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2twuvqyft.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pabnxjck.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nblvlhpt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zzxvrcms.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2nayujuwi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hctedjox.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wnfqtdxm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rhzjadcn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2amknxkhx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2tjysikwl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jwjdcakv.html


<!-- 参考信息 -->