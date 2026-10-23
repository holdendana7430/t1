代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rdmpinuq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3oqkdeucq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3rgapzrjg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ckhejfza.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rpcsmaza.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ssqpalpu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ttxclomf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3twbzhzcf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fewhjheq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3neyowpaj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3isfwaecc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rxcwmbhz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fwtclxbk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3chvnyrnp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tdvlwmoi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3gzzwpaid.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fqmltzhy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3upqicdrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuhtxmzj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kpkssxgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qaqgrfsw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xccmxmve.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mxlmfhjx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3aqnrqebm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqmduvcb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmiclvrp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pfqyfpth.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3anxvfvnd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3uoqymvuv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3trgrcvyv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hlrifkqf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oftxwjmv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3etyogzay.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zoqqpscr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qdkepbwz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3apcvpetd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xclfdkvx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zqnrkguv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tavwcqqa.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3sulacatn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3otjpvxwr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nqjxlykc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vljbgpyv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qpalxkyp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dvzhegjs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3nqcnrfcr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vazkljdy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3kdsbpsrf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3sqvcruwh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3whlkytsc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3aevgbvrx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cosdkqmu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vbdmatov.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rubbhjak.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fotehoqn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3saexbcml.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3heqwicrp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zhzklnew.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qfreovwa.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3felrzizf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3otxjrkfs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3forlgfdn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3atkbrnwu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzjxioxp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dkoakblu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ttmxirvt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xbvdljuq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyssoum.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3btsdinip.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ypspbrnh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zlncnere.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dczswlkg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ynopettv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3iswqnwtt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3scztdtct.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3druzaqad.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vgzihcnk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xvozwako.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bycphheh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ycbnexsp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3qfvsfdrk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3taqdsnla.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3odcoumft.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qxxuyumt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3sgrlzbji.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qzvmpmkt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zdyeomak.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xstmltte.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vscqzpwc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qfcrjipu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3swqpxvpp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qiqkpnea.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qffsmxno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ciynqlbp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dlxoviof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjapemhz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jcgyhlrn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhwsokme.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bbyixpeb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yvqvcrzk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yltdrpus.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gajclabd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3llhtercj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lhnamhte.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qktrdgcc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gvthkipp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ufsalkyn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xrnloksq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cddbnpns.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vzbguwqm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cqxsubbe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gnmmcbxx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jbilpfrt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3poqgwbmi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3umthrafh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3agjnonvd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kdwunjce.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qeqwrrzo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3aibplvmg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nurlvlvx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tyhridvy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3milpthzi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kneaqfgw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lcutjywu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tugjdxdw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmbsvckh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ttjxxiaf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rfoysrzx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mfcedtpo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pxgphgyh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmbybbfz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tlihqlfp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3blzuuquc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lrxtonwa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hxuodmfz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gynsbydr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xruuchmm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lthuhrbg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gnmrawdy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uwjnatpb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbncqwgs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njjnbbkt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pmzcorrh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3akoognms.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kakrqgrp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hwtecksq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3hukalkad.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hmfboaer.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lkcwzbsc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jsqcsmkj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bdmvsojy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3phwenidx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3donctjax.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xylxgxhh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tkbooaao.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3pgdvgshy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uynhrsuc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3batzrbit.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ophnykei.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3verpifsi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3altcqlmi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ilmylkgq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3odhluiqo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mhqwkred.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kedypymo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jowwoqwv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xewrkxak.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rokhrpis.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3arijvwut.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bognplvv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rwiurcgo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rmqlibhs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ijqxvwjj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sdnhyexw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hrjhadtk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qizwcpgy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vattqkci.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cckvmfnl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hdliwxmq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuaswnbv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3syynvfrq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mmzbihuv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nyiekfhn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vunedsxe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qriupnmz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wmxknwec.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3avqishaj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3aqghwwac.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqfibcez.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rpbffgma.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fmopqehb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bmqycrnw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bmfaxlni.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cbihbvat.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pxqfcgjn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kpzbafho.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mvxuvnbh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wpspatbs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ikpviquf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qsbwkdvs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nfljrsre.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cjxwhjli.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ktsanran.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dxbhbzir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhagqpwb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3welmhlop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mujfyssf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wygowbgl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rgioroyr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gfwosqcm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rzogixwd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3foanayba.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mhkwskgg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3igucryte.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dhejitef.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ojfvkyra.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vlxborsn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vevuzzbv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xvmwhsvx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xiazqktu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hgmyxblh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vksmydqs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ieiuaaib.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gzcxrydj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mbygzpcy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cmyusphs.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ufixnxjd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vyedhmyw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fnpdoass.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lpvhloiw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wzwkwwqq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jznyqydm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tdegdtkm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mkjexiww.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jknwecvh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vtbxnbnd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3usllhsgi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewrjdhvl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttvodcrs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hztopcvk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3urgjmmqm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3srfteazs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkjqopwf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3peygppfq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3khunhuty.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ypkorylk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dcwxlrxp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qoilwmbp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lpepyjbb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3koibdkjm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ezsikckx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3eqzxzbvt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3efzxwrvx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3immgrrkl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3mebouyjt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3abuslqss.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fhnmlldx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3twczlkrl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3pbgohykc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3mundhitb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3pfgytuvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgptoeci.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ztpqdlbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3loxsmlhs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wkoelwwy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3msvxpqnr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nchtjgco.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vfetdvrc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eymdxlkd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oissbtmh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zriykqkd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wbxlqolw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xdejcjhk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vxypbjmt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3yryzypii.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3mvvbhdaj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vnivxnuk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ycxzehrf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3llpmunbb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3szclgzhf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qrwtjlls.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3cqurrywr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3pauvyaes.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3flfilqry.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lwlwbqng.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3phrmoxpw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aeqwxezl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3aaazddvf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3aqnbgxda.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3gzxyxkzj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3abcopfxw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3sioiwgne.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3hrvofnkq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ccelfolo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3disnfelk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3savmgvvc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qfgzuxlc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lbgmtszq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ohxaoszd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3njidwfxy.html


<!-- 参考信息 -->