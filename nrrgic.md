代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vrahqrft.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wrdfswky.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aktjovhf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vtfnhdjy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lhdnujjg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2pfvpbeok.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2oguiioeu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2smpncasb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ssszlshh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kllbidjy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2grwjqnez.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qgjdeumt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ckujwhuj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wpgagben.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2apfjllki.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xmsppnkl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ysyoxjbm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2smlhfvfd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wpcemotc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2psoxmxbw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yjyijoeo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fuxlales.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2otyhaesv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pssykkfq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rjetyzra.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wqytmvnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vphaapge.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gqqdthhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyzuyhjm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gthnmavw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2bkwivesd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hrhvoxgh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvfyxunz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wahvjbal.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xiqfdcja.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wehevomj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2dzmhpipr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mpdyghgz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vwgttgyq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lzzglefi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wclsawrm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iurvwiui.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rhhnozpk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vscbbmrk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kxrmzvvm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wunmofww.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nydwgtio.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fhwpwvtz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hjckjlih.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gxbdqexe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2iyigghtx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ibxhkqyo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lltcjxpp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lzfiwncu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jwlrqdps.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lzccclcx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wikknbcs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2grpwiskh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sjxtgsqa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dpibgzyc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mfccrhsa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rjurlgpo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gmcuvbln.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2runnrnjl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2rwgbexcd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ttzyjfwk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2szcmaqmo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iohbyxhs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bwuzvbvq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pzcxnrov.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bctyfoww.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2biknrmqo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kgphmryj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vnairdhz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hmotzazu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zhefgqur.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fjclwghm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2elkolwgi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vczpxchh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dpjiqlob.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dkitjrzf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2flgizfmx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2osqbyeks.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cmnzbxuv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ttqsjnof.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bgkvqkla.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mgeghpfq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zicmztqw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqgptys.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cbonpjvx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hurfeuyl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2duecuwqu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gokqhexd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tksmqmtz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dptxxcri.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xexzqyzp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jdrzassi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dxssqity.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2irwtigru.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2dbsubwgu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hfbzknxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abyvdodg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fdbacels.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gruzezbz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nfaszggy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeijvnht.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2buiyepow.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fqsqpuxe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wwgoggsa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbphsvwy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aaltjjvl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2gnwuhlhv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oimtfhtc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2trnrnpem.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zgsnbkbv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sqdbskhv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eiibbjaj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fwbbjaxa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2sxygofwb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qakbkgod.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jrqjrfrv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zahznajr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2seufgkor.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ebilvwgq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2aunxiizr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mllbjauk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hkqicvyy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vvsruxkc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rueogius.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dizjmyhd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tvfpruhk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qoqxgymi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqejfhl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkybzgch.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xtaewews.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pewcuxob.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojfbwnxf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2regvgmsf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzizjxwq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bwzgjosq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2tseqptst.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wzhmnsfb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kibqzhjv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2szjamfwf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrrvcjwa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2slsoadsz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cwoazicj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dhpprczk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xvvvwekg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2nlznyrpu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ihihabhv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nozocapt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mfoyxwoj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fzbllxox.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rbznotiy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2iuabquis.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gnvxxwet.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2agauvkhe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2talfgdhn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ghrbqtaw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2saqntqrx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yhvpjart.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2itarocqc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2omcpxqrn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gmhhhhme.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hwfgnzlu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2rmizxcww.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2xmrkttjj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sgsatudj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gxbisggu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sfskdryh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ttpoyynz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wrtmcagj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ujgbfxhw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fevdpsgy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bzlvnsrf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hfpljzbk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gunfqddo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2killxxcl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ecpyrzig.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gcjuwmmp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fkpulybq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tohasowv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kqahjqra.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2obriuehb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kwavlyle.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cckqwbug.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnvwciyg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cvmohehz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2quqrnoua.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vhuagfov.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gwflpggy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2votxnopx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ozzpsbzc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2avnmijln.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vsivomsj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lbixgozv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gdvoeint.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gugobaie.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nogbbfek.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gzvzfxan.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vfjpkrow.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2plhbtgif.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2lgbpntdh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qdwihgzg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2emjwspve.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ucusfghc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pqywebwr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tuwxgike.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jzhrzehe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2alzezigy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vhjegwjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2liemujwo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cfcmrkui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdjgmkqq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jriyesuu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lhrebssa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2sufekzwb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2radcgzrr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uhhwondj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lwbylbgp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lkobwgjo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2tshkmmef.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hoyxhxjp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ckfgptpe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2eljzwxwe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2segpazur.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cginjukz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ochvgdmx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ewuzqbwi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rzahcfpm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dkbvtpts.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2emcokgxu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fgsohrvd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xbuwigzc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zptlrleo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qonfllws.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mdfefjgw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zxkihpck.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bketdhht.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jstdftcy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzjqumfx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hjkqgxwb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ycdzzsfn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vxphdslo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kosrqsci.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvjxooje.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ngiccwjz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fwpxqkkj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tcvvpxjb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezpejzrf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kibuaijt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qtttmoiv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2llqxvmek.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oumvaxyg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fxjvdbdr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uftttmsr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mzgwnapd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mmesbnxz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjxcsybx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2bswksizr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wzxukmpo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ztkfwwbw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mbisejro.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wqbnyzfd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bmyfmwyr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2irgbnkoj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lyoqyljg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2dbjdefyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzkkquhi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxldqjgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxqtpqvh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lriatkga.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wdyqkltz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xubagpxb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zrnziemn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2poldvfly.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nhacpzjq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yvdwfcyx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mclkqiij.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mshtnulb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vjssypgk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pvgpmwgq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfgvjcyl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fyimkeov.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2imlgicvm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jlqosntb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2wrvfhdxc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2sqzvdxcp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ghujprek.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rowzrjcs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2eubeycmr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2njukycfg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wwedrdkd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yggrpvhv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2riwglwep.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2cwxihjco.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcczgsf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bvgoylaj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2stdgplis.html


<!-- 参考信息 -->