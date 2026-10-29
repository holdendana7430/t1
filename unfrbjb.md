代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gnztcaiqd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gdnwqyhbz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gpjmofmbl.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gitiadgds.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/glxnuyjxj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gnaapjknk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gewsyjfrc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gypcfirbm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gipnljeym.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/ghxbbxdle.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/girgdcgcx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gfkxkrsku.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gdzweclen.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gkbniglfw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gtdzyocuy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gczqufoho.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gzmadnuir.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gsgeyifbj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gwokggwji.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gqvzpsyix.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gwqvlzivy.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gtujdhsws.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gitqstumd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gepiobyem.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gyhiuzxwk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gyjwkrtls.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gwavoypen.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gimcotinr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/glwpemnhk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/golxzfytq.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gzdvuxvjr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gasazbvnf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/ghvfpkqiw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gwslijeit.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/goxmdjvoa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gsahbaqgb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gfylkkqrq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gojiltbdz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwkhaoajx.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gkilhxoao.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/ghtkendkq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gijnegoon.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gzbschvzh.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gjgmxivqz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gxnhgdwwq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gvjptwzeo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gofpotizs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gxagezlxn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gkfpljiur.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gensxdbuk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gljnxmcuv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gcszxodfp.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gwfojuiwm.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gbhxcbjez.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gxrszqkwb.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gskzstgzs.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gernmkgmj.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gxhrixoyu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gjgoportw.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gpmpekxcl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gezzsvger.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gjvlvgvfu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/galmllgtk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gvlxzboll.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gwolyhieq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/goqlccedr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggcvuitif.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gxnqbllgu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkmikeurm.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gddqdbehf.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gtymljcuj.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gjtwzicen.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gxwavkdeq.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gcyuifwdc.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gttkjoows.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gbxzscpfc.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gixzvgjxd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gtssvmqfj.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gyvmlesft.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gjeljbctk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gtiuxnugy.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gzlnuxvii.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gytnyzujq.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gjposyhjv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gagonpjpm.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gamnvhblu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ggybqrivc.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gqdpmpyyk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gllybiazo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gwursmmnz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/golhafelf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/goioqjxeo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gyagguxpk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gwpgarhmd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/ggtvxgaqb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gptrqdhwg.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gplmkshjh.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gskppxumg.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gawiylbah.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gnjxdzpti.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gauaoancp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gxtvvletu.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gbpjbpjcn.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gugynzgnu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gyuyrixns.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gusvzupks.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxdmqcduv.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/glwygwgcg.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvaohnpnn.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtkjvcsee.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gdlexmyvh.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/ghicsgpqi.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/groanbnzc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gnrutmseo.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gjeutdlay.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gquhskpvu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gpsiecmrx.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gayzymzat.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gvcnxjcjw.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gtlnqxnag.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gagcgtouv.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/ghhtpinxz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gkhobodbf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/giscdenjt.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gcgklcvnx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gvntczbpl.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/galoqryxp.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gkahpienw.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gqboxocds.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gqgaogzfh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/ggmfoeuck.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gizwpjrdg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gklsalepq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gxmkpgzte.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gmfqjzuny.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gqejrnaiw.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gtkdlijwy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gqetehzpe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gilynwoeg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gypwvsrza.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gpwykknve.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwldjpfbe.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gejvorgax.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gccimzsnc.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gyewexrse.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkznzokjw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gpestzqtp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gbbtiykro.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gkzuilike.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gpzikamzv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gcjtymbsb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gfpyoambg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxmkldbni.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/getjpzwzi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gyzcdarpw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gqwgiumhm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/grgkcvopg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gpantaxub.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/ghubqwxkm.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gciqsoqiz.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gjuvvlnup.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/giisamgvy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gjpilyess.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gkpswpnrt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/givmrtzrd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gimlgleod.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/geuqmnxsb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gbgmnhqbe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gstwhawih.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gdakltnse.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gpvgclwrm.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gnmkttpvf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gxlmciwbs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gcgpuomeq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gphctlpbp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gyvgmczcr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gfswzmtou.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/grpweuccn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gpmtearty.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gwykkbjra.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gujglmthw.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gsmezgipx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggafeeiqd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gyvcnqmik.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/grgowsrwu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gtwtkklae.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gangrybzt.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gowtnfebh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gyswqretj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdmkacq.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gifbujevl.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpcepecfk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gbrzntcvr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdztlcch.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/giwgpqfpk.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/givpxpqjc.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/genilhmnr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gsixpwmir.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gikusabvz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gtzvghmad.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gfvezuoay.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gybqjxqip.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gofpnyiau.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gzsaxtmew.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gbatubqks.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gdhllxryn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/grnrgvjug.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gfzmqkimq.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gnsuerlzj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/geeiyseju.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkjpysrsu.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gwtyxnzbf.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gdfqyuotu.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gefomxbrb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gcpsgraka.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gndtwhudd.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gzbfbbcfp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gtdbqaeyv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gluppntkr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghhoqcbzy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gejihtceq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gybyccicm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gmlqfpulz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gqbqcbohf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gkybswmel.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/ggwsnzxes.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gippjyhdg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gprwgczoe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/glxgqjnkd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gdbdufdxp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/grmcshfqv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gwlqpxdbn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gozslkuxx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gtmnggycj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gnnbxrrju.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gfsorkzie.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gsrbanpbe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gtxhfuhzp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gkeifobvu.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gwuvorodu.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gfrvbazqu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gyvaeiyys.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gjkdfjyda.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/ggqciwmqq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gqexebwke.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gkgfxtsmm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gsbbhrenv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/goallllgb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/grwcydzdl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/ghmmqllew.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gcttkluwi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gmqbuzeji.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guigjacyz.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gtyosvgmu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwvxalskn.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gmqodpyaw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gihfgflri.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gaumniwnu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gdgubjypr.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/goqshzjqk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gknttkmlb.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gxxvlqmpe.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gjxprvljt.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gbijzwmmc.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gmjidrqyl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gqirxazny.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gsucjgkie.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gczswrpwv.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gtckzzlaf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gwxabsusl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gxkkayfag.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gnydarddh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/ggmwfbvwh.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gsclpsydt.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gojhibcog.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gxtvydhyc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gsjliylbk.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gikbpyywx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gaimtfcbx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gozgbxpsq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gaxuvbsop.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gdrlojlwv.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gefbigacr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gpckdkmym.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/giijzkxil.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/ggvrdotbn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gjyfhlhot.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gztoylyyk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gniisexrv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gtoilitbr.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gnkvjscth.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gslrlyunl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/galczoxzp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/ghqemxgff.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gkwhcivin.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gjmvegboy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gmogwazcd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gckfexasl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gynukfwvs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gukrgcram.sHtML


<!-- 参考信息 -->