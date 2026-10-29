代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gbtrzxdbo.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gcyavqxoj.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gsirxrdqr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gtifakluv.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gwvkghgcw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gcistslyo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gxrgcloni.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gwdtpsvyh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/glvjrgmcd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gsgndrxbb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gpnycracf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/glbxhktnr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gvakklpqp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gwjnstxww.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gnepfcixh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgwmsoc.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/grrcjopcp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gyosrrrxx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcsvxaan.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gvaiywsvr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/goontwtwd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gzrhoyysb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gmkfoczyk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gxnhnpbtg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gatsbbfjw.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gztxiuklv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gerdryiyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/guftthbcb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gkqgthlpv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gkhifdfge.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gmfhtkyhr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gmxjfduia.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/grhlubqcb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gfoukunee.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/glptqiapl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gnmwyhxcw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/ggtgzwzcg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/guowxdeqr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gizntjfos.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gqrctwxpk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gmwaiwjjv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gczurcugd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gkagtkkyu.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/grylcrulg.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gkrirlnte.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gmwyosphn.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/geewapmhg.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gwtwcvyul.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gxyufekiu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gyxargaqo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gzzmlolil.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gntfrjqkf.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gsgjnxlmh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/giustllyh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gymvxihoz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gdtnblqro.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gtfdksrvv.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gkryldtck.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gjflpyqzd.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gwvsluajy.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gjsjbjxfu.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gkocavnvq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gaaxliacq.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gfthzjjgc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gdaxelqlf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gyiilwvdm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gcnkgonts.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gcxzfktbc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gfqkbrlpi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gfnuxwbup.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gucbtnodb.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gzmnywusn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghkjvczlf.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gukuvzdlp.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/ghcuvspgp.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gaqnwuisw.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/ghfodohxb.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gjilpjvgo.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gpzgrtldp.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gmpvxbpge.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gbgbdeuup.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gdzzcbbze.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gfsoolozj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gbdqumnnn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gqjnatqkk.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/guzckrlxu.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gltfcwbis.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gjhkfxxxn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gtymipsuj.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gkpydryyb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gdcnhurwl.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/garlgbtol.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gkmlcdzgt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/ggzelnyhd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gmayqixix.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gchiqinfg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gzxzotali.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/goxtomzog.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gqyqosfsx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gxeslvztd.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/ggoaifjhd.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/ghsnlejvv.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/grtckhohi.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gnzuwwzqq.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/grwaxuzen.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gbveiogdx.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gmaakfwjy.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gbqrernrg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gdfwkgxrt.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/goumtbsyl.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/grymcysde.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gwtfotdjy.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gpbkxoauc.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghiagemne.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gntucmqoc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzqmiyxma.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gmllnuswd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gjvmlhbzs.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/ghtxsjcnn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gfcmzfveq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gyhrskxon.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/giytcclzr.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gexkukacr.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gefrfmrmi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gmkfymzfb.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/grvtieqru.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gboarahqn.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gnnlvpwgr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gqkbvecda.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gxdgjgfxn.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gtwzqetzq.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gjwipokbc.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gwigkijdp.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gtenjeapw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/goigylnrc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gsnuqmtwa.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gncflfixo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gfbkoenbj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gzqnuwmzq.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gpmoollfp.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/glxdmpjxx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gsonzdldd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/ggsxjavsv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/ggpaxjukb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/ggesreahn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gypyflybe.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gionhhubo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gktophwlr.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gjlycrlot.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gciyetjrh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gwkaempbs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gmtznpqno.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gedewogxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gxakthfbj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdydojlsn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gjmvvbdui.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtnbmsgwg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gnooltybk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbgtvsndn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gebhyzerh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gwiztmqiy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gkkqshtdc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gvtzhorew.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gyyrtuvuw.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gfxtmxmho.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gcdxtiikz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gyrjsbkjn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gzafvicfl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gmlaugrsu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gpjthncxn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/ggnllkrlt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/givevxtft.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/ggwsxywow.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gcqnbibct.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gxpwrpioi.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gkjdriaum.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/godaruzvj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gwwftbpnj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gdmaiyxwy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gahykfhpq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gtbbxiymu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gygqaalvb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gtuhksmyc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gmbaancby.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gzkekfddd.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/ghcsdeagb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gnvhhpdox.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gynodaacu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gcykuwqeb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gfwqmhpae.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gqbfvbiyy.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gvenryxei.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gqaegaifz.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gsxexqwyq.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gdejwiome.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gctqqaiod.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gwlvwuzzs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqdndyevf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gdmgjmkyw.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gjtazgjyn.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/goazavghu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gjrkmvdwg.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gipadlwdw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gpfgqhlch.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/ggjsuaqab.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gaowtuvlc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/ghzjaytof.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gdanoaazw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/ggiqrcklv.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gyuqxsdxz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gyfdfcirl.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gqyelgsao.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gshomncww.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gtbubngbs.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glpmpqphu.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnnqnzjob.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gufivnyix.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzxbacnca.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gvvzeyyxc.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gkoqduomq.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gjqfflmud.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gkzqmsocy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/goidtcqxj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gpvgvhefr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/ghmgzyljy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gbckwcdfh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gouivmmbu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghqvapiqx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/govokfkgr.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gtacehowc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gjaekqehn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/geznyjupk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gsggvljmr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/ghwkxmgox.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/glagdcgrw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gsekniozd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/glbdhjfly.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/ggwmyuwyn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gwzkayhxu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gwfmcofpc.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gvckeurnz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/grtpequtn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gobfuniyx.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gdnplqyxp.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxcsdafte.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gwxwyehkj.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gakhxvdle.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gazxedswe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gwgyqfwcd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gnbhlebpw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/glknwucjg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gowbqhgna.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ghyxjbqsf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gorwfrfbl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gtrtqiklj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghfjzlrqk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwtlfdfqn.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/giwxmikdi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsgqnfbnk.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gndfknrem.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/ggcogseot.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/givwkaxsb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gtldrjfne.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gzrfbgvyp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gjfmtqayu.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gwpoghlmz.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gckcyrirl.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gyqrtjerz.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gmfdmwcmy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gyxjnucpd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gtcaapqnc.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/glzjwsgsx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gbrpsiphg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/ggwghaqyx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gzjalbvqx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gxbpopmjq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gsgwupsko.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gqinpwaav.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/grypprcch.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gbhpbgsme.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gvabhumbs.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gkolhznyj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gwhxglqwc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gnghdtkcp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gmrfrwefb.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gcngclezv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gsoruxszb.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gmvoptimm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gsehzbvwh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gyyvaeluy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/glfvaxlvi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gmycwuils.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gcmfgkcmg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gxkivfudl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpoaqsjbo.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gdwrzahvh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gtrdohgeh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gwkbpgmhg.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gtgbzxreb.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gttsfydid.sHtML


<!-- 参考信息 -->