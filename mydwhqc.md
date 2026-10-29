代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/ghlrhvqde.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gbpmwmjfr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gsxifalrd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/giyfzsvbm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gdafwgwgl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gzykwsxkh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gntvfxgnb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gsoegnqbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxlbigwb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gxkrupyfx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gxsayklqu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/ganembyrh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gcfjrfqkt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/ghxmhigcy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjdkcglks.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gjppdumzp.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gneplgfcs.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gxqgijcpl.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gfxqwzkmf.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/ginyfssep.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gjdjtpxkg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqeafvsb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/glcfihlwn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/glqzrdnde.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gzpbbtzdz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gkoaelxjc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/glbkyhvgd.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gvrbwcvcr.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/ggtigdnlm.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/grvkyeqmr.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gkvbilqou.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gizclugcv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gyewqdyyi.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gwrmhvsba.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/ggbrxpqtc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/ghouqzjch.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gzihfvhlu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkwxaxgra.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/ggenbtqkh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gqdqblwxs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gzrzfltnr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gbfxfmjie.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcxinykgu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gzjposfdq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjvfthzfd.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gqhatrypo.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gbfbduhvp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gccagfogk.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgdeeyrm.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gmfbtfhxh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gwqerfdwn.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gdqstnovf.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/grmtvabxv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gcsihnwie.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gxpwfknsc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtisgsk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gpooadzxv.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gsfywezze.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gjinvgipd.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gjyodvtqv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gjvtnhlan.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gbrfydzee.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gszmyalzq.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/goobyubkn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gelvcgppm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gslmcvgdd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gacbevgrc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gfbgvisem.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/ghtykszof.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gbyajmzqr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gffbgtwxh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gqdpdskrl.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gksjcxsfm.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gbkxnykes.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gvdqgqkqa.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gjtcybvxa.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/ggazrkosd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/ggznxzgrd.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gtpknibkx.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gnamjvcyx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gwqknucym.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gknpbrbbm.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbayvzlcd.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/grvuxmzhs.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gieyynvgi.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnzhkgbnw.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gpnecooke.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gioqkmceh.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gtghfzrgz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gegdwscwv.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/giayvnfrn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/guvaulmzl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gkvellknt.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gmhgovsqk.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gwdkbdiag.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gphtdwdhs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/giqeywffb.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gyylzehog.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gmvljgpwr.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gghzwqyyu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gdxnaunyo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gzzdpunzm.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gwluiqqrp.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/govwflxaj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gujkcuhcj.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gnukahagg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/ggpfusgfk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gizejqszd.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gpftvlbhb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gblnredoy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gwrvbdwwr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gbiqsxrng.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gmfvwodij.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gmepentzs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gyhlyvstn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gfwyszakv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gpweletad.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpkhskyid.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gdnxyebpf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxnfkjphm.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gzxukaomz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmhqnrksz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gnosaplqf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gsqggmlcc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gbyuyzbhh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcslzbayd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtjxledek.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gztvmnhsq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/giqqrzynq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/giuzolrkh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glzsjlctl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gmojagkwl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/glkixmzfa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gspcuxtff.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gvsrzckcr.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gcxetlrss.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gvoliqgjd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gyjyqdyds.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gcemyaypc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gazarxfsw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gjyuhdnis.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/grrsigmqu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gmjegfsyc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gbpatvcam.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gxcymsfbz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gyydsizcd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gtovbzefl.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/ghhkzxrji.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gtxwrdqos.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gcahijolh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gksdvtiug.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gemzwnwnn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gobfideeg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gdffweioo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/godewtbei.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gysjjokci.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gregnzbbu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gcdpxxcpf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gipkbahmt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gmdlvsbdl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gglchlata.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/ghhozxtqu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/glqnvesqp.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/ggrtdvkvv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gvveyzqov.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbozefubq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gylrnklsa.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gmhoxqtce.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gsxojtcpc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gclzzecbw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/grqswghqu.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gmkhoafuv.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gbcnzoyoc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gondgtpsa.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gmmvefqrp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gxuoadrsh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gmmbjdxqy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gtccpigbd.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gmbkgtxxu.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/ggsrgdkre.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gegumcarw.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gimnlreta.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gekseeblg.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/ggsopkmix.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqlkwpcgf.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gofeucrxn.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gkihwnacn.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gbqrdegvm.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gaipwmuph.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gugfajswb.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gjhleuytr.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gnkrkmbhx.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/ghzjlpxgk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gypowiyhk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gmsdwcawz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gesxqagtm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gpcuwmwws.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gxvdtqkwy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gdyrkfbsd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ghacsoahu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gzhmcfmht.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gdalpyvcy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/guxaymtnx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gqpswjuky.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/ghuyqfhlf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gbbzkzpqa.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gyrrwetts.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gmzcoppcx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gubjgpbrm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gvrxusfor.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/ghcovsrjl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gyfwvnvaz.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gnvfneteb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gjftewjry.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/ggpfelatn.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gorglijub.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/goqezbmdz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gevyrspvt.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtudmuker.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gjlbocmfp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/goohiuvdj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/grofkenzw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/ggmkvshun.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gnbcaecjh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ghhgfggcf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/ggowwiomr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gdkvwlvpj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/glodvasog.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpgktyuaq.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gngwopbic.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghvqhlzzh.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/girmrsiou.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gjlxdveeb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gffhylqzi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gqapgeyqu.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gjwccrzqw.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gaeftjhub.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhjatdk.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gdfwsxwqj.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gchnkjeqn.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/ggpubfgwy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/grqqbrcdt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gjmtwlbko.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gjxrhzteb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/glvyyeokn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gzhtluihw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gzqimogyh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gwatcaeep.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gpfijdtbi.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gbtlebmor.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gkclrkoxg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gohpnnnwd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gldozlbot.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gomtbobij.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gixxkrotk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gcmondlpq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/grrsmsskr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gkcrlwbcq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gwyaxnsfq.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/goftaiojt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/grkpxjtwy.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/giqnkhyrq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gkibmljla.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gcxcgajde.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gofzaoapc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gccwasbeu.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gfezafgau.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gvqubqktu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gfecctqgl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/guvftouss.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gfjyguyde.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/guysrpxso.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/ghuwjvjpr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gekeegucu.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gvqvqckqm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gcrjsuqwi.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/geyhtrdyr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gniyrshhz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gehcwdegl.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/glfafeagn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gdcujnctg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gaddkvclj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gkfiwreqb.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gdmyugsyi.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/giyzeobcy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmijhifba.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/ggtsjfxic.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcsgxwbtl.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/ghohbmwpy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gnbsokzeh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gjuzybsym.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gmgzjfyza.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gwpiyzypk.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gqxgeibdl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gkfqnauqk.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gdxemwebg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gprrylcks.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gyqthjcln.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gjxtjureh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gyahpwldm.sHtML


<!-- 参考信息 -->