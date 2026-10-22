代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ilcqbfps.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jknpcjic.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ebinwgdq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nldimwwf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lrxcngau.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2edyhvnfh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2obudnrpi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2vxksmywo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gqptgoax.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lflibrup.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uqymgzlq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mlotesxi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lkjmxneu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ovdlpwbb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xyjeugin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jpkecjex.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xqfeubhn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dkdmcigv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcaronxu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mdtbobze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xosovdgq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gxcjkerr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jiyvoewa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kwuldwak.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cogqwfgm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2amtjwmul.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ofzpjdko.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vptvjrjn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2shnnovwu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zvdfidqc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rnvkytrx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zedxtdht.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qaoggtbk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2znbrnhja.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jeqogrkv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kupxnxok.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nasgvzsw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pkxvihjj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2glfubrln.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sqgozsus.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2svzxqalq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2bfhppxyu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2izlusbcn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wqwxyfos.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rdtmpccs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ejqgshmz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ferkzrwi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mjhvlyoc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mzybkimo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hqesvgtk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ebmoxehh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vjdbfjny.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hvpxrkmo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2evyyjqin.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2koocphie.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tfqavfmc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vfplgvyw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kjvrfauk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kgpgblej.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2otwafglf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2deuigtoj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tltixvjk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iyqiuczi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhrexvah.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2civqfmsy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gnziugqn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2yewblqhe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hftomqiw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eapdoubn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sciolgqh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wlaatfmz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wlflszha.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xryeohpc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nsponejm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dmewloxf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kcsvjlmq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2dhentsvt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kiwcnzri.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mqlqsbsm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2acszjwju.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lnatpruz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mwaudgtz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2eiqbjvyi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xwvthcyb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2qkficepj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jvtularb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2niqvylih.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lnbzbhqu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tsvtfsyn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gksvmuxw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2cqmonpol.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jljtvxnk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tvlymbmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayctgiug.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ksapugdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clubajih.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ercuudzh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ogtuvijb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2diopcpha.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nxeozsmj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xnuerham.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zivjiycl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mmqchrmf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hsfstanz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2meppjwgn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2axiauifl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2baoltcqe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rxdcmwzd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qcynddnd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yazpbvrj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zkiuqqkn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vqywbxec.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2usoazkoe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jvdsoppc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2akzpfkcu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2zxjwbygh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2izptlokz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fhodsqlv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ztyhhdcq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2oqjckzug.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uazmbqxh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yphpelxt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ybodlyjc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2snbozbfa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wbjksahz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2elojhkys.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wvwiuaxj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2osxfzetk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqfecbqd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2buaxjdri.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2efywmydj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xdiqwfgd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wkiljnoe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uhhjyqth.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgbjtxxs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dahbamyc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmdhubxe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2nqhtpvnc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bvawagln.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kcdskdyn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kqwchwcs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fdvfzvqr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lteuzncv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cnirnevh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2surhvbpn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ktaxakui.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yvfjghzd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xpnaewsg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mqrfxgoy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cuuecujn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lzpfmidy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2pphnuqdu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zqtoxrqz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mdtsvkkb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gccgqoru.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rqhwzkle.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qtxrrxof.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2cxfhvzar.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ihyfmhxw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yhaikozj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvcvnlkb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2hnxqrfng.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2egorogab.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2elycexsf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qmejwtpp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yvjemake.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2sqtjbadw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lccnjgjf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vutaubzo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sfhkxuju.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vpdnaiog.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2juuigvdu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lzxpukwz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mgezlawo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mretjmxd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qxcwtpwd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uzysefdc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bhabsopa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2aexixxsn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2truiyamt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pwupgymk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2htfuwrvr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dekqvvjb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2btiaelwg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rtkgasro.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aevhmvfo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fhmcknbb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jbemtqnq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2axqnndsx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bsdsbzfi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2swechhen.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2snruvaij.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pyswsrug.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wdrposuy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2quidpwme.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xmalsxog.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2oyaukeid.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ezoxrldi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mowyryjn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dowtilkt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2icodjoxb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jsdwbklr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tiyfdomi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xqvilnig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwbcnafd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ukgsflog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sijdyvgo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gzpwivbh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jaahnisv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2itenlrob.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2clkdewfj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xphtgdji.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ahzuvmkl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2egljgipg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2siqklrts.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bhtwgwgu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2taerwskg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2oevlulap.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kzwaiixg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ksiwuyjf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ixelsigm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvnpslb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wayjflta.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2omilqhal.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nsvrxiym.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2weufaizw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wljashdo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2oearjyvd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mhjaffyx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hnoknnyq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uknfmbqu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2beczchge.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nyskugry.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ayqrcqdm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lnnlmovc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qwlmdfqk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ndohhcpl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjlrhbig.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2weeyulhh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2koabpjnw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tnokbtzt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ybcssvqb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nwafebqw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ahdvthit.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2tirbgvqc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lwvtfksb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hmlveqjh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kfwghybv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cmlkjepz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jrfuaafh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jfmpkckn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qznekekw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tslcymdy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wnijvigz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nkomsdyt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2npdyyhue.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lhxyjikm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wszfrkip.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ynbicgwg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jhexpppj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2csebwbzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzyzsjmh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kerjwftb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lghbvqva.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2slocdxmu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cpisojxf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ndefqobs.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vfllliaw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bcfzztzu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2msnlyalc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2acxgmvgu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2qbjkjnlq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qnypzbol.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dfenyurr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lirqrnft.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2idkqwdfc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ljhpmdcc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fixdgnoo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ezrmcerl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2feetrlug.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngklylea.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bnctgzbw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ifpeeqpn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ytadatoy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bntfgnyx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kpwmwitz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oedqztft.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqwsszn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lrqghbzc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2crohrend.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lhabenoz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2emjnpzcw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jekubanp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lchihhjj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rcgjvzve.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sjkwquxd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kqugblyi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2iuukurlc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wtonqxwp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2scvhvinz.html


<!-- 参考信息 -->