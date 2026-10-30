代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gitqaovvs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gnwtszctw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gpkksoetw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gjecfildt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gviygnytw.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gjvfiihmv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gugjtrzwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gtjqpwifz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gxexehtox.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gkswqdpjc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gmdyryylj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/ghsywrxne.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/grigyxtte.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gvkiyqiza.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gfzpfthet.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/ggpygfyxg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gspjpczad.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/getukkppm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gtizlhmyz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gnicvgveu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gqlqhjwgv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gnbqblcze.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gyhgumrom.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gupfjlfch.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gwwtpnjms.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gdscgvwpq.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gsykgyvyf.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gfuomcnpv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/ggrndhxxq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gxrfkimuf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gikqbkiqy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gagszpota.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gweqbtozq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/grpxwkxlx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/glmfudbqu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gzntqnrnv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gbqkyoxkh.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gjgbfotdx.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gprywhiri.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gihakvwph.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gypqszrwe.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gwgjpopee.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gbqcplrqz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gxhxpijat.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdepqgwfc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/glgbtzlmb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/guooqxyng.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gpmcpoirb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gsocihupw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gcvmpfbvc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gunashuij.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gzoqqhgmi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxtstvjld.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gtwarpwlh.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gudvybrem.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gwfudxvty.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gubajkude.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gwfzzqejt.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gyzgpczxy.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gncbtiplg.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gzwxzyauh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gyllnaczl.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gycqacwvr.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqaijgfpw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/grskwepas.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gclqrdlcv.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gbllemrnf.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gocbucgeb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gnmneqhog.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gkftfamdt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/goybxoktf.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/grefexnsm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/guajmpekl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gzeskxvwz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gauqybczj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gfbsuwndr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gxqmkvufr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/grmpjxfit.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gfirtfrdd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/garufjjif.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gjfokdrsg.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gqpbbfxsp.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gymuhstda.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gtucxrwrr.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gdmgtbhik.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gpwsifpmz.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gcdgrbkmj.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gexnrqmwp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gnieyrgcs.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gdrizsqtf.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtlhcsbni.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/grkfopebk.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/guyzcgtpp.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggrmcsvjv.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gzeqitord.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gdjxvoijz.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gpcxpirhi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/giqpjomwn.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gcmmrtgpo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gwtmjboln.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gefgjmehs.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gdalrsjke.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gpvrgkcdh.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gesvvmmfk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gpjdhivzv.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gdrntmqyb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/ganocwuos.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/ggzlpwwqq.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gsdwytcrn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gbjktkcyr.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gqnnooypo.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gprstbskx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzilrykf.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gadtplber.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gjbvyrkli.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gixchrrdl.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gecsgklxt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gnraitnbu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/ggfhdgjiw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gvrxxzmph.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gffrvcodb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/giztnqkyr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gatwgvbig.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gajonymyw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gxdbudlez.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkkzqzjtz.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gpvfzprsc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnhfuvewy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gmkicztpr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggtjrntjm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gryqqaerf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gfidpqnzf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gsplodwtv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjjdtorla.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfsxgaugc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/goilshgsy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqcvxttmm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gpvsdbsyn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gchpmxeke.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gzvzudvwg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gaueccccm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/glxwfvdcg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gdmeekobw.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjtlcegxo.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gkdrqdjna.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gjvhzqvjx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gilmvzysb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gjwkznjgg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gtdgdyqta.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gtalfloiv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gvgypaxbx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gvehaifgl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gbamjnkum.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/ggnpleudu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gnjjvxzgc.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gdfjnxeup.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gehaabhch.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gbcduntex.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gkqeuhdkm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gnnimptfv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gbxmtxfod.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gorpflrgt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/ghkpwotbt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gpmthathz.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gipzdcexx.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gjwhhrlha.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gpmbjojww.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gzyleybzo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gqypnwsyc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gvagiqrss.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gigjffnju.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gkxmkstai.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/geoctglbj.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gcyzxfzww.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gaoopwpme.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gclyzkolf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqstdonkh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gqvrwpppe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/ggyxvmiyf.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gqnqfjqya.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gtgdbuevj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gyyujwtrm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gfpflmivx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gpwqririd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gogpnnjjg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gwgomagzx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gtuhmikjo.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gdptghqqj.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gqtgbtgpk.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gbodkgqcx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gtebwyfaw.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gazrvueqe.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gtiejnocx.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/ggwcvrwed.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gytgddngi.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gesvzgoqy.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gtekhkayb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmeoksxuc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/guyoommoj.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmwjgjbho.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gujqiauje.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/giygbcwyg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gkgeyazxu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gbhbopnlh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gptylufri.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gatvgxfxi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gtwzamdjq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gbotrvhmc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gycvmqlek.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gkjwaudzy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gpxgahuxe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gzqfogmhe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/girjdkpcg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gqacbnyey.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gjmupdtuw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/ggomyfcol.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gwywcozkj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/guuffizdt.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gqryglkjz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gtfbjkcqo.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/glrwohsaq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gyummcadp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gosekbfqz.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gggdooufd.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gvdliqaxq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gnrpieprf.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ghrslpyqh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gkhlkyisn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gghfgbvrl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gsgbxwnsy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gdvfgilyi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gsifznrbp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/genltzwkh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/glnxoehdb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gssuhcibp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gstxurgcb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkmosnfzt.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gpprcjvtq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqmmmzuje.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/ggqdlzbeu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gtgkmyqit.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gfbqhwram.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gotvqdpkx.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gdtuybwfl.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gcxwhtaaw.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gamefzrju.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gdxdsigga.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/geyhebezp.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gsaqwmmzu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gtsturqhv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gelvyvroz.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gmwulciwb.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ggbiewhpt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gkfglbevv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gulhderhf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gpunqrujx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gsibvlnev.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gbytatsmm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/grkznhvyd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/guicbwhav.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/glpwsataw.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gdazoyvwe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gnexhrjbq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/giqekmnez.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/ggnpclugy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gnbbiquyd.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gpsatjzzw.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gqljiemka.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gnkscjpte.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gurollwrl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gettftama.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gimpgvkvf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gqkgoecwt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gnjepofzn.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gptnoglpi.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gsikmqleg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gxylpzvzr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gwyurssex.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gmxrevydk.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gmzpowbdn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gvcwgqiha.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gwnkzbvix.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gvxsibhcl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gsqaqyweo.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gctolzddl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gdddltzky.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/ghqyrndoy.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gkrkgwwdn.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/guatvtore.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/ghrbiunbk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gubhppvsk.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/ghtgsghyt.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gmgcdzbrt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gihvcypti.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/grggubqyx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfctkdlgc.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gcmhmfuqu.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gcwhlvlvg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gvogiplwx.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvntageys.sHtML


<!-- 参考信息 -->