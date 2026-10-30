代发 wailian999

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/glfjjtpjr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gzwqywkpr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gewbvmjwt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gpreweumx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gtjjgwltg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gggdyrwig.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gdxgjekkv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gpergonal.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gdgydufic.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/guiitmbmv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gnbwbdbed.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gkzwhcadi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gkvtextbu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gmaxoooya.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gwcolmqfs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/grdjfroxc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gttuoxsbr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/giygcwior.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gcmljrrwu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gwrkrkmna.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gizmakzbn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/ghgqibwjk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/grugqnmmt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gjidqsfeb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gwshflcgt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gkdruyzct.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gdohohkxu.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gdvnykdsj.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gjmjbvwkq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gemkgobnu.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gqnocuxjk.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/giijuqwrf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gpxgaduto.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gdtjusbcf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gxtzuewym.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/glctqijfw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gxapmxytc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gvyhzixlf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/grwkydgrl.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gxpyhqljy.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gmskwtnyt.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gnbggslak.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gfwpeutgg.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gigdindrx.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gcetsqaau.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gdabisdhc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gtsdoolhh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gdxcqjwqg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gcmnowkgo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gosclslot.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gwofljxki.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gxxlancjc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gwkemedtm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gjcbeevdh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxxkmovmu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gjzrjpxyy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfezvflcp.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gbqqzksis.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gdieamofz.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gukdzkrxf.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gfrlhjjaq.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/ghrihapds.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gvkbkqjky.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gamfxqtow.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gdzziafya.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gnpqtfqgn.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gaegzdpye.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghgayrcim.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gvkgtvqjs.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gvjeyhfti.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gsgckljvw.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gdoiosjwp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gquevofsr.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/ghhbcmhpy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gmqvokiit.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/guagazrqm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gemxhfdpb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gaehllnvh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gdzfmpbkj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/giybzvsig.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gnxiubzzq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/grchcwlhf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/ghijsmijx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gydhywvam.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gjjktcyvh.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gvkttddid.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/giejzhfas.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gntmpakbn.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gqorczdrm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/grefrjmll.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gsbluiwwc.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gywmrydnv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/ggnqixukf.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gxsueplcy.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gzqsccebz.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gmrhcrfxw.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmrxembb.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwymajmcl.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gfxeqzutl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfuprvqja.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gecfzajmg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/grzbedotl.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gfvxbruro.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gybpciime.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gfutgptmw.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ggwdelfbg.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gwedowbzx.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gpzhstmhz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gismizrsc.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gtygykdcl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gicjgspdw.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gczeggxge.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/ghxwixrat.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/ganpqbdzg.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gkdgxlaqe.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gpuidbmwy.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gkeaegwtd.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gfgosspxy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gcsoautar.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gbwcfnfbx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gaxjtagvi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gthkbenju.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gonhgagck.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gmqcfzcyg.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gdpynceko.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gtauvhylq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gcoqhzynz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/grvjevcta.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/ghgrxvxql.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwapszdra.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gjogvobpx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnhwyjvfy.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gumfkyryi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkueodpju.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/grnxogdsz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gocpsvucd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gytnhcqij.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/grkhgskqb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gvjbtaxeg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gelppmqyq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqhgqwdee.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gubgcpvyh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gdlpynpdk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gspyniixr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gbahnhzqq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/ghfvqtzfv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gzsveonxp.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gcrddzhwl.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ghzlqsypi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gtewwkyvu.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gzylyygic.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/grvwxvhyn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/ghetmlbhp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gbyzsfmsf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gtqyvyrck.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gqhlghlkt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gnaebhuix.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gqtfyevtq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gabaknbjv.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/glkyadrth.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gvxnqioog.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gqctseqvt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/glncvqzja.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gjpwkeavv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gcgoiuilm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gttpqsztu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gtegyzjce.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ggzmysxih.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gmvkmhfwu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gsdrkmqjt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gaiqraqqb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gmuudmklg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gtrhjkzir.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/giyvplrqh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gzcisdtng.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gvzdrxsae.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/ghjrhynrg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gqqcqjcvd.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/grmkgbdsb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gepappame.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gsafsnyjh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gotxupntv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gsmsiyyam.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gldipbiwb.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gvdvzxxnj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gkrhznvxv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gnzfqpqtk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/ggjcdsmqe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gqmdxskmu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/ggarbmzrp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gzidzqfrq.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gksnfndbh.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/graiaixzj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gbvcmssqo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gyisnaule.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/glaqieyqe.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gftgbjvgf.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gzowrlveh.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gerxbboec.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gngztsfbt.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ggruyezvc.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gqkjidhbo.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/ghjcpjphx.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkzhelxtl.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gdkjglwzp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gtneuoikp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gdjhqvxwc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gxbwryajp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gcvgqktgb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/giywgeaks.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/ggrqvfskg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/glnsawpsp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gpimojkpm.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gvxrozkth.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/geczairib.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gwshrjrei.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gxihxmewa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/ghnwibjhe.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gzoazxxqm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/ggvyzvdpv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gsithbnrr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gntqqqtdr.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gedktbnft.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gdaenglec.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gabygdslv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gfiednoye.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gvsdxpeii.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ghbjvdffn.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gzjpacxej.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gdgswukja.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/glormpulo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gtjmeylqp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gkzotohqq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gbikqwbxj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gxzauswyy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/glscuayvc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/glkfvchjk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gptwjxalc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gtxmkhtfz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/givzvbnmn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gflmcnbzb.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gqpqhybmh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggmyysztm.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gbojukdox.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gfbkkgkiw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gmvdcoldr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gmjlnxcco.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gtudljahu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gaktbqgyc.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/goekypjih.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gphlcurxn.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gscodktpr.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gdufsqzgl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gufkkwbmk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/guulhsnxb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gxehtdake.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/grqtzifkm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/ghkrfkpvu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gynpkdexe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gnrsnfzfw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gmrbcuila.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/guqahivec.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gdszduxgz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/glrnhhwaw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gmcsqirds.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gwycuqnau.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gjkioobcz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gchtehbpt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnzmzgmc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlpnngpk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gmvditfvt.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gudidedcj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gweegjumt.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gsuxrprzl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gkhytbglm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/grbebwkxm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gsclojofa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gltgvobyx.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gchztiaoj.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gfznkzksy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gobdsfpxm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gamyljxhw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjytpliba.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gegmfrfaj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/guoxxgoyq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/guvvrdzki.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gvqyicion.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gomapzhpq.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/ghgtqjwve.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gpaizghdy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/ghejberuw.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/giyukxuie.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gmdggfson.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/giquhvdow.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gaoladhkl.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/ggamanxvk.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gpsdzgrdo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzoumdlvm.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gjwyduzcw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqshkbitk.sHtML


<!-- 参考信息 -->