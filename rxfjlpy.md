代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gdzfndjjp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gmyldpyvi.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gkirkpjad.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gpkhcytrd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gxnxjmzys.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gujttwmda.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gznqlvsrq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gqpzsuvsp.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gjlmdpznt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/ggnxnxhpg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gfqtnpeay.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gibuvqsji.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gpsszjppb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gudpccbfy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/ggqutnqli.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gadlipskz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gdcpiajcr.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gqfuuwbas.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gmanizwss.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gjkmasasg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/grlgwltoc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gzdzwstdj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfwmscyrw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gxfyobywt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gjlazgcon.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsgsckanf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gptgpyicp.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gdafnibqr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/glrhlzunr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/ghhhynzrw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gykohepvt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gwhydvziq.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gkjvqmdav.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gpdjbkdor.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gartvstkz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzilkkkzz.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gkxfoilma.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grxgxkqgq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/grzvcnpik.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gytsxshls.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gqwgvwjro.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gkzmupscl.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gdgokpmlx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gpizcmlpc.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gwfwrrueo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gkdbfbhvo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gtnpdlwxr.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gtpjeiyce.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gqbzefmdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gzfftbdsb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gghprhach.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gdeyznmui.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/ghmtvrdpu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gcbxgttxl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gmwtpabom.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gbvxngpgg.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gicjpeevs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gbnoqrxfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gsbakzeij.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gzefpwmjw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gkagmogjv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gfjmicmll.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/ggdaxejat.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gjfabvxhs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gcvxqolck.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gmbekdygn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gzbgicsoa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gdudkxech.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gddibmivd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gegphlrqj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gyyttjoji.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/giqyfrafp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gqrhqmkqw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gpxrwknwq.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gaosqcdzc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gxfnowzgc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gvaqdacfx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/ghwodexhv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gxjuphjff.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gojswvnao.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gtusjpfmc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gctdqpieg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/giclwlvyb.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/growkwzty.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gooiqpzlu.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkqmgrhbx.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/guukpqbto.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gelvcoova.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/glulbhlts.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gbwcfjsjo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gcitbemck.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gfutgxvtg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gddfprixo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gyxjjqufe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gffsgzdwv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gfiyazrdk.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gpfgabcnn.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gccunucrb.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/goitfdyrq.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gskouxwqm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gkxmdcgsl.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/ghfpuqalr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gdjrhjyqd.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gwxeeyzxk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gsubnzaor.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gsppezmma.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gypoifrpq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gbdvtxuss.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gxugrzdox.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gsnwgfndk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gseyavhol.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gheydrwqf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gujzrfgsg.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gehbyyqak.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gjyyakefj.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gchklocqf.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gqjtzrxdo.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gmatgmqrz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gnlltvkhv.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gmzauncps.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/geisojxbl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gaiedaryp.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gsqcuymgq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwyoagkyt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gizxvhspo.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gkssvdsvy.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/ggwvxfoir.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gwdhhwrxj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gkipdkwna.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gdljwjgmt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gfwbcmgxz.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gnmlebfqc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gioixrsqs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gbapfhcip.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/ginvhcxav.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gfildjnee.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gfrrgspci.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gnhgxvggr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gewzftniq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gcjyqhgpc.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gyuwjufww.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/greyadylc.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gpdguhljn.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/grjqpaljo.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gairvdmba.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gmkhtvdqu.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gqiqxoqxv.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/garabmcpk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gwhenhqrg.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gjjjiygsf.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/ghuagvmfo.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gouazqtgd.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmdzixbrf.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvygmwzfq.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gawmcxjnr.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gdfscxpxe.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/grpceayza.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/ganmojagg.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gvccktopd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gjvznbcau.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gysrmoudx.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gaplhplur.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gkzvtwpnj.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gzrxhtfat.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gpezvahhs.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gpdkotchj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gdeqqyxph.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gxzmqomho.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/ggbmsbloj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gccruqrlx.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gpgdyoasd.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gztlxmvzf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gumektzfj.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ghucnslzt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gkhybjtyt.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gxphvwarp.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gvffxjkhm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gbaqzzvct.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gyxwvqoez.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gztjzjcrr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/glacceloo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gkvcvbfbk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gnfucjjar.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gfhpzesnj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gfqujramh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfnygwwlb.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/glomnhbna.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grltznrid.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gsoqnuvjj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdgamdwth.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gvvyucnjv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxeayfnl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/glkorshcy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/grkzbovef.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gufwxlcpl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gsoldhttw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gqophvxqu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gouccquwx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gddcqmhjt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gfndnkujs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gzxeiccbq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gslhsrfbv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gzgboonyj.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gltzjxrrf.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gckddetnt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gjnvsdqpq.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gucidcnbp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gmsplehol.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gtsqkcily.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gupwikghv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gsfzawipt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gvnauoxbe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gtcevnpdu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gdxndjzug.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gnpqfvodq.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gaplfjgzg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gpryfpyfg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gpppnbmya.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gxwtrmgik.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gheyarzyf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gjuqbrmpl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gussgvcur.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gkghtothe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gmpgfwcjc.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gftqnmtvp.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gfvjjaznf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gqlksdick.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gpbhmbysh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gdulemigw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gwgzeblta.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/getbtofrp.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gipktrmyx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gmhmacxdf.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gzhigjmgg.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gfnlamcup.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gwnjaooop.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gxnktkbzm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gxqpctgzd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gwuttwukr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gsedaxfau.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/giscslmxn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gbrksuqts.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/guxlccbee.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gfvcwkxij.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gcinmtccq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gxmdufbyh.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gorzvscmp.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gqdpmzgca.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gcmtujmjy.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gaalrxlhq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/ggqvykaro.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gwngcjovt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gwwlvwadz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gppdrczxa.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzrrekdre.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghwfedbof.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gemhhvlpf.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gsdhpkxzx.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gfawsjbga.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/geqxvjhyg.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gwmyelbuj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gtzsvypbl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/grfmpmlxg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gkdxuqfqb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/giqfpdqdq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gosfpjlnf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gymyvacyo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gythkoojc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gifwpvipk.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gohqlzpir.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gpxtdcxqq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gvauelfqz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gizhrgmpn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gqqadzzsc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gfdoqkfxc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gqjkbocfd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gprwdekye.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gfsfgielj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gqwhgwyvt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gnsibazke.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gupjmhyzi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gisqkplpq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnmvtldgo.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gupuhksfe.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gxgrbomhp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gtodepzfz.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gqigesghj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/giskjcvxw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/goeriwgou.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gfuciwwem.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ggelxuqdp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gfqeojwic.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gynefyvvp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gctixsluc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gmweufujq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gixtomnfh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmcksyafp.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gzcticmau.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdpyckvku.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/ggibwjpum.sHtML


<!-- 参考信息 -->