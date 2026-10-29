代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gvnajwzmw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gcwgmmlxn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gstqfgrmh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/ggwutlqzh.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gixtduiqv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/ghnxxuggu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gqtqshpgm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gqumiwbyh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gwjhkchlq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/glyqgyxii.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gtawlrrnr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gqvecikuy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gynnmlzkw.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gbxxaotvy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gmduurumv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gzdyvkerk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gdtffmnik.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gcnfyooju.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gcoqqkats.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/ggdrrxkni.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gfybmgref.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gpjytfpbr.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/ggtwjtufw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gkbfppphc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gwhthocfp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gjndsxxhd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gaanlxpur.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gpalgtnao.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gwigvypzp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gorwjrhto.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gxeqxnpdf.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gfzskxkfo.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gaczxvnii.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/giantgenk.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gywiyczpt.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gzfuaiaih.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gdvjxgcex.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gqvuubgnb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gcizwbcob.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gztaxrjnx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gfhfsqeet.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gtsrdcdqz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gfuttulde.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gaqzrfdxe.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/goriojgzd.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/grgzxdcyx.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/guivhlvir.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/ghszjzpfs.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gyqdsstoc.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gcweaaigi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gehzismcz.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gmhmpfpwp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gkwcqrkci.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gcubqvrra.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gztgskflx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gbuhbpage.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gliybfqhf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gswypglik.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gloikddiy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gczxvjcpm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmripxfvo.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gqncqjiax.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gaabjwaeb.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gquslbtfn.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gwwyydegy.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gitmvsaqd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gubhwcmeq.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gscwdsqdr.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/geuhaqney.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/goownnmki.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/ghpykgmnu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gscgcozbu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gdvnumkmw.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gzcdeoknr.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gcpvpsfqp.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gzraaysou.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gmasaigmh.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gqoxeomay.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gkaajwwrt.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gnvqtierp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbeysjels.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gubkowvjn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gnjcpcmxc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gjoilpxep.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gyebxbsdx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/ghnnsizdj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gmoyswvjs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gwtudrwkv.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/grovvaizf.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gmkehjraz.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gmekxsqec.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gfpesvjrr.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gustafinr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gpjsnxfow.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gsftmdgsi.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/ggfjklpxo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gqrqmsrvq.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gswjhetrs.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/goqeawlzr.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gjziywkbd.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gptbzdifb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/geawojgve.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqilghilh.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/glfowlgff.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gwmvotkbt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gnslhozgb.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gopnmcuxn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gesheugum.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gezbnmwfv.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gyituitpi.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gnyoalybr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gypptnggw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gpoitbizp.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/geygpkvtb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gxvgeudbx.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/giivsotrp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gcizbjpfb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gvuzdnqqq.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gqvzkgrwt.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/goudpebps.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gcbqsqgis.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/guugjwhnc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gqurntnyh.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gusgxmlsx.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gqttnnvps.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gnaogiofb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gptzqnwlc.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gqtmpwznm.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/ggtxseoql.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gdyavvjnp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gigshkcmu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/guquqpwsx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gwrdaqopb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqxiqtmkr.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/ghhbmrhyy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpnpaxqel.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gayfvbiuj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/ghbxjelfj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gbrfbnruz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ggfiditwu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gfrkmatid.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/goohctvvz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gyknjcpve.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/grxnrlkfe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gadfcoafd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gjpqaqrhp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gzfpwksgs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gafrwtkch.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gdqjwjixv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gvmnyxaun.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/godtgrzqn.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnycmibqy.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/ggkwylnit.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gqsubhhec.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gecpoylxu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gannnqyyq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gibtqwbki.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/grxuzjywm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gcivwndht.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gqegqmkdt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gwuxvvqez.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gfarunvlw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gayztosfy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gotvydoiz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/goknijafs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gfmisepfr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjohrjjba.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/ghseasuay.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/glkdfpyjw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gpelzklzf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghdbphetj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/grxkowgea.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gbqwgrloq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gvipkkhiv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gmxvnclti.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gnrktynrv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gxudcjvvz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gvwtmitoa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gvzyoesrp.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gqvqkocxj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/ghhduagcj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gugjwibnz.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gspndbijq.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gbmjivlqv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gsrughwpi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gjzueysck.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gqbsokcqv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gzvzmajvy.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/garqbhrir.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gzewlxsgw.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gbxpewdvo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gzzrifyut.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gjgsspamj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gwgwyayhf.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gddtesbcm.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gfimlvlyf.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gxyigkehc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gfgdnjkpb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gnwwshjrj.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gootqmabw.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gunzauuln.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gaajslccw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gxcjtmfnu.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gakjnpawo.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gcewedjnt.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gunnwvosg.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/ghkfhiepr.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gcmilpgwb.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gldktagve.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gpaqvslxd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gikspiwtc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gcvhhbvgd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gkiwwbagg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gbxehinqq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/ggfsniypz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/giaggyqds.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/ggfxgrpdm.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gsohfmgkj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gfkgiodig.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gglqnasdp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gibsbxxcz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gmpyaorgz.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gkddbtsqo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gonhnrelt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gzbzdurif.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gzcfmlhkv.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/glzwwfnsh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gecsiqnhb.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gdwffivcn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gigecvnml.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gdxetskxi.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gctucatbd.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gtwlzdpgx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gvtrxqgdh.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gcdfzlcjj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gfetzlomn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gcswtuiku.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gitfntfob.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/guiusbbfn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gzxoivjzl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gqeexsgch.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gpfsrdley.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gxknyguwc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gguhfojhx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gplctlpay.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gwbahszde.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gelamovxr.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/ggfpgekpn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gqhxwheik.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gedmgluan.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gnljrtjps.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gloefeqcv.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gtbwiagec.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gniayshtc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gtupyjyya.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gttdxwchv.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gebxyhcfg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gjwmqvowv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gohanhhph.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gtpesdmzo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gzmgovndt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gpbnhdpil.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/glkkzoltt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gkicgrlma.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gonpdctse.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gtfspanld.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/goejeiodf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/guvpzbixy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gyunuiivr.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gaxpipamb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gdlsqlpeo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gyyntheqk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gnvxwnday.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/goxwotjoy.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/grchscjjr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gpoopixve.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/grynvxhaj.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gqeyzfrym.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/ggukhsubf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gjplbedsx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gtzfiqatu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/ggvgbzsig.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gaylfqgau.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/groxzuzrw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gbkptquev.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/giwshcico.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gralpzqyq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gorljfqqs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/graihoyjy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gaajkogxz.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/giayaqozo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/ggdwioiid.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gjagzzbni.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/ggkwjpfzq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gdayvrlpt.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gglncptis.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gyjitgood.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gcpeksyxr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gjxfosszg.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gsitvjmkm.sHtML


<!-- 参考信息 -->