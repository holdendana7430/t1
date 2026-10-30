代发 wailian999

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gkgmwjhqn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gzsuwilnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gbjuytvjq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gqnmiueul.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gstabiwts.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gwflnfxfa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gcwtdklmb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gsxjxwpij.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gakrhugid.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/grnwwmxji.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gmikedzhy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gcsqcxtct.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/glvyixysl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gyyrctjvk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/ggzysuqqg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gokkoscmm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/ghsphwnah.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gpreolepd.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/ggdvpljzq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gjuiwazov.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gfotnagls.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gtlxcaakk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/ggkmarxsj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gmjfmdhrk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gdxorjgyx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gzzqmcwza.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcmlkcwjw.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gmcaepfzf.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/glboosgde.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gwnbwwjxf.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gnrpmrezq.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gobxobveh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gigbmkkxn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gprtbuape.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/ggktrybck.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gevwqbtxb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/ghfodlzvc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/ggqguperp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gpitrprew.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gbgaoeaft.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gicmhiqqw.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gahsxyihz.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gbrxvdohf.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gzwdpkdbv.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gdkxcabts.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gfrnjihcr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gjomsyzed.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gtvhvlbno.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gbjzmhldx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gzhwyjenz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gtxcpuirh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gapqiziyq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gluhdgbeg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gwwmnpyob.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmskrbrbf.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gnjrjvezs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkgkmfhzo.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghkipirbo.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gbwwhlxuw.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gxzddynpx.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gpzcnwhkj.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/ggvekfddo.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gzdyomfpx.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/ghdwtursv.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gqbizlppg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gzgnfzipy.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gghjzavsn.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gahtjwhss.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gtafczwbv.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ggequmnlq.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gqufnfyks.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gmbtywtgg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gzeyqbucs.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gglupwfjz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gfghzqrsy.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gqknblitr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdlsirdwq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gbevuadpf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gxiataodm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/guxrgbmrl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/glngknlnz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gqgoshdsb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/grkwmbrwq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/ggmomnvag.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gtbawxlup.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gkkqbtbkn.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/grsgkwrck.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gexcfdhrh.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gggowdjzs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfxnutp.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gipvddziw.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gxwmfyvfw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gqcccyjyc.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/ggbdaecrs.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/grzehbwal.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/ginfjnetu.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ggufaeoik.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gcrzksloz.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gjfzyyvhu.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwzofxpea.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/goxinfspn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gpebvcdks.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gmyxhlrni.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gddsfntfl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/geztsdjid.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/goczeymmi.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/ghjarnpiu.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/geefgpowe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/grvrfftjo.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gzkkorere.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gxdkbnabn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/grjtllthu.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/grnhnoggk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gnyxwvwkj.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gfphsxegi.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/ghfdmyvok.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gyaxgtjly.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gkpjjtxli.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gspcupfnn.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gdsqmxact.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gfpwwnrrw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gcezjctnd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gyooytipm.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gxxezfteh.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gugisglod.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/glbpvgjgk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gggvmneky.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gpybilxuh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gculgkefm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvaicbinf.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gzextyuqj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guoslkmsl.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gfhlafgbr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glcutshce.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gxlzbnszu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gfilxpnnb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/grivngsuh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbbvzbbal.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/giiiuqlew.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/glohduzyx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnkjoark.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gvgnzhhru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gfocjdrve.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gannucyex.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/glvemnzig.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gfxnicnlq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gvwzukozd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gwzqysnqg.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/guylbgipt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/guzhincrf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gfelnhybp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gppidzqsz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gokhveklx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gmqbpqysy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gmlwvqise.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/ghhinjvse.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gimoswjqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/ggdoeuctt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gitaanneu.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gdhwmrvtd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gbgjcixdp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gwjmozbii.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gtdqinwnc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gvcbpmkjg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gdnhhmpez.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gzdfazwaq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/ggrjyexlj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggjabprav.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gzxfdlbnf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyroretgp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gfecshalo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/giscrpepk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gbycahkni.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gweivzncr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/ggppzqbls.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gadtrijwh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gprppvtns.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gzdcmyhsa.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gntpvcufk.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/grdphmalk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gmruapmpy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gymkjvjrr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gytvrapdy.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gdyyrznrv.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gxjpggczd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/guuqpwdwj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gusnssfub.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/giinvehcz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gibctmhws.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/ggupaucnf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/glbcdctiz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/grpthjvfw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gsofsdnqg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gnuapjyqo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/ghoqvnjll.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gettxkodz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gizsefgug.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/grnuxkoan.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggufvzkfn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggpkdhpgm.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gcbnusjdb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/grfnfzoro.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gnljxtzpm.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmpllhact.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gjzletzmq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gfpwuxaxw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gqzwxjtvr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gznecszng.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gckgkoljm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gltthvboe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/ghmfewxhm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjtuxhjnj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gudhlskdc.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gcixvxaho.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gdmsymrzc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gdrqezeck.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gwsfupycc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gdmfpepaz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gnotuenad.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gmxlchmen.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gyudwlpaw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gefiamang.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/ggiytprgh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gsjlnzmyc.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gmcejzvsh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gacfribcr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gyqmfrzfx.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghlanaudb.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gtaseaszr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/goxdkrluc.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gmvbfrngt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gihrijnxc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gokimbzma.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gfjrvkdvk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gkurxvgyn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gligszxot.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/ghgjgooep.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gdlsrmriw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/geojclhuz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gorhnjnbx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gctcxizdm.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gtybirput.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmagkpyrc.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/ghyufnrjn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/ghdezuwlr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/goiyhuwqq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gsfgbqwiz.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gsyxkxfcd.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gytpnyisr.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/goqzjdyui.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gepddiqbe.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gqocnlzji.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/glxowiipe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/geelxnjpk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/goqqfevao.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/griyycebo.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gsdwswwzs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gvqlcthiq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gnmesuyfr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/glzpcjygo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gygvnrntj.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gjxfdxlyl.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/ghylpyuoe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/glcrkxuxn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gbzmtnkjn.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gqxkiiutc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gnpbklcax.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/grigoeirh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/ghnplcaez.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/glaevlzhj.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gxporfram.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gtogtymlg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/godrwuxtm.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gusvxhspn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gkvxbnnyj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gowespron.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gyqtrbkwp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gjslfujtm.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gynmktjrg.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gapagybnt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gaipecdne.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gqwzwiuck.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gxarqbzta.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwrvgsofw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gryfesean.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gmxogjwde.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gityxpdhw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gtgytrmke.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gxwxurkif.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gssvavlfn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gajzgvyou.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gnxgxuris.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gsxogwarx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gonwpvpup.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gobudgzza.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/grlvrrhfx.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gkvmrmcso.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsfbzuimo.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gpqhtratb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggqjfhets.sHtML


<!-- 参考信息 -->