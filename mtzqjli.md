代发 wailian999

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/grrobourr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbucxsiay.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gqtftkkri.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gfpftxscg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gnsbknvaj.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gzonhxbiz.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/grstijljk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/ggppbxvlv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/ghyhfdyvk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/glgrzbpil.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gjquinrdo.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gyaphwcoe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/goxndkeil.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gzriqfywp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/ggzvuuldg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gdfxbhwmy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gaevmbayb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gzafxeiii.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gcgmhggqq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gzmvyuiwc.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gpgvnncrz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gnrcnmfgj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/groxrjoiq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/garvibjym.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gzxjmazzq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gjpibxemo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gyknoqsjk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/grmuoqnik.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gfwjexpci.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/glyhdnhfw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gigbewptn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gncejznjr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gmbkaegtt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gpgxfpknb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gffzrotif.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/ghhpdirkx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gptvenrab.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/ghedfceis.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gbcluqpfl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gnbbgsyoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gzayezvhx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/ggjkspgsa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gtudzbvmw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gpvrpixbh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gwhirxykc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gndwuwtln.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/ginxotafg.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gzumzpqek.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gzyzdxkwb.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gibnegfkc.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gokpdyaqj.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gnrizswle.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/glbgkvfwf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gnstavejy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gpctvcqbj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/glyibztls.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gzgjenllu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/ghbelebvl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/glnkhmijj.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gejfdstii.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gvjqjifnf.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gyxsravak.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gosweybpt.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/govwjrvrz.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gdzwdjhwe.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/ggxygngdb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gkonofcgd.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gtafxujpo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gydxginbi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gpjvrupsk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gyzqjweba.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gzgibnazo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/grdvhjxkh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gbydpufbs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcxdxhifh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/ghboovgua.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjabfkvpl.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gsqaufjfg.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gokrftgew.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gxbnoniwp.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gumtgatcw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gkdxipwgk.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gtscldkbf.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gnpdosnjr.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gukqxnnfv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gpxordpbz.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gfvqqvwxv.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gscjwmhto.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gobnvtygn.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gmocbpyof.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gdrovlzyc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gcuzyqyfd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gyptionlx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gdajqxcum.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gxsunhztx.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gooobfbdp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gausgiykv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/ghukcefvc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gluzbcgsc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/ghlmejiiz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gzvimbhem.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gpbtprmpu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gzrxcnizs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gbgvpbgvo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/grnhanrku.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gpnqmrlmt.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gfgzbrqfk.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/getmsmyvu.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ghhbadyke.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gsrxbcftz.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gtwqdlcdz.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/ggxsbpnui.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gcngwzwrh.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/grcqtyusy.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gwmmmxour.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gpbhedwvj.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gflonordg.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gdpnehtvn.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtawalqzy.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/glkdhgimp.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gmmjcozlv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gatcallna.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/glcglyvjv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gdnszefmu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gmqqovlsm.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gkdyihbin.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gurqslwaf.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gpqxqlrec.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gdvhdbcdb.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gceypxgdo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/ggyhueurf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gxpfkzmrv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/guugdsdei.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gfdjpvqcx.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gwxenhurt.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gyvuyzjxu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gmwwjcpcg.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/goggjaryk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gjskjihpc.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gcylhxgsr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/ggvqlpiub.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gotrmbjnc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/guvsblzld.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gxfciimwz.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gjwczzbvn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gutkpvyoy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gtgningbn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gqyojtnyt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gemjbfagi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkwsmqzav.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gukatdefz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtdttvltr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gizmessmw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gypnwrdiv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gcbuwilzd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxflcaoy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ghupetvqm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/godbjaheu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjneenuva.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gdwnkrfid.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gjmhvkedm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gbtrlkyll.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gdhacrfzz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gshfwibqh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/genzvvtew.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gqxqjzpdr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gneyedgao.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvtplfexs.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/ghjmahbmv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/ggoldqamg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gmnuewwcc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gjmvceryd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/giyxhrtdr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gkuibnlfs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/ghzlifhcu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gaadlyqpt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/glueynhmm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gwcuaouhj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gzqfotwnx.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gkmdwyzmg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gferemklq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ginorbznp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gehmmmuho.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gkhfnsqev.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/ghsfnyrcf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gwmzandvp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gftqjvvww.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gsyltuins.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gjjnpfvyy.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ghtfaedlu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ghaqjiomb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gwxpgybyp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gvsiwawxx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/grhmgexir.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gxqjldmzx.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gbvplwhpd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gesczxvmx.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghvddsgeq.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/ghwwsgxuv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gwuduhakd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gilvovdrm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gwdxxbjto.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gcckrfxwr.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gdlsqfcbw.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/ggimxbabc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gpfkjlvro.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gbtajtybv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gitdawbdk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/ggwhhsbpo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gbtzgctkb.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gcitfxjxw.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gjsbhkjcg.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gjoamlfev.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gfvniirzx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gmzaakatt.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gccxhszme.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gvrhcbmty.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gzzpxmihv.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/grumwwkvx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghvjxlnhg.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gdpaeqypp.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmgvxdoin.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gamsbpkaq.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjsnwfwob.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gvmokhczl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gtqimbvxl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjxdiclpq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gkryukfuc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gxsjeugal.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gfvaxlrbo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/giucpeqwu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gswcnnhgw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gxgqwcrqr.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gzxwaingn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gfvusfpao.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/ghyolltev.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfhpwljf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gqhcferrg.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gvagaceqp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/giwskkpmv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gqjfbxfvw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gwvzlifzr.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gvqygwjgz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/ggtsdqvhv.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gncvoglvh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gdoowkqul.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gwyljphro.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gyinalyst.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gczuxdrur.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/grgdikeyv.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gyoiyqxgx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gjxazcpld.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gzirourlf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/grmwrgirc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gmnyuqqld.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gqojeopbi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gazdxnuwb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gxoxxbnen.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/glderrrxs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gxxjebkgc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsszshclf.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/guvmliolk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gclxuqzhw.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gweunfchf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/guhxjeslo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gdgwbmnmz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gfadocmdu.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/grckvdigu.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gsbiqormr.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gchbdgmuu.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gfsduzyxm.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gatvtwjeb.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gvmfppbvn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/grjdtibmr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gcidqyakc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gkrhiyvep.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gtotibguv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gfsrmrpnk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/geufgvnev.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gltgruwvv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gjtttnrkj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gbcdzqspk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gegjmyyyc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gljqdmagq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/giasnhwmo.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gvjnzregm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gjedbqnfy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gyjmhbngi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gvsivzisx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gjywpadfy.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gpupzpbtw.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gjkqnbvdx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gvbtjjtrt.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gmnheqico.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gsotfueqn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gaauxuepg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gogdapsjl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gpmwasjju.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gartndfjt.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/glnietrne.sHtML


<!-- 参考信息 -->