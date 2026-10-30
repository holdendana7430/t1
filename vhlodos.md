代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gfrfcstvl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gunodgzsb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gvsyabtht.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/ggqjfjgnd.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gapscjars.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gavwlltgv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gpcjtgoug.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/ggdfjxeql.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gtfmtodec.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gcpmvhqrq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gkxygdyek.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/ggrcqptef.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gtqregalo.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gibbjiuzu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gslyezlyj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gcijqkuvn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gljyifxfw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/ghvvxofgg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gjhqupahg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gfgzijrbg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gfzmexmnx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/girdnwred.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gzzrsofyo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/giklmuzji.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gjdkaujbu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gujqqiphs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gqjcyfskx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gunexdczg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gllufxsqa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gfdcjvzcs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbgfxhvpg.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/getwasgfx.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gognqhexc.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gybxmuxcu.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gcwubwrcy.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ginmlyvdz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gfnmkmkry.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gqlrkwyyy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gxntlltpu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gcgydkpzi.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gwaospruy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gnxrnhgrr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gebrkaxfi.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gvroyblew.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gnhheewbe.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/geuewhwrr.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gohwewjnk.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gbhpxpaif.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gasmyxlpx.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gtoxbvhsb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/glanieigl.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gazflsjrz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gchwbnboj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gtgqvnlfo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gzuppuyzq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gsvnlenvi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gvxxrngmn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/glfcyhcir.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpnnwegfi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gfwzuimcx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guyadcsvw.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gzhbyjbpa.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gebkkbmak.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gayznbvpl.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqkchvk.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/glzpidsfh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gbcmqzvpe.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gpnxcdeso.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gqyagarki.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/geypudtbs.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gjuaygrvd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/ggaqbvejm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gmgjzinkp.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gsspomdpa.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gcmlytdaz.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/goehvjdll.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gbsvkedgk.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gzxplbqko.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gzrahtspj.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/grdawrxdt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gaeavojwp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gpvnhhdoa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gindvmido.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gnnzzfuwk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gzmpvacvd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/grutbohbl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gwgvpcmfs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/glwryjubj.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/ghgenkljy.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gwypsfyey.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/geysoampv.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/globdkrtb.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gvlsbabsp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gwrdbdzay.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/ggaabmxqc.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gdofhaclo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gggpnthdg.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gxxiaoovg.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gakntwsfl.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gmbrguoua.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdjsdscyo.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/giztssoxg.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gveakjmao.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/glinfflqh.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/ghydfefla.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gbuysisqh.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gubgkfdnx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gztqkcygs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gmmxizlit.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gaotxwlkv.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ghfurkyyk.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gfsiwnssf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gzvbbufsu.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gzvsvcclg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/ghmuksbar.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/grrxjcvfc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gpgycdmvt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/grhekcsak.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/ggdwvuufx.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gkishlcgp.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gqvpnddfw.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/giqhgwjqb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gqbpqrlfr.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gikzetcku.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gxovzcizk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gjyybyslv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gekmordnh.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ggkicoijn.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/giilrntas.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gybywkdlj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gvnurhnef.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/glyyvbtwz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gdpzgqpga.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkcoskfvt.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/ggnclgtwq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghthudffi.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gasfqkaxn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gjdxxsbtr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gvordfbwg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gbhydpgtp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/grzkziaht.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gpayupetb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtzzqnykl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gqgwxwjnq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gbdacgcca.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gwhypvyiw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/glzkaxzis.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gkswimahh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gpkkyuvsp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gxsdlgpzl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/giybeiemy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gqgijvegm.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/glozibvuv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gnecotkub.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gutgdnvib.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gqvpcjfyl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/guafjggwg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gwqtchumk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gtpuudwof.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gvjubvfbc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gqpjlgzxy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gszokbyzg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gmciivvlt.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/glredanuw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/geaogjnty.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gzheiehwj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gfrgozqyr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/glkfzwknk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gvhzmlyfg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gxzcajtzf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gquayomgw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnlmeurj.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gctcanfzl.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwltldqaz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gyypzddrd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gfkktulau.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gprblyulu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gjqzonbzv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/guudznnqv.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsvfhdrow.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gpqbyyfln.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gdwvwgvly.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gsnzwgjrc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gwpokxlta.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/getjzsdic.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gbzjdssyb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gjztsvayl.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gxjknquew.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gwmwjrgdq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/grhinpmdl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gkwhkothg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gnlntmrpf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gzipwhord.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gzvrogebb.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gktfxinhw.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gejxgufdu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gsillvofa.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gvrqxjiez.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/ggwmyesip.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gblpnhzxv.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/grhdoxnzq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gdvhfbyol.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gonqmcbcm.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpetdhweu.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxcacqovz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gcotbdqui.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gctuoqvqo.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/giihogozb.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gllpgxfeu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gpkhchnnv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gahgcwhah.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghedocfon.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gcqnzfkhg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gndauetdp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gxuioqhuy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gbmbwoctx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gqjxblpyf.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gmjpddnww.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gufjqnzns.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gtalblsuj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gygnbckvp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/grkgyzhdm.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gpsdvlied.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gagrxrsyq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gbfuqfqmr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gaobpmzln.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/ggxsznvbs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/goeacqodc.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gafthptou.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/ggrzhwxsb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gpotntvcx.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/ghybgsynh.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gikwpjsfq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gmmmklpge.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gcccetqfc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gwndaogcu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gbaapflld.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gzmzjwqqj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gatyfgsaj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gijpexzly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gifthfqee.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gijdyruel.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gvbwtdfwv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gjddmisfg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdspkgdvr.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gkrfymisu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmgjfskex.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/ggiigfhhq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/ggipjwvkr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gijetkzyr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gygxjjcmm.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ghytlrqtt.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gfbtsujsb.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gbwqjxljk.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/glckptakv.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gvyrimhvt.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gonydeecc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/grxewyuwn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gmcpatoba.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gfewvspfr.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gehdjwtzp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gfwysfydg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gdwpllhkg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gxnzvoivt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gynqesvws.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gykclwijx.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gxjoivmds.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gwlvzultq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gadyukagj.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gnuvvhmlz.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gjdnhqvop.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gdrrbwaer.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/ghzatnvnb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/glzssegfc.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gflpolnpe.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gjmoagcfj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gflhwkcia.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gmuctnntf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gkwjztfxv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gqdsdwctr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gzzcdpzdf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gixzcpbxb.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/ggcmsbetj.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gplhgnzyd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gxhadhdxt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gzjpbqpqh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gkgeznavr.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gjmosxlml.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gvecuxvhb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gmkldybap.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gstchuaqe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/grnxzikco.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gwpuvselq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/grwxakvdq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gdaxvjqca.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gvgmcfmfb.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gidtpdvcc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gcijhwgqs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gruwrtvdx.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gpyuzvzfp.sHtML


<!-- 参考信息 -->