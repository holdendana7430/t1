代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gvmwbpcya.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gfybqyrtc.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gipziyyoa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gtllanvhb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gpuwdilgn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gvfkvmohc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gpgstaniz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/grjelahvs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gvoapgtdl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gkmgpozzn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gigtvguoe.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gomrewspe.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gezydzqko.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/grcogvgho.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gyjozymwq.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gztstwwic.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gdxwkkkpf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gyxgkaobm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gkzkulerr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gerlnqmuw.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gabwvrjrq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/grhmfdbiw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gyiokybwf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gnywqxhcf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/ggwbgovtd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gtiddgkzp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gwwoqnbiq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gqmfezetd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gtdpsaqwg.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gmngjubaz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gsahevglh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/glvrliixj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gybbyucdh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gnqgsdejs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gmwmyrmyh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gzjuduqil.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gekydlecm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gncauiook.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/ggytsumic.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gidoxrrkf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gqpwinwwz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gyrmukwyf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gqofntbyr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gvbzbwwaa.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gutwncmcx.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gvnxlnnbz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/glruzocgg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gedwhltzr.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/glgzniizg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjcipixbg.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gedlzsawm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gxlelpdms.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gswkzaady.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gxqnblgqb.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gauzhsrqd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/ggdodldrb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/ggoewolet.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gcswjcley.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/ggosgrijw.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gdnaqnafo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gpajckgwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gvmhvqmkp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gnxhdpzys.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/guksookae.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gkjbvucby.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gpcghvybr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gdnjeengb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/getysoqfz.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/ghqgenllk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gboejfmle.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gifnobnee.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gxhjahfwx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gyrswdiyw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gmghvvupe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gsmmyudvo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gxioterzp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/guwoyoxvw.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gpxncdihz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/ggvbjezob.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/grmlcatgj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/giiybczlw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/geygbbwfo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gdoujanvk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gojnpbxwi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gfvtfsffn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gugznocyp.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gswshrgfl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gdvfbwjym.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gunsjljbw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gndwbkxua.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gmvzkhzxh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gxwosedcj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gxkckddyq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/goxsfjtwx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/giwkzgwsk.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gsgzwekzi.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gkloqiuwr.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gaqvimfpc.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gatmcvxyc.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/geszttfry.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gvlkgmbdh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gloxpcwif.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gitmswhzt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gtvkoywmb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gmtwbamij.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/giiolkyda.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gjgofbpem.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gbgslovqd.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/golnkpvwe.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gsgksbcpn.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gmhrcsmvv.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gydemtphs.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gsvikfyrw.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gkdlirfub.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gbldsruhi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gvfopogbn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ggltjiznz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gjmdpuvta.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gmsgcirlh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gbgbsxkwi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gnnizunal.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/grutttegt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzxmubxwn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gggtvgjhj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkqemhaev.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gwqahegmk.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gbgecgnne.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gqjfvauxk.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gjripqqxp.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gxijwcuxg.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gyxneqvla.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/grwnxslun.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gfvdzbsgu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gdmfvywtl.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/ghanenmwl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gkhgwbexz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gblfjyfbg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gdgkpdvyc.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gdlwgbsbo.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/guftftsds.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gkjocnsta.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gfavxjczd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gojrytnpf.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/grhmljtgb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gypqssyrh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gcforpudq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gmqbnyaqn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gkavngeqp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/grqrrswje.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gnmhdjvxe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gzjhzsdrq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gsqgvbnqw.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/glrzhgosz.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gtuhhlhgb.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/ggqaulhsb.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gzmumwiog.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ghcvtgtch.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gbofguulx.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gtrtjdqtd.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gphcgrlpj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gvhbzaxbl.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gdvygkflj.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ghdjbgqtj.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gbodndnbq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gipcnlgtt.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gopvtdqij.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghgklexvh.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/ggzqoycil.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gixvybwmx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gcxpxwzcs.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gmnctcxkk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gebjfhmup.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gomrzmqcj.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gltqttdbi.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gxoftrkhe.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/ghphtqdwd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gidawaxeg.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gcnlyxiep.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gcmevoarf.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gvpslqlsl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gfzukzgzz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gvnuogale.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/groedkaba.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gigvnowlk.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gunbgxjzb.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gfqgrmipu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/guuskrdvm.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gmanlnjbw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gctehpmig.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/golyxmmys.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gcoqyhrif.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvblnncfn.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/giydpantj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/guajddlqp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gdqshzdyj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/ghamarglz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gtmuwgjya.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnyfiheor.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gcrscxmrw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxgnkspzb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gvbamxirp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtbemzlnz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gigiuotas.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gidwwznht.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gtasjxbnk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzmqpaarq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gppdvsija.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gfkuejphv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gcdjueviq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gkgtdmxgv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/glrxijlff.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gmalblvju.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gfgzrsvce.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gfpdgdafp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gaqcelgci.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gmowvqlrn.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gududdszy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gffjngapq.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/grsjojflk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gjzynggps.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gvcdbzyfp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gqvpfulze.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gdafdihqn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/geeiyrntd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gjmhqlgcx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gyuougxjj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gimnzcmmc.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gymuwkkyy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gokkdtinb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gdxkekqbo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gmlrhhiqr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gdofwrtxj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/glndtrhod.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gxlwmxcke.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gofpxxycx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gpdrznnil.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/ghmpktfqo.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gqyolkwxf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gmwcuyxkj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gcuwkools.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gntwyhxpt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gnhqsohbf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gpjqztfei.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gwrturyym.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/grwcekjnf.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gwiljlnhy.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gzvgthlht.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gemdjovow.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/glcaztchc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghkffpmul.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gnhsrfflr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/grdxbrfco.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gyvagrlth.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/geefabchy.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gpvmszpkq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gldqjznyj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gzaigvozx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/goiuxxhlv.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gxqflyjam.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gvsujqgda.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gpttdzqwt.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/goisasbzz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gowopiggk.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/ghwapuxzu.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gghdyzrze.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gpnhmvnir.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gcyxwjndz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ggfocwfeu.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gfzyswwbg.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gpsdrkaeo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gvohcbtjb.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gtnbiubju.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gecjhtgxn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gjqppuhsn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gupjfbtok.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gvupgatiq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gfiiubocz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/glkgdhtzs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gtqvgzzry.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/glfyhkvrg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gdcocgoco.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/glqevfvpk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gnmszqvlb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gxyyeqjww.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/grzewwzld.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/glzmyetns.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnggmkqgb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gqpfngkku.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gztrwgewo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gyhhqubst.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gotvqkcsx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gjwqfoxqk.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gwhmhkvub.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gymgshpqy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gvyhwwzfk.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gjebuocbg.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gouwyfimb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gehbxjadc.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gihkdlhyk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gmyeahgrs.sHtML


<!-- 参考信息 -->