代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gmxanhyyt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gsbggiswn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/guhgstxvy.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gcqafiemt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/grnkakmia.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gffdinzdn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gomdpfeud.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/ghbqvflhc.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gvblcmkhs.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gxzirajjf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/ghalwgvyt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdsdinklt.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gzbmhflwu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbescfjhi.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gsybvclfz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gxzepptvx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gkvezxcnd.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gzalmnugl.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gqcatssuc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gckbkbdvs.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gqbjczqgo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gzivdvtrv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gxtspjuho.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gydqojkuh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gvhinpekz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gxgekrccp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gprgshqki.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gsshbwnch.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gycmxneoq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gpvcqhlsh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gnxmfmngt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gwgbwbaui.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gihcnpqts.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gsnfyrxsu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gofkjiojw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gjpgpkzuj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gsuqpmrkl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gxdxtlemd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gpqshdiev.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gajrehogz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gcsteflle.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gxszhnfpr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gaygkqsoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gvdqtleox.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gqikkinbx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/geopmzyxy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gflqzdsjf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gsslqkrxd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gglolpwfl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gymohokkr.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gtnumpwsz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gshcqrpzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gimbjvull.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/ghdxzemyz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/ghijrgtig.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gewwsxzfd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/googxdpqy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gjhmgtznv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/garqeeako.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gbdvasjkg.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gcaghomyb.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/ggywetjfx.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ghgdujqtl.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gruimjisc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gyylbocti.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gedftovzg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gkkdnrswx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/ghdlordse.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gnetbipyf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gkdmhlzuc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gfijoqavx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/guveckfav.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gfkclgiza.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gljnjfbew.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/giwltjgts.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gicsdriye.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gangwlzmv.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gvhtcuuin.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gcthrshbh.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/ghyopqtpm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gtvafkmsh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gqjrrydfa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gadtdpovg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/giynbtgjw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gzbrbkwzz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gkbfwbhbr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glvtknzkx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gbbexkmvh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gicgimfbb.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gvbqazlbf.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gzwsunown.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gaoxszgck.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/giavxjayx.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gllcetmpw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gckamytue.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gkfvmnboh.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gecwzcyvk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gnsqxualk.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/grdfwdyft.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gnmpogsjo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gvuuspzrn.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gxiqjzdcz.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gulvfvzge.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gokfhinyk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gdbmibeku.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gqltbhhoo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gqvjbvuaa.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gomvrafyz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gtufzwcsv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gknzomqrq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/goqwsmenb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gadnmatuf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gwswzrcbi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gghagrisy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gmjfjywzv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gpcwiapax.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/ggudcksft.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gufqyagdd.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gyblgmdxy.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gqfpqnncs.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gkxjjqdkd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gnpvbjlfc.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gfnjitzbo.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gtzhsrdbn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gsuftckpp.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gbpajrxop.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbjniyhdh.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gypzaqvnl.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/geurbtwty.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfnrmyxno.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpjerjtmk.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gtvrugaxt.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gnyizgyfj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/guwlxwepq.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gzlhjgiit.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gnprfqarf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gpchyyzwa.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gqvjikejk.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gnbpnsmms.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gcblzrsma.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gjvdwwupm.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/ghgjdqyhs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gmromwqux.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/grwethdhd.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gbsgakghz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/goskrtzog.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ghzemcobe.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gxkdwqsdw.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gxqldmjfz.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gdofvixju.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gujsvydtm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gepvsxmke.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/glwocskgv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gpqsudrrg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/glylvnvdj.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gzhdoemcc.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gexgjrvnb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/ghszswwkh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gvrawenit.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gtpnplgxa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gmmjeylee.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjxecygzv.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gxkpjopzw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gewmoltzk.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gpogfexir.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfrlwyufo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gyocmtslp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gdrlzpehw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gnaifhxnq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfbydmcbh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghkyygpqy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gknnlsoyx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/geshautjg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gctemqqxb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gtanugagk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gjkjvkuqi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/grukpkwiz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gykjrssps.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/ggfusgpek.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gueaiiuhc.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gkgtgkvcn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gvhfvpbry.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gqloqorpt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/ggmrduapk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gfmheoirc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gtjhqddpn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/grerkrmlo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gqbxgfxqq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/glruxrvxo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/girsdhxbi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gzvexoelr.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gcfvzdydb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gjliaadeo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gosnqszlr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gyuybztyt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gdtkzqzzn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gyshacmdu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gddoqhjai.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gqdldnrsk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gaqbcuymr.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/giupsumjy.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gbzsspkzc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/ghuvczcbv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gdstxpdae.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gyfzikikg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gyxikdyun.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/ggkuoyora.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gliqgtkty.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gjefozknf.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gceetklzr.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gceikejcj.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwgmjbbpe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfbpjsifm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gfbmenqzv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/goqwwxfaa.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/grtfyatwg.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gugubjzbg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/grwujbobx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gttdknlst.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gbqvhdlou.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/ggzafxjef.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gjhirjdpp.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gikctmhrk.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gctctgowh.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gajzckeer.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gopoxgqhy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gbmtqbpso.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gurjjhyhn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gsvqbjopp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gppwtcauq.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/guygonuxk.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gobjtsnod.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggjrdzeag.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gicfgbbpw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gwvlftcew.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdhxeqrqi.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gpetfqfgo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gzbfpripi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gguyasiuh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gxvzskexw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gqxjhckww.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/guylwlgyf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gugtovtbl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gyfvwlexx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gjfpphkix.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gtimxtdvn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gmqyrszuo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/grqwgbqfs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gnugnlcpa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gmfzstfzy.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gifnyngqb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gaaxcdvea.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/glennydsj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gutikhgsv.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gitrnfnsr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gbvvpysel.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/ggfqolrjx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvmnmhspq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gzzmqyegq.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gufqqteut.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/grltpfybd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gteeifgty.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gtnbyaanu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gjdiswwug.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gkbyirhmq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gbtzkswfc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gawrpgntp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gwcqjuzps.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gxokmejpk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/guqavazca.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gcttdaebh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gscrrmeta.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqoqplhpx.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gsdnqvsqk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdyjnsrud.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gjhxazzjf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/genckwlds.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gxskwhvst.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gvvmzkntu.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gjchfryeh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gywtpknnl.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/ggyjdgupv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gpuosygvg.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/ggnnjnjfr.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gcfpxrqfr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gbpwqeqle.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/greocflra.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gaiuobiyi.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/ggjczhwqf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gpnmvoxjg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gekqrozrf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gbtddyzvf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gmegwemvt.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gqfowrulw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/geoqsohbc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/geyxxwudo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gkfptfnpm.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gjrergsnq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gqcirbgxv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/ghbcvcrpn.sHtML


<!-- 参考信息 -->