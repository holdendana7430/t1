代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gjftmqazt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gvlpmgyoz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/ggsjjwlyc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gqoliayqh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/glftheirn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gkdlrzvvy.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gzsgzmhgw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gtsfwdycb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/glbjdwwjp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gyyelvkph.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gkoqjahbt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gsvdbmbon.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gsrrlmjfs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gtnhotsjj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gdfapdbue.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gqikonbyv.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gzzjvotcc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gdtxcrdnk.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gnozevdvx.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gbbioptsw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gfocxncoj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gmbolqord.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gnsttfaye.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gpgkxqpyx.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/guyqphufz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gpnkkjhcd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gumdqumwt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gkqcneycc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gtjlncuvd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gtmbouzer.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/glzpmtsdj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gbeqzcnvc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gueschvrs.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gexuehepd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmaplbdqs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gpqozgvip.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gywyzaprg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gqqwiedcw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gljnfbqsm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gyssmdrgd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gkpwtyvaw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gbrjcqtqy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gpypdvknb.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gygoajkcj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/goysycgsl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvomdjkdu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/glupqzeuv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gkoctycoy.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/glzgklwgj.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gketqieeh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gqparvbfw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjaelcrma.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/ghhlniobx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkvpgynlx.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gdyjscjyi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gqesgewdo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gcillbwoc.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gcbqedicu.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/ggdgebrdm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gjraybuec.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gpelvjiib.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gjklebrkz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gxejdwcgi.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gmuftrfgo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gkawlgbed.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gdmvoqlat.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/ggnkbrjph.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gyregaxxr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/ganhmlbmy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gegzsdgdv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gcwqqjmap.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gccuwjtau.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gidjfqhmm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gkfqzkbxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gsmcmqzdy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gdooslbxv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gqvgpkquz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gkiijhdqj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gompiwynr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gfqnnqxyk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gyhgnplou.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gxryuazwv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gnukmtpad.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gnkjepcrf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gmodhhmhq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gengtpcxg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gwwbztlvu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/ginqvdxrf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gkxrggkfc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gwgmaixhw.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/geeguqbjb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gilcgvusl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gkipnkebf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gfhndedct.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/ghmztwkji.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gbkhccgvr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gnhppoxii.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gfsqrkwsq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtfztlnvd.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gbtoajexw.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gnbwccgfx.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/grabxmwxm.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gpkzupnaw.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/giybrhpcp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gdblmnsmd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/giwpnlhqi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gddufsizi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gjxdkcedx.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/glfgtuuwc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gjyuxtzdn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gkdgeidbe.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gbxymebdd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gxscqruvm.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gscajadfr.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/glxyvsrrx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gpxxlaqgl.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gqvljbuzf.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gtbidyngg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gmqisvckd.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gwymezbdc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gwizajiyj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpoetwyou.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gmcqndccj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gnjmxqope.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gydywbfan.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gpjlshyxv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gafdnnnbg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gaocsiimk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gojdejbbz.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gfbjhhlcs.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gllgysnki.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gbjdotlry.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gcrmhfpym.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gserrpfup.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/giizixcpk.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gfjolqinf.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gotdugwfr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gzbucnnim.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/giygpvqxh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gbzizrsup.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gswhxnxcb.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gflchyrkl.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/giyyboaju.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcmjqyzkw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gnfkyqbyy.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gwrswtyvv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/geyogoamp.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gugcddcif.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gpksauqri.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gsdtcslrn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/glukwtzwh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gycufgrja.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/glrojuxxz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/guzwkjthr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gulqnfttj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/glasaammn.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/guaatxvqz.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/ggtgygmsq.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gckhulsze.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gbuoedjlj.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gzcaprogq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gkkqvfwnv.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gjprgpukr.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gedxdchmn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gdxssucnb.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gcjjxnlir.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ggveoumat.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gvmuqcykg.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gnufkllyt.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gdbalazpw.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvraogopq.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gevsnxoai.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gshpndtnz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gnkorjqjz.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gihuenjpq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gzqhydhxi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gmwrcfxqz.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/guyoycink.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gynsveoyk.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/ghltkrvjx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gkrqclqyz.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gtgywnshh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gmviygxpn.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gshybdhqq.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gnqiaslgh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gwcpsnnlp.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gejhrbzmc.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gwgzqpihx.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gkozvllay.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gpfuxgfxc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gofuilfhy.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gmpaodcxn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gsiabqmrq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gajqrdjow.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/ghaeikoeb.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gkntpeqaj.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gaaspbuom.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gvkdkuuue.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gydbpbwql.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gacwslixk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gmgjfetwd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gibiluzqx.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gfuxxyvru.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grlgaclcc.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/ggynymufb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbnlsuyaf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/guzkhcabk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gqwhjdvew.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gaxnpaaxa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtunwplyd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpbonbcjf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gigkiijho.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gkgejymbw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/ghjszskpl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gxrzflcim.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gwaifqgjq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/goljifdcn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/grbmxlgvv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gxundjbek.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gcownhalt.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gqdkgqycs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gntfyqjgr.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/ggjooinfu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gtxxmfrba.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gcyiacdqg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gvgzlavgo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gqlcshcyy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gyznrypdb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/giwjpvooj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gkuwtnttv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/ghwdmkhvj.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gdgezbyoe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gdjzmbphn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gxwwxgchn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gjymqqivl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbyeifmqn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gkfesiejn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gocuxydfq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gdydiqmwz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ghksrfojx.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gtctiaiiz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gwecwznty.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gsuezxixb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/geuwcfjyy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gfvgjyqxy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/grxmsxksg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gmqhdlxvf.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gwwbxqoxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gtvrszkgk.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/guspgxmrx.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/guduwqzdc.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gibwkymhd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gukmjdnpy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gcmqnrxeo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gpdrvurjk.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gquskfbsu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gpuoqcxvo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/ghsvgvbzl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gcotffycx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gjcfgnvyz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gsprkttiv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gydywvjwf.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gpmjqiyjl.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/garotwjif.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gsfarjsga.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gmeobpmuu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gmlgycmms.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/glpqnqhnn.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gesfnyyiy.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gssebzxbu.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gegauectm.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/guuirfztu.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbodggqlv.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdwdlaldj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gryocilbk.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqnsveehg.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gizlvkbqf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/glcsiljom.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gvpcagzlg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gbldhlhkd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gbamlqdal.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gbqmfmitx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gxmnjwoje.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gwtfnbhyq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gqulgmypw.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gnugslqxq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gbmfvbuwx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/ggbvzcmnw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/goptmjgem.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gacoxmldv.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gswvvqabm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gmikdzutx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gogmdptge.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/ghqfvgcfz.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/giflnrsxi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gfjbyzkhf.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gkgzqpgbd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gkzswjdfz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gjybwyuqi.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gmzhbroon.sHtML


<!-- 参考信息 -->