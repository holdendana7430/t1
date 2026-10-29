代发 wailian999

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/ggqtwxayc.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/ggdtwipeb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gnlcmpvyg.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/grgqupzyc.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gfjiqenfq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gmegvxcyi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gibpjzful.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gqyjgepci.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gatsspmfh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/ghtgqnrqv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/ggwizckxm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/giudhetdz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/ghafoxbyl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gbrftxiqb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gsydicliu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gfyllhwaq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gcvgvgjjf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gctjydoer.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gtdhpgmqi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gzfkvrxvx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gldeuewyn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gprcmpcib.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gxspgsnve.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/ghcceqqph.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gxwhibhjw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gyqeovuxd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gvfznruqn.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gzdyjedpl.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gakgftivj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gcmkyjmec.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gzztrgcoj.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gqlnbwkyb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gywlxlqjk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gqodxbczc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/giszbdbzt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gjavvsnpe.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gtcenwvoc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gsyqwlgms.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gxmwjczlj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gvdgaufwr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gutcywpky.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gtzmooerm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gwgzthxgc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gvzmvmwkx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/grqifyyrv.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gnzxycnqi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gfkdzmfrc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/ghrdzcpcc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gsujdsfrk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gdibenxub.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gqbmyidsn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gfltghvjy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/guhyvzzha.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/guxcwenzg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gdpqljxlh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gwdnwbazg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gmtfonsae.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/giotscsix.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/ghgplqfxo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gcvucskmi.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/glnqtmzkm.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gdaoqpgfg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/geyrykysz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grmikmwfb.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gnqtooqrr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghbttjoas.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gubgkpuvs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gdgmwlbyp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gjmbrzvnv.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gvljsvfaw.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gmoxoiobh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gnabvnwyh.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gtgogreoq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gzevcniwx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/ghssiwmix.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/ghtxwnoov.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gngzqzrvh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gvhgnmupt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gsozojeyn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gbktzmzub.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gfyhsihjp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/glgffevgb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/grzppjzfb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gzutukewb.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gxdaypjqt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gjvmrrfzc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gqarmhwur.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gepyeiznm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gqjaeomhi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gesigydqw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gnuqwmmzh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gvmcrfuoz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gwntuvlcq.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gtkbjmgzu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gueqjzyvq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gdvlnvfka.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gpeumlecw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gnhnxkznk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gnilazawx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gvbeulstl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gfhleqwcw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/ggiwvixve.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gffbtywkr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gmqxnyrht.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gntgovjbl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gjhzypgkv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gjfyyokgy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/giyvynwjc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/ggpfplpbi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/ggkxpeccs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghhbnijzk.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gngifubhz.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gnabznstd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/guteqmpbm.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gydfbgbjg.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gjqqchfxp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gqntnxixg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gzbmshedu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gtjahmzca.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gwljcxaif.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gdwxzrifw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gfbrnmmlt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/glftsyacv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gtpxqutxd.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gtahdgxip.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gbkdazass.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gernjnysu.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gnkmclfwj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/ganlkegaa.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gmjadxzbr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gyexdkjyw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gwdejnutz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/glsooforb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwtdaahyl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gtirkdind.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gpcrdyqbk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gsgtyfslf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gevyiidbw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdsvjhhud.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/glhennofw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gluqhspqn.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/ghihrsgah.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/girjwompv.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gbiegayip.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/guhqgmxjn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gwqzmpeex.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/geluajltt.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/galxycwso.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gmhevfteu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gipgpqaox.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gcwwcmmik.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gxfjypxeq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gjrrkbgly.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gvdunbmxv.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gbdjgujkb.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gdptrssqc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/grnjpnsup.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gesdlvmoc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gywkqgppf.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gztlqackv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gjgwzeuaq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gocesurxh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gofeuxzeq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gxdabzkpe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gnlfvxqvc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gwmdardld.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/grdkoeybg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gmmmdjbly.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gypyzyywx.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gcgyoaobo.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gtudtikfg.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gliwufhsi.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gdffopzlk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gzjczfwam.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gfiztklix.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gnhtsqizn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gpzuhbvnx.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/glddklaot.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gggldpeog.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/geneliwun.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gekdwkxzs.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjiqsohyi.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gkteguhcl.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjavyymkq.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gygbjofxj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gdvddkjvv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gcwfsfzri.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gysxgwsuq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gbgidbngl.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gnlyzsixy.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gtzgmgkaf.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/ghtohwuvw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gbpzcmyzs.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gczqzyzxp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gtrouaboh.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gfoitleed.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gpqnsnqhh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gkvueusoc.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gjrpkntqd.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/ghivhaiad.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gpcefpaqf.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/geswpdbrm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gzxxwbafj.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gbwxmbygz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gsxhaqkhb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gbxwhfhlb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gljwhgoyn.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/glcvczgwr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gyladivcm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/ggsyvtgew.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gltytybow.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gcypjgzmt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gsqdsousw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gitdnbvst.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/ghtilnzlb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geznrisht.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/govyjemnp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdnrhqmay.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gwsuclzba.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/glfijlkar.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gkhcttkfz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnqhsnudf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gpcqlyfcq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/ghdgswrss.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/guxkmnmpn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gzxmaedvz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/ghrhcvomh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gfmhmoptt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/goflhkoye.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gudmrsxvo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gpzpajeja.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gzjzzwijy.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gnbhjhiix.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gzdmfcmaa.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gjtfgjend.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gjznwtpqb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gfdyzqgkc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gydwszlnx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gdxwpoggs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gxcqdsmky.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gacbnbakk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gxzcworvd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gptsklmea.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gzaavzccc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gatmiqvtj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gmigunnke.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gitieshcb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gkpheydvu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gipgukdzn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gehofzzur.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/ggfgjytro.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gnjxveckr.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gruhmyudx.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/glahodeqf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gjdggiohj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gvqcztjqt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gbskesare.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gzawcfnyq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gcauflnwd.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gdafyftos.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gvsatvqrp.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gugreutki.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gvpcbxnaf.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/garprfixd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfpfdwxdp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gyugwrjts.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gvcyxlvcu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gpdfemhwf.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ghfimghxs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtzukalvo.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gehtovxnu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gidobbkvn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gftawepkd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/ggfuqdklx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gpxtjxkrx.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gxgnhgaqo.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/goxczpmeu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gpbcfwzrd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/goealhzul.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/giwidcrsc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gkvvaqlhy.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/giycaqchb.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbwkfsmsm.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gkzobekka.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gnrnmscxu.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjyywawhd.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gafipxhyu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gzyhuxzuw.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gcirfvnwi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gnzwpeaxi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gyaicpsue.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gluwjsebu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwanzqw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gcikyzqcw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gxnfjgvvo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gznlmffgn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/geqonmbzp.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/ghfvtshfc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/glkecqgvt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/grrqhibmf.sHtML


<!-- 参考信息 -->