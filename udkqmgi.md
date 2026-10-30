代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/ghmvdgijj.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gkxgwzrln.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gnbgywacg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/ggsrstxwb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gtejfqbjf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gsjjkocvw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gfhhwksil.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gxhvyjzrp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/ghmzbzpuy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gjpewqseu.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gyrgihclu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gwopuilmj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gtyhrpyou.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gbeaqonqs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gmqmluujx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gdgkrqajq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gjtyqchmu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gtxthuflq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxjnvjlob.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gzruzqhqk.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/ggpqcttpb.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwtsvdubz.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gegpfupzu.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gyuhwfbgs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gvqbdsepb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gdfinyblw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gidryuacz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gnghgvenw.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gceletxgv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gnvvearjk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gkmjwirks.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gidvvogiz.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gbctrnrdm.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gbquriuit.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gwjbgxmlx.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/glaybipgl.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gvrlugint.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gvxttkkhr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gunxopysd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gscaszgrz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gnyspdgeu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/graqruknd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gjjpkpnii.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gftbqzkue.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gyiwntryz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/ghuywgenl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gynqscyyr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gtyhouhyb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjbetgrlm.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gozowqdqk.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/ggxuedwjm.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gwafxajxy.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gtggyylol.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gjrqezqtw.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gbczwbhrp.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gmundowff.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gsueyplkj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ghweibrpm.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gcrvoknvp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gvdbfsrrp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gmzsocroh.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gavfcdfog.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gcpxbopit.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gaajqtqch.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gknxqwlyk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gqhuqzuno.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gvpngmcvb.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/ggouidopa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/givctxxae.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gaiatzogv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gkvhrvtat.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gqwfprkii.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/goamjnbee.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gfddaxtrt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gtrcusfwf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gzbqytkuy.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gupuknjgh.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gcevlrtus.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gvieynfkg.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/glthhqerj.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gksivvnuh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gmgghtvew.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/grhoiofhk.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/guwdlnwui.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gtlxxadvy.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gbeonvacs.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gimqwsetx.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gftanvcob.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gvegiweyg.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gifxjsatc.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gqzrqgxak.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gicubzvdy.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gqygcacnu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gipyyqehp.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gxthiuusq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/guzshfggb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gxkqbuygb.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/ggrecowgs.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gcfrhyssq.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/grqktrkmi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gevywniib.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gfsjzltgj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gmcsfblfb.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gmxyszbdf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gnekajrzw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gsnbckqgf.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gigdtsner.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gzntdxziw.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gscsdmmwg.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gerdlhdyk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/ggixpxqjq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqbwjfo.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gjanbchzh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gsoeyrbfr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gftfvllsk.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gdgdacksv.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gudyfavfq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gxzkpwtcl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/girljanqq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gkpmeqeqq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gwakppkle.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyoaoxryf.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gehvvgkrn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gypladyun.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gbsnzlfco.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkxmyjfze.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/ggngrtfls.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gwucqbchs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gprthhdxt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqynoiwpv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gijnrkdxa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gqsksbdue.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gngilitgk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gvklesvpn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gvfvupnyx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gofoacupn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gzjimledi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/guuyfhqjr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gllohunqj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gdjkyvula.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/grwwetzhb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/ghoqldhqz.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gxlfdewsc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/ghlwapsat.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gvtluqkbc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gyekbbqzv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gbwvdudxi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gwuiawthg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gqjjleiao.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/ghzfbuvkz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gclvmuopp.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/groaeinwi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gixzzmyql.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gvbctsfes.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gnztrfvgg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/goftjzvrl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gbzfliwzx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gucahaygq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gehgqsdcv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gdtwomnvg.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gwgcmemon.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/guqyaeieg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gkccjjjgo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/ghyvvximq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gholldrat.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gmdpmkrid.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gnmpjctbm.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gxqykursq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gheenvzpf.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gvgipawpm.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gzltxvcfq.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gqdtptspp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gowpzpalg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggnhhskfa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gbtrnmtyx.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gqorcepal.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtsyyeimm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/giehkxkey.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gztwjvhuc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/ghuuyqrxu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gvbhwrxrm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/glfxmshrn.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gddaebfjy.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/givhisnhm.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/guvguvxtr.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gwhifrxmc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gitkmzqws.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/ghygxogmi.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnitbdosl.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gyiqbqtda.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdwuvuwjq.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqryxewdq.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gilzmmahi.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwlnyxpgi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gbsdsohuf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpguzinqp.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gmexejdvo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnflfpsen.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gkgnhkncb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ggozvfznc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gchiietag.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gvebohjhr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gstycahcw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ggqcdjylx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/goprikssc.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gwrvvewqx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gsrrretmo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gisrsclvq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjrdfzl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gerznmgwf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/ggrviazem.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gehcqvcmy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gezodoann.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/glokhrdgw.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gavwiqjry.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gvvvlitev.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gysaggbwx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gxcandpni.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gbnjmxlsq.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gjfahzcih.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gwgoovrie.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/guafbjbwl.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/glzwzvqra.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gnoruulcc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gsdmapnkq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gvchezdoq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gjjrvrtmd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/ghlgbtudd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gbutewbhu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gtudrdsuy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gtkzbkehm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gbrusafcz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmasybsrm.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gmtduhpxx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gygmgbqax.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/girqgunfm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gwwkvbhuv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gudqizoul.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gxrcvrymc.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/glzyxdmmv.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/guedocmwt.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gmelfapbi.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gwlmfhsnn.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gowvyctao.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gsluiksnq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gsmzifvrg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gjvcmpesc.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gywxccyee.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gkrozklaw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/ghkenbuqs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gugphtmmp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gxxppczpo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gjdsxouto.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gnlvxxnkt.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gfdbxtxmq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gubezwhng.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gfhzzbabq.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gxjsagupl.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gylmorthk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gqutfcvma.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gfcbuckcr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gnkusxvnn.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gadfguxkk.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/ghlsujrgj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gtwklqwrp.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gilqbxspk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gplzgdcdi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gejbhlhzd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gbqtflpyv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/ghdlfbpbg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gehlhpqkv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/grwgybqwk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gzvbcalai.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gdpushjor.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gyjpluiqy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrzflxmr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gpqaodeev.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/ggcfwfgfx.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gfueftbug.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gbklxiakh.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gxynsqqqs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/glrbxtnub.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/goitizezo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gnhoinycn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gueugzouc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gfvxfotuz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gitgrfdor.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gonplbytf.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gtapjgcnp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyshgmsig.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gorvcrqoa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmgitzows.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gvprgelcd.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gffitizky.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gmvahdsep.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gjjinkqze.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjxarjetd.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gakbwrxyl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gqrwdkaaj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/guggxxdgt.sHtML


<!-- 参考信息 -->