代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2meeizrgq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2btzeuxje.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2klhogmom.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fumfpwec.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dgghgqby.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kmfukfgh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iqnfnien.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rbwxwzln.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gjseafqt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dpwcxamn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2esnnbihs.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ejonqthn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2houbpxrq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cybdjmiv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dquhdibp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vclcqizi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cuaoosja.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2xuvkyaxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxmqpsiv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ffordzss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cogsyogq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2etotrwov.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mufhtdcx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2gfqnxper.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gjaucfoy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlcjpqvt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jvpmxalq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aynjecmo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nayecltb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fdmckvsk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rrthmdcr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2empwnzyw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2euonoxhr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2oiynxrqb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2weoooahx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ihgxzshu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2asdsugki.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dfvdjdhi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ibwxuvmy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tnnrbjxj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uffvopyg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2quiabwze.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kyulhapz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vaskyyio.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rccfzorh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jlrwbkyk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bcjdczrk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2slbizjcz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2yyokwcvc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gukegjrd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zjjihfgl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ftmtrcyv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uclpgufl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zvpivcbq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dqawwnbd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zqjrdgri.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2deryjdgu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fsnqytyn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbewbtgb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ngziawbf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2asskpdji.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djstrgad.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wmualumc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtgzgpkr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zacbylwb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cpppwzij.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hiwzmrdf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hlwvljfj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yglbcglv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2maqouklw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iksndbkj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cxaocirw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fktzkemj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xiswpabq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2himhirov.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zrpmlpql.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cnzescbj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ygxrksuo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2llblbnpn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lgekxlps.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yvnsighq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bmzhzdix.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2akorzrzj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ulridhav.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ugycctwf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2oqnnselv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2prsduimz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kqkfmuxc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2odwrnegx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bhjhsrba.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jiqqjnps.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rkpkcmug.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xhajfctn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ridtaeqs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2czsjwetg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2paunaavr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2limbvhfp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jlrfteet.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2isnwuwrm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wajouyhl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2umojvfir.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hoqtyyiz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jrwdpgyw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2aalfrtwy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyqjswc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yilvquow.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ifjgrlko.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yicpyvxp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cuckrodn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2acmqubcq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2riznripx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kecoyoqg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2okziqbdf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nkdrfnle.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jgjtsijs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lqjnhctc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gbcvqgrl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hchpapjb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ngatmjwl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2utovwdsy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mtrrdcvo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gwaeehvw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2sqwpvsoj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2glxzgcuh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hdumzqyt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vayhxxzl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uyluyuek.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wbeaffjy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2unhaqhdc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zihrrxyl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fdhnrnes.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gfevxmmk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dpyujjkg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mkctbesq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcvhgibu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nxrjdsep.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqervzff.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2egbpamon.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hofvggrv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2sjqffuvj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2frrctdwj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pfcqtfws.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wlnlebcm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bbsleydl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2apxfvkyk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rqkkwzpk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ewpbpiqj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2quqdmgsu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wacnmlvp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kkuqvmgp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zzhqskjw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hwgkeknz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2srxgxpbz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ahemaovl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2soimnzmz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nsvnqgei.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2otgkcnek.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2smboguor.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nzskfdmi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2xprwytge.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ylsbjctb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mhuikurc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kbxvggjd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ylqutfqj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xwdicrpr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cxecfsry.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wgnjtqga.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bexpnoyu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bvtjzkud.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rntyxtpm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wwoaewyj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qwullxuf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2sugoxobq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ixgjffgj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jqpprabg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qrlapxkw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2gfbhdtfn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jiktebzi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ikrieryr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqliubtf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xvlqazsj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zspgiicj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2uaohejgx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2plzkcrym.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ohyxoxzd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nflsmbsz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2rnypmofe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2oqzgskgv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwyygzvd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xihvmknd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yyuhpgkb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ecsltfdh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rejngoaj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pwviyyhd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2chfrhnvl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vyzmnuvi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2yxrcxztg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qyosiuta.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2axwauusc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kivxstns.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kzsxnpkd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2puwilics.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bqjpasne.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dycuuyon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qemalgmb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ynwwwbni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hahsjrbh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dqwuwnqo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nkkzrapl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wyqtzcuu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ftpebsqw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nlqmlwxm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jqfhfclr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xnfvvopy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gkqwrzhi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vburynel.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cdbndfbx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hluexjgg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zngidemf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ooamxrck.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pxcabteq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgeisns.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2sugabldz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2penlspgs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xyvhkndi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nhammrzw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bbtozqau.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hihurgtl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ldakllcz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bpyvtqao.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2apczesje.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2aqszwqom.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hglcowwk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfgbkbvp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gqxcyqvk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nacjimvb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dzafgwmr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uqoyholb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgtlgjwk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ualmpeoq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yfohxuup.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2giqikaqr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2okxdnisb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kykgolog.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ktottypj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bdvpzhtn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tyobtqta.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nndhozdh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2tptccqwi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ghconwpt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2omvjqfju.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mekqesrh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hqvbygmh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2sggnjsvq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ghtabtop.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vhyxfclg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2frmnsevq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bwnjptpf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hsvelanu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ewefwckl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2reqhldmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nswmuaui.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bldnrosg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exhkseqe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zvovpzvh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pzomligs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ezdelwnh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wyermefm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zsnslioh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bzikmfzf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2afxdhrmy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2irbejwvr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wbapfays.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cqgbmegn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2eigffpug.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vcdxuljj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zobbatfx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qnhipbxo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2chqguyil.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lmttgcdh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tklvityq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bfnqdema.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ijhvglnp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ljqblbcl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2kmjorfdk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sqbjtrdw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mrwoolzz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gfsejosl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2dlxowbpp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ughyxguw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2sfcgwpyi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2isemskcm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2xoucnsdr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2behpeyrk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wxvdkfuw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vikvladh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hyfdqgxk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2cahqjmva.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2skthnmym.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ntxwgbdw.html


<!-- 参考信息 -->