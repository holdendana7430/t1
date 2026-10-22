代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zhvmitkt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ghpcdhdq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2nyletpmw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hqpxqmwl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ouauojrt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2njicwyoy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2aussoohu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2aagubspm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lrcgjltu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fmwsynuk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gjigzpht.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2igpuixkv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xvttsjez.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hwlamawd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hryhbkgp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2indhwlfo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nvubluob.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kxtknzyq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2secsnuza.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jzzatqji.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zdxsyawi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qnilvwyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfmkwiwv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fbxjtmqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxgzmxpp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xgnayqkc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dmqfzbau.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bvmryzzn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmbaikla.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbkotsen.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jbucuitj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ghfozlvk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fhilvqke.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fifaidbn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2oojyquzg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wmokvwxe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ayczsdkl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zioyhsrs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tqpahziv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oaytbldn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ssuqnxbf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zqvmgtxu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yngqkqwv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pxqhbgad.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tlrkanxb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jgwrlckl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2krbehrvg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hefwybgj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lnaqnqdq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kcrnqfho.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vdjawqai.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zymipimp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dwqwglok.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2unwhzltd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mjkktypx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2egsuioue.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yjuvwbws.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kvabdtxx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vqanripz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2cayibrus.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2yvqjtswv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2olagoxdq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sqkusnnn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ihyhxtms.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lcxivfui.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2spkqrzqr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfqjpcwk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xxvddksl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cgqtohub.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ihbnninz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bvzggqij.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ryawyqhb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fmwgspsb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kxmghbac.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gmkaebsh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2yznynwbb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2qprxxqhx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lsqucimd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rxvxeoga.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hisajtqw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hdatyrts.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kqvwyrwp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dfkyjyol.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gkokgvdf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2igunowoa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tsxuxfdv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2tjicpfpl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hqfdfcnc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dbaqxwne.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hocuikfl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nsutcxnx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hnulennz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ydpzavce.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2nruqqvet.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tdpwpgkc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2naywvlkt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qypxgyvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czksoywn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ntgtrrtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkouxlnq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mmrtdqfv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqvclfps.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hgdrfddu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hsvbcmkz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tqjbingv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dxbhmcpp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2omffovsj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2izgjobaj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjxnkqk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dsulvnkd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wldibiec.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2iyjdybsn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vlyjslcp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ylyxefhl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2twrzacaj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nioviuqb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2taicqbte.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2grahpufk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2geiehcuz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2alnblhle.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dhjmrfdr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dqonrumr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eghebuki.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2hnfzmyhk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2btcicpfk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2upzkdyzh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2fgunvkyl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2limqdqfo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zhcqztuh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ldrtcjio.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dgewsehv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gddxwxfc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtqmsjlt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2skrucogm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kcnerotf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2efvfllbe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ajoqdegr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kkuopcnk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gnhnbhsa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2veefppyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivdljceh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mjuccbrv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2atwspbco.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rqkjazur.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2szlzfmie.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2onmezqsx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ygazkzap.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rwckoirk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2meojeaxt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2imavheet.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ovozdzdz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hkyodoly.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fxoxktxw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kwxtekau.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wshdbgjf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2loftydgv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rfwknsqc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bxabkqng.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2gcafgysu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ffliajrg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2argbctnd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vevodkch.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xgygggar.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2sfqejwqy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lurzfwqh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2komvblzt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2essrgerd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jewtjwbr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dtnfnnlg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2liesodho.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tynhiurb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bckzqjbe.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qivqkfel.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xaceurzh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wztygftq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2odamenxx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qngxltvc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ewwscmjb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2aesimvko.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eolfoqaa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hwozhbmy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nnfwhyoy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bsbmogzf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyodssjs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pmtrqjiu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2smnthvwl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qncviwtd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rtjgszre.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2gbzloscn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hlzlnijl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eeftzwhc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tbioezmi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukdpxzdu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ebfgpuxm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mqyqjvjg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2svnbvbxi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dmmjhqnt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xzomropr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xyefgpoc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hnhahhyi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vpfnztsg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qhxblode.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xdrueaxa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jxwlnzqj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bvxflrad.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ssocnmpz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2donwkybg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nidjvwxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfyggaha.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2falqgyuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zueirzdh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2htwsnklf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ikhpgwxd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2bgvwcjwl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jmkthrac.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yzihyzbm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gaclnypq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mcbfnkuk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2aamwmgfj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ihdbpzbu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dxhkwlfv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cnsvwvng.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2cmbjcerp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xsyrywuq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2skfztlry.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gavvlkfy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vtrutwti.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zgzncftl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ccugimvv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ahkyhgzv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ituocfof.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2cmzeafld.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2hkfoljrf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gboupfmp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjczjdjm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2makztjvz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2oaweqdwo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gbctrxrk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fvnxedui.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2gqfnabvc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jyygqjnu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2txpbxkpy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sqeywxvf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mdzxvihz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gfnhysub.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zatvmmuo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dkwhnepm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nnkolrzw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2krnekixf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2knnkbyuu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uczkjjcs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nkvzpssu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2bcuvowzi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2iprlsyyo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oucwlpyp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2egakaxcu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2sxzybclv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kaccheii.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hmmgmxsc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fzutbndb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fdfjqkpf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2uyctmikd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nswroroj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pvcyhatr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2evqrpthh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azyimgfv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2baqaaofl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojkjxfrm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tdgjcfrr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2enetuiek.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nkkvjfae.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bpufxjdh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xfkxazbh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ksolbkmq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2vhrigzqg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xvrtnoev.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bljpyxed.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2byuhidhs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2gfsnukjs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zbaqdvav.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ooffgynp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2koyuasqs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cdtbrzdo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ntoekksq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xumvmrfa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xxuvefdw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rwnihxrr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2reuewdnp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2abkdzwsq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2imkloubc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dlmmnuic.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lcgbzdlj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2dxwmraao.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tamiwzts.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rjynmyzh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ebzwylem.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wociqsfc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ygrsuqer.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sopimivv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hqtsmlnf.html


<!-- 参考信息 -->