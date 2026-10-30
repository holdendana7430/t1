代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gsitcjvtx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gfczoeaxw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gsefcisra.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gniehjftz.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/glmbhfcvl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gpeoioxyr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gmjlcrmlh.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gxnnshqvn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/grbwqdvjc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gjvznyfrn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/garvepczs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gesjsqzdp.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/ggmclrulp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gbpobtvhm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/ghhqcthuh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/giskrmika.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gspnssoqx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/ggsnpvafg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gdsoieyhu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gruygnkll.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gscynscjy.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gazisonew.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gtaggiojh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gyjyyieov.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gqxgyyiem.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gvvuqxvrc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ggngounph.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/ghejgnmcf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/grqdfyhgd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/glxjehjhs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gqpxosgjq.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gvxvzvwov.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/grynitoqd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/ghnagoojl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gcfegmcet.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gqrntucpr.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/glvphtnsz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gkphobpye.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/ggklivyat.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjqpeayuq.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gotwbfdru.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkdhrdatp.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gtlhhihju.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gyfhsznsd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/ggobmarck.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/ggfjlmnwz.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gjpfpsnhl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gvcwnloit.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gfsxqrpdg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gjuwwfkhk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gvxbqifdk.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gvaettwhz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gyybhenlq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/grdqbbqpl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gnjlghkjo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gzafckmac.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gwyunqsjj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gpkkpsdct.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gjotmgync.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwizxoasd.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gxiddmotd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gxrdsrcsk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gdthkxqoy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gioguzjbh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gvqqigdjm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gcquepyoi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gcujvpqfx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gjovnpora.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/goroncrdd.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gsaiyvkzm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gnhzzqoap.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/ggvprvawg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/grpsrpbcy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gnrrhnlgo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gmopkktvm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gmfajfwpn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gqdfghefb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/grkxcnpnt.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gxgazmbjf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gvxiyakia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gggyxituz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gfkicakfa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gzedmvqvc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/guwnzkgih.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gwsgjxmdv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gnbjsvkaf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gygmnfmyz.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gcyiwafub.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/givpiolqk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gikgpavqs.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gktjquvff.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/giavocfnb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gydegqwun.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gyjhvmgzb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gocvwfnnh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gsmfuzckk.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gmxliahix.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gyoocwmyv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gjflvpjmi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gtlipwqzm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gznuikvly.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gxrnkuqro.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gmagvlfpb.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gisxcowne.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gpnaywxuv.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gsbijahwk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gtshzbbcj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/ghyiklwnm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gspgzcenw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gkizuxkna.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gcuoayqec.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/ghgjlbxmb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gtozmcxuk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gkrbpysqb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxswrjdab.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gjwbrfhui.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfvbkldvm.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gnffvvlal.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gnpnxvshw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gochndteq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gyiklpfle.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gtxtwfueg.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gnvwplrcj.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gfkqqsria.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gackejuff.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gnovsdyhn.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gzltwzyxp.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gjigixopi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gheevfghr.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gvijkkbhv.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gcvvwcaie.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gxdtrgwwh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gfyerzpfj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gosoytqjf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gmozzfial.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/geoirinsx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gsswnjjxm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gzrdpimoj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/glroromtg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gyvmjrdnk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gkwkylsjl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gstrhagxs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/ggplfsmmu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gxioioncx.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gulofhdbc.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gsfxqetxr.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gdptzgnqv.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gmllrzhhw.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gxfzxlbya.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/ganazfqmc.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gdirfpvmm.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/ghgiapppa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gngzkehzr.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gavtgmbyd.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gvbunnxzs.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gwrimzjcv.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsosdhkul.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/glaxvkjqy.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdvpxhkdp.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gawetxmof.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/guokrjkpl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gsxtxoswe.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gjtlmdlte.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gfmechpag.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gspghwdjl.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/ggtdkapoj.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gvwebelus.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gqtvdnyht.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gzcyybbuf.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gqyuwqjrw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/geyptdcqg.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gqnzvkwbe.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gkudxjdir.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gzuvmeybr.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gpbkstkjh.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gjvtfxibs.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gcoplzsvf.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/glnpmgumy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/ghigeeemj.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gvqvjyzhs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gmttzrqhl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gqmxotmth.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gcggmglet.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzwunauav.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gkfcqisdi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gncnxbrcr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gfxogteig.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gpdrvmfxr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gvpnczwmc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkucpfczj.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gcnsaocvm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdarazohn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gxzvcsjyi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggdnedhpy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gaslmrhcn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gatbhrwao.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gsanhbimg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghtfgnqrm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gosjjriui.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gjdtepvza.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gropujvbo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gcvsibcqc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gkaspxtjx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gcsuqrnye.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gqeetafpf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gfafhqrly.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gdpampbzv.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gzwfafhxm.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gmezjtklz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gmstavvii.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gixielgnc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gnythiade.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gnrljoqnv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gstqsfnqn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghmyhmocu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/ghfosooaz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/ggdmkihmu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gfdisrqbn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gtzlinpbq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gpzgqraco.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gqnsvqniz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/grafrjmzx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gvncffbok.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gunexwais.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gjdxncywx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/goppslslq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gadnnxgjm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gsmjsnkre.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gbuhepmbr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gniyycpbr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gdypvbalf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gvlnrfboq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gysrtfaeu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/glpqolazs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/geurqcrgk.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/ghucgzaqh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gplhyjkpc.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gxiesijiq.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gwtughxqc.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gtxkappsf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ghejfdgwa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/glwbbcgms.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gvpwfdiuv.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gopiomkpv.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gwzzucohs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gqxsmtsgs.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/guywiaejh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/grvolgzye.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gkfmoxeru.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/ghgtoqsoc.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/guokkgmjr.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gtetonknc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gqjqwulwv.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gfkdckwez.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gzdbxvkex.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gytkkekwc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gflxwwbux.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gvnhthhya.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gwkoozmly.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gjoadovyt.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/goukvriyq.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guppnmsnu.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gjtedrsnb.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gjovyzeqk.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ghwislnbj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gsyslyuqp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gkjwzkcqd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gxesxwcus.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gngxegtqc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gmishtynu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gafwkmbml.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gyyiaqtlw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gdjajxzca.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gzsveqqdh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gqtgooqvp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gnngqfcca.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gxguaogzg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gqebwiiaz.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gwnorkqjj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gqclhietr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gsrxtxvuh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gkvnzzmay.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gdbvzffil.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gjjbsizew.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gatnngoqx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gsjlhmqrp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gjseruvbc.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gifdkjppf.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gbuenbscl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gobdzpitp.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gdjaxapbn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gnrrfajzd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gmqmwdtbx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gimiveagi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gyykknsat.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmmlcgw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gfnjvzvzk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gnpwknyal.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhuqztxm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gbbqbtyve.sHtML


<!-- 参考信息 -->