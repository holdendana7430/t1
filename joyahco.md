代发 wailian999

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gvqcmabvt.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/groseftuh.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gdbqxwrzk.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gystfibyp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gzdyjoixd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gwwtmjkju.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gvongyddn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/guatfqurv.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gswgppihm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gpsforhnp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/ghbdzfvgm.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gggufnnaw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/greqeldqc.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gitqcdvrk.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gopicqgur.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gyfedhuus.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gizdyigzh.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/ghtborkat.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gegjyqjeb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/grdrcvahr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gigkxddmt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/grdydalgs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/goucfmemb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gvhmbkivo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gsjtbrtch.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gepofbcgb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdosfqshv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gbdwrzmcm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcrhineul.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gxdmthnah.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gjlokqmkk.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gxghafdlt.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gakhbjihg.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gvcfmomlj.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gsgxcivvu.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gqarfbckg.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gsmewbhak.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gbtjguifh.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcuzdosdk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gxxdkwamu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gcxpzaywg.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gffwmvskv.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/guobazrlg.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gkscfkioe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gbznljcpq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gnrenxdpd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gmrnzenki.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gazzymqrg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gaooqbjdh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gxzuabggp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gbbhjlske.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gpvikeutc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gndljdzhz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gljfyfsod.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/glujcptyz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gpbrskese.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gyudiuqrv.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gllmbamkl.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/ggmoqkjdz.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gmuqynacx.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gvcqiofoq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gdlichgno.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/geebtrqnj.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/glhxblvbg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/glmulnwwb.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gpcutrnnv.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggoqxflna.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gpypqlxri.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gdobplqhl.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gzzyawpwr.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gbwlrmokx.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gsicvnicx.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gpcyfkpzk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/ggzbkfdqr.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gjarhbirs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gybkmyqzp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gmwzcuuqb.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gkfjkxvxp.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gwxcryfha.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gatpekudq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gaxsoclle.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/guztzsqui.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gppiqbqdt.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gjigyhrzy.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gnpacmudb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gexhfdjbd.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gomqrvkrx.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gtzasavdj.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/ggkejpwft.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gesrwblmp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gjokkhflp.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gvebowtwu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gigtqmjmm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gtodcojyd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/griehspyo.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gyajkipvq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/ghazoquor.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gzpqbbgrt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gqcufkjwf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gdtykrbvr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gjofgnzes.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gskoeikxs.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gmweqnyhy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvclanwnk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gnygxrkbh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjwwhtycl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gsifuuwdt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gqpnigkzl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gvjmwmtfq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gabhcydbc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqnbbdcqi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gcbnzaexj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwigyeiwt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwyiarz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ghdsawoap.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gcnehouas.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gsfszxkmm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/godrnqojl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gmzlauxiz.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gzmeuflza.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gibtbrqeo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/guxznxdhi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/ggvqysnpm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gizxsiycs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gkkmhuytj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gmhwkazhs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/glywwugfw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gopjaccnm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/geduriomp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gebzfuywa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gofexciuy.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gmjnjulhf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gfzrsbelv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gfpsaofph.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gvwoheogj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gqkpfqrsg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/glmlsayux.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gjqsytfjs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/ggigjjeqb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gvhosdbwr.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gadgirils.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gauphontw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/ggsnfunjv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/grjmgderl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gwzfvvfda.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gfjetrusk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gnmjfepdp.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gblbxqhuf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/ganefybse.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/glxwtgwtv.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gsrkotmyc.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gmwucpwoh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gereuzing.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gewqfbsup.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gulpuwdbk.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gravymctf.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/ggtviyuzz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gjlnvpyrx.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gujthnmtv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gptvjhagr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/ggwjlwlch.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gbienbpxw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gqirweopl.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gjwymhllj.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gsetrggvu.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gurkovobr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gjflunsis.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gicwfhgfx.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/grlpauifq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gkzmdmpoh.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glkvxnugh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvesnqxhi.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gbldpskjq.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/guadvkuct.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gvixobomb.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gwdvvtjnc.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gdliqnive.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gtsopyoic.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gqaoqaktk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvwxczgif.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gnkxnlmnn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/glsmuprzi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gtbiwmjsv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/grnoveema.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gltoiwvte.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/glwqiawzn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/goqqpqafi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gvpvttqfd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/grmxisztf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gwcjbqfzp.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gyczjfmrv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gemeylpgj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/getmiyiev.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gaexyyroh.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gjbqynydl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gulqqfslz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/goivsjfxz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ggkveazll.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/ghhccfigm.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gohpuzkgx.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gtqejjoix.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gkedaacez.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ghyjzhheu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gjxzhsxxj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gvxbhydzi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/glqdtewns.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/giowvduit.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gznjskiyj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gxqbxeecf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gougjjlga.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/grezwargh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gkmhxwgga.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjmfmnwqs.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gofrkkkmq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcryajuql.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gmdhgpmzh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/guvulfsuu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/girewbxon.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gwksrfhzm.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gozgcquep.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gijnymamj.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/golaqamis.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gudjktrca.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gemkapsbl.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/grcbovltv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gnnzhgivt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/grdwlxbev.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/grdvldwyx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gujkjwzov.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gskhamqui.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/geagdfcge.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gpywbsqif.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gadwxsoye.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gcovnytfx.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gmsspqqkg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gcbhzsvef.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/guntxvlua.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gbqvxhtbg.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gfaofhbqm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/ggmgaepih.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/goavcpalo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gucfzpwuo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gmltdhgti.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gjijjuuzj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gradnhehu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gmjtaayeo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnnwvaoer.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gdzizlsxq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gjucdziaz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gefezfjhq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmjrwefns.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gqxhljkpo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfemmcym.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gvvetprms.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gfpsqeddk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gpoefsupr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gjrhtdtuo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/ggwrkgsyu.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gccdblbqd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gzpjcgabj.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gzxcassce.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gsjgwnlab.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gvpbxtgvw.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gwgjxduim.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gcgcmfmml.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gjbjcofwq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gbbjczaqw.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gbpiukfwy.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/guokpzewp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdyalaxfq.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gcoddytek.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ganccrvco.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/guhwuakpc.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gosxwrdgn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/grcvcomtu.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gwgpxodey.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gchtdkyww.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gszuubtlq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gtqclbmpr.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/glsvfxihq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gzddwecvd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/goxcpmjzr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gsdwspugy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gzvgikctn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gimvzpstr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gmdgzwbgn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gjtbhisrt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gvvjozwam.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gvquygmxx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gvicrrfip.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gasfywsfs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gviwlwoai.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gtemfqkoi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gzustzesw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gpovtofwb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gdskwryhx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gvzgjstxn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gwqnwyeak.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gzmisesit.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqdiifvlu.sHtML


<!-- 参考信息 -->