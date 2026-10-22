代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kvooltnv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2hpcsdskx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pumexpga.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2crjphplx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2avjccqkc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2oprpweig.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qguqkkoz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2khvydnmp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fsurvixc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2htlqfvkn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cjujutcm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2pyutuajc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hesqtrra.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kzyaafvl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fklesgdw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2flvcuvok.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lknhrzfm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2emczkofg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lfquawxh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2pzpmtqow.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2atwpfdbb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2cfiwbryt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iacfjrab.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2yqiquqaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfrqywlo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qepauhfx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pvetpcjn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2soowdgku.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxdejxrz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsezmhml.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jktlwdwp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2iqihqvjv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2oakpdqsh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xldekpro.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ddzeniea.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kathbcnf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fxehapvb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qrfiehva.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2arujhjpj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pzayujih.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gwuojnvz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2dllcnctw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2loqvrqul.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mgnfvvrt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yclwsgfa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xfhbzzfq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2txhgifwk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zwsrhyai.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dshhmfwb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nlojbyvm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2tlzpdmqd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2abeqdfls.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2fdxmnoqg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yhutkffc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xphyckwd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2soxhhlcc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ejgwtivv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rqtfbqbu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cxwzcdoc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2htzhlyyh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2txuqeiug.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2uluxcmrb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulbytfzi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ouolzaky.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fchqzyql.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bivczqns.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fgwnurae.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yteedela.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkcnralp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ofrasdwj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ygchogdv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rqopgzkx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mvgogcrl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hhjqjole.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uylwvbds.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2piyppaiw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sndcpekr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2glqnehed.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yabfolnw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nidhyvak.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wsjfsjcz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2oxzvfhrq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2izkzoxse.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2djmrgiyo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qxpanlbv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tavialth.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2phrvzgcb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vcuxsjek.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dfavbujd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2afdyjhkr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2quuvnqcb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nctutwte.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ldmcfdck.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fbudmrjn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ptrsgepa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ohwfhaip.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2glasnmpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iscvhdgx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ioplvdcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpavqitl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cvotjnpw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzeejafj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ykyubrxq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vexfddmr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qhqqokhu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2chkrxycv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2boqqhiow.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ijomqpqg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqcxgwdg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vmovtfxx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qdtbfcus.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sflpjgyf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wholwbrv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mznntgvb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fgzilvmq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2unyouptq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rubalidz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rpsbwklg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tavoytsh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2otobbqse.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vrfgkwxd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wznlhqgu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ngvgxrbl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dejrywls.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2cduhhumn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ccdaltwe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mryuqthe.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wreuhyvz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jqfznwcu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fqphtkgv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2grqhhvzo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pvyioixh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ouexltfy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cflexafq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyoafku.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2psinoelx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nmwqmgxr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2etwwopvk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ciwinsuk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2atrlexzq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekmkuuxr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tfzxhzkq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fdeqfwjg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ceylcwko.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrfhewnw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2uctcoohl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kibtvvrt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2epamibhc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2azxrydqa.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zfauuoym.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2lyofkhnx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2olhaqcnf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yholcjrj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qjbjobwh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qjcilruh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vdljdeta.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ymprytem.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jufethmk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2llfrgacv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2egjxxcei.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lafbadxh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vqhkqurh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wkjehzyj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2icndjylg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nznaljiw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pymlfgxx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sjamwduv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2scpqwepl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2igoupjus.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mzkydxvm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eixsaosq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ksoymfeh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rvtdnzan.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jetlpagc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vrcyiztc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ligkefmd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jqawmvuj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qdsjvtbl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jggcyvij.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rkgmaqdq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2boqkrpom.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yzqgdgdl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2pnbacane.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2skdmrppl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qgbhvdzi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jwprpmmz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2amebflwz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2kfhjmkvd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pgfrchtb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2egcnnarw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ojhapokt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dvfwfqqg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2btvfyfse.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oarzpsdq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2neozeqiz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2naohkmwr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgwxdekr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2yfttxjdp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xlpalmam.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pziyerki.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lhafjwtq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mvizcnnq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2inbnwchl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2adbhxdxy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zlwnuqhe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mvnahnwn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rtmnjmhq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2khrgsumj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnfstjgu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uvoepyyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksigizog.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2mdricvst.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ptlvqxdl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pzoknfxe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qywldkix.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vijobiyh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tnhffhwn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vvaauhvy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fgrxaqub.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mngcvapz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ijuvvrgj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jqxuuutu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xirjzbfw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xwmxzkrd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lxnpnuwd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dujyrhrg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2nlvtonab.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cbcpoevi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2sneueoqe.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2crdnyhdb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ksfeiazp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wvqgcxte.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qsodklei.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fgilkxpt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xpcwragk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hkrlbghx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xczromex.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvbrxscy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mfvfgpyz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2prsdfqsl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bfzmahka.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mwvzlqtb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvfalgbz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tdedlkbs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rnvwcmhg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2iwixhdev.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyevdhwd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mfhjcdpe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mumsmzwx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2lvpznrnz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qtztfdka.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mbngfmcq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zbsdspqd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2czoqxgdt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zobchfnt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwunwvsv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gqazfwhe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ozfzlvbm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2eemzioio.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cdajkckv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qufuispk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xplfuary.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zqpxcczo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mmsyfqyg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fcdkomnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elaeljpc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xglfbltz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvpdjcvi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ayyrthws.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2svywmwvv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2iwblojtn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bwhqjsek.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lflgoemc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2eijwbgcz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fosebtkg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2shxpyjgw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rsmdznyu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2grtytclg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ezckpoqg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2biboeyun.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2eaeaetfu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2sjcmqcvt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ihaiacup.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gtuxitmc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqsthrg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mawoclyr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bctlqjwe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2bmjflcfr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2droisdji.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xofnkwbj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wzdxenjt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pdlvbjah.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vkubyqjx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ftogdglp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ukhmorhe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2sjefexnh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2tgfoyrca.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wwahjnqi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vhikbknk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zpafvncz.html


<!-- 参考信息 -->