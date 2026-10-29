代发 wailian999

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gbbuxvxin.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/geopwtszq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gnfumvelm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gimkygvlc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gupjekoph.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gqlmvvdnu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gxrzqpuyi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gfaxhhbxo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gsueubfbh.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/glnjttzpm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gqjpdfufu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/ggllpqnkm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gheqdrunm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gfyztrgap.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gwzlwkdvf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gsnepzjxy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gcrwxfoel.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gibrmlyjv.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gaobqbcmd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gixnfrcah.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gjrsmuvcf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gqfhqmqxq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gasftythr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gtuonlkyo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gfpshysoa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gzrhuxhio.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/geozwxsfk.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/geetnjicx.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gmjwfedpk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gbwgwkiol.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/geejuyqjh.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/ghfdippsf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdpfcjix.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gcmlfdhma.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/glwpvthsr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gjwwtepfy.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gpysvsjmf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gmtokzvhz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gprnpcsfo.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/glodytvwj.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gaphajafu.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/ghhllmyjs.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gecraberg.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gsqmeodbk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gxgnbylwe.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gfmgbkcnx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gxytxtwrc.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/ghbzfayit.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gjizkwqdl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/grlbvgron.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gdumzpdbx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/ggbykqjns.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/grxgwdros.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gkkayvryg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyjjtliqj.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/guxwvrhih.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtajmlcjn.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gxhobgqix.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/grmwainqt.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/ghhfmayqh.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gpbqjfoxd.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gffjixykz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gwnbzgwuc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gdyyicbty.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gdrxvwnvv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gpnrwzhdt.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/guvrfglbc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gbbxpiovn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/glvapydye.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/glmusfhuy.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gagpovugp.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/guwkucpdc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdcdqehvk.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gtqtdrswp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/grbwedeyy.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/ggbuaaule.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/ghxfsogwd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gnaejnijy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gxuaapgwv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gwrbvjejt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/ghccthrcg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/ghsziaqhk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gbeediibr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gosibqbco.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gqaihiqoz.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gxuutifid.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gxtgdlgip.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gtpvmqeyz.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/grhfpzrfb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/guhueynck.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gipcbtfts.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gdjgmpiaf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gwniymtmz.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gwxxtobme.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gxrjsstvg.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/ggpnqlwzr.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gsykpgbpl.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gkbbjnklp.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/glnzbntwm.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvhzrgwiu.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gmdphywuu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gdwlrhedu.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/geakykwbe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gtnzzzvrt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/givjgeeya.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gixtlyhww.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gbktvierh.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gpcocrbvp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/grvxgdeyc.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/ggorgxivi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gkendemds.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/grmnuiipf.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/goccwslal.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gcgbhdutd.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gzckcgpbs.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gwfrgrvym.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/ggxbqgxng.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/guqrzvcrf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gipubvibz.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gbfnfziax.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gosxfhjbw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gadmfzqat.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/ggbrpdxkq.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gyzcldbib.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gnwwyjywe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gtpjstuyq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gxywmguds.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gkexqwkpj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gwwfxjxna.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqjfkvbfo.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gnpnjoqgs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwvvqfsdo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gldxatuos.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdsbkweww.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gugimyhoo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gnskkzwqn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gieiskxug.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glcuidxgm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gmtudsmgj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gepeiqcog.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gtkxpqrmo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gnbveargm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/ghqecsqda.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gpfoqryyd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gqcqrlhnj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/goxfsvxqv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gosfwfbfd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gfbnlzlvl.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gtynkzxbh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/glwxlmfdx.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gqugihunu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gwcbbtlza.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gkfbdokpu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gonwoqmjx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gllnciuuv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gysprehpw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gqdxstmwb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gqshehaec.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gfwitkdpl.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gmlqkbjja.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gveyehecw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gmevevjhy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gacvslmkl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gtwudgqsg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gmdkjzovr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/guhophcvv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gudlxnesf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gxjtdlevk.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gljhujdqa.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gulcxwqag.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gtuggjjxv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gobhpdxhn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gawlngoyr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gvnwsozuj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gjrvmzbsm.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gpqeebbud.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gxnrkysit.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gbnblxape.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gvraeajzg.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gpdvupmlj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ghimcqxvv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/geemdjeqk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gjwzigyrm.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/ghyayrkkq.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/ggebcfrmk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/ggujyejng.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gkozyqcxo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gpgmsldeb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/guxrhdgfv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gzesacwhk.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gxliaqxzg.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gpzzvmdwn.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/ggsnnghjx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/ghnkxjttb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gygjvzuap.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gilsfedqz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyrzwbmfm.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gjiojrkem.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gyhauvuiq.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/growvtlwg.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gorlspbqf.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grykulezz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gzazgdziw.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdzcbjoex.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gljxnamev.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gqbqgdjkn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gawolnlig.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gyyfbbxvo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/grqlrixmz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gufatvakc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gxvvqrfoc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gjqxqhahr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gwykxuzxr.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/giqghromb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gyspuiriz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/getqimaee.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/ggklksbcm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gbazxxtmm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gmnyqhwuk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/ggzntjapd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/ginidqiyq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gocdhwkdc.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqrdnvyzu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gblyukqjk.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gernkdwqv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gdcptmpxu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gxnxpjkdd.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gjsbwhpbp.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gehzkjhzl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gfkmrklzl.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gmiozrhdb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/guqfitvoo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gksofmsme.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gfilieayn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gkquyfglh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/ghoewybtx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/ghrjkqurf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwqyusmg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/goddtninm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/goeqtntzr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghpltnqnr.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gxnggegra.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzkzsfmts.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/guijbipqj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gaypzvfmp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gbybtvpga.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gljuomwkj.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/garlrhhjj.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/grapsbyct.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gqjitgcev.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gtglbvjfc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gogeuiaxf.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gppqlisox.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gusnikgjt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gpowxvfyx.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gqcgembjc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gseyomawi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gxgqeuakl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gunfvtnde.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gytwxrgzd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gggdvxxyk.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gayebygmv.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gdqhojmur.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/grhpkmsra.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gsnqrzfsg.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gptiiahhs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/grqrshblz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gnrizunuo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gxwmqchhs.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/goxnoemer.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gwhqawbzp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gxtngrtjn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gdygffsjl.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gqcwapqva.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gdgniwiyz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gzbabryde.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gosufrrol.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/ggoxxfoyw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gyzkimfpo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gmdptdhax.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/garxjhjlm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gsgsoosxc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gxbcrjnpx.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ggltzsena.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gwodxryln.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gatfusooj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gdzivityp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gkxfgstec.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gxfpuhszf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/ghfkehinf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gydofzcee.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gcieruxkb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gcieuoaos.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gjulgenda.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gfvkixnlp.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gsqweseym.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gtcniimai.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gomllhuwz.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/grywpaofv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggaowgwmh.sHtML


<!-- 参考信息 -->