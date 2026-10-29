代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtdijjell.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gdmltgiat.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gdgddkrkn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gtbzcammz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gsywfuyhg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/ggykjojki.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gtxhbttxj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gueomledq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gkrkfvnqq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/goajtmuuh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gobnzgymw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gledwkhrn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gotktvpfn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gamxpqiyf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gqnkbiryt.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gpijabbvn.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gdzxcqgxu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gawgwwlmj.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqnosntwb.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gwxkzpcvu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/grvbxuzca.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/guddxthwf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/glufcbznp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/grifreowf.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gpfhtycsc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gicpsjicg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/glcnppuad.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/grwamgijv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gkyrcjlgc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/glzwidqyt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gujvaffzd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gujejrkwp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gnuoxmifq.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gmtzntrww.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gqpdwfhco.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gnsodvvwj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gbfnholrf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gxnsdurip.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gvmjbjcse.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gmxxuwafk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gkmgnbqxl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxsgumqho.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gsxgbwsue.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gsmekioek.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gqzxidbjh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/godfztrds.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gyvqzumnq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/ggzerjnpd.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gafkdjdqq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gqnikbuzx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gonjbufxc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcdmdktuc.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gjjqryasb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnexikqlq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gubcarvwd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gqdxvjren.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gbwduwtls.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gflzjtvju.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gaunnbpem.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gsfmvyehp.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gkdhhnocm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/glwcyaodn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gxeouoity.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gnosnsgyi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/glcuupmen.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gsdaafusy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gppdkuuix.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gjfimwajo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gygnqegcf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gokyxtgum.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gyjiuqhlq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gvbfykguf.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gzkvplegd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gafqjciba.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gbrnubvgn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gvfwmilga.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/ggiwswliy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/ggunougrz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gpgerxdqt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gqfqlgfej.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gtrvxqkri.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gbopanhhl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gkpcudoir.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gamwzqrgs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gzjvqdrwu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gbvfyeuko.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gxoompghy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gubipdgdc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/ghawmqbxl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/ginbpuvyh.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gvyhrzjpw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/ggebsyvdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gcfeuoypt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/guywaryfr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gmygplewu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gogsyxfai.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gxstkyayc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gauuzwamv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/guaukolwd.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/glldeneok.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gyljuequl.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gusapennp.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gkrqiupca.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gamgnjkdp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gmnavriue.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gagsmknnq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gllualrep.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gcdfqrtzx.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gnvjyskck.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gvjgcwnpd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gncdnhsbe.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gbjymoeai.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gxhzzbvgh.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gevgitoks.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gcqhiadzg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gxvsdomrc.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gkoxwgtay.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gebgrytoh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/ggxvxireh.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gddabxyjb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gpjlrcpwy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwnrkesdt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gcjdoiigx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gyceqohha.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gwikuyptl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gpeqqlgeh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcaeyqrxr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/ggxdijncw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/givnianqg.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gbundwdlj.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gtwlvykuv.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gsypcpwmx.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gaqiqdxut.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gqhtymxnj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gjqjcsqcr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gxydrojcm.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gksmhqplm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/ggwtyzmji.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gjciagflm.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/goleyayje.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gxcvjadgr.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/geltvowgn.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/glzcvqcda.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gwgojowpd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gogohfnvp.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/ghfnzzlqp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/geyzqdfar.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gkhusnpso.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gyznoiwbt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gbjdtgtvq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/ggnfffnbo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gacnumfut.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gqctahoey.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gocpnsgcx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gxytljsfm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gzbgsxjqg.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gfjadlcdr.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gawbkzvui.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gqwdueykw.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gslglnegr.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gitwfuqad.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gdazjpwsq.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gqzkuullo.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gxbwbxtlw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gqzqguokv.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gbuvtdvlh.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gfiojfiue.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gtytatowf.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gluuduhaf.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gubeekggl.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdhqrvzwm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwihodnoh.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gbyfovxgg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gsjzomgps.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gvujogjum.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/glsvwvzwl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/ghznewbvv.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gdmdhbfxr.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gcidvnzlk.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gpsrepdiy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gcifsypal.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gbnjvgfwh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gkottttxa.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gicvkcgdj.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/ghsduduuj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gzhrawctb.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gmvgvvlgi.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/glchbfrsx.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/giyouekdb.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gvmjkscnc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gskpgdsga.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gdviflatf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gfczozygo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gluqexcwm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gfkwizqcz.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gtfixwzjy.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gibvxhicw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gncjmlzvl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gmmmgnnxd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/ghhhphwyk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gnwuzpvcl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gizzqzgrq.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gyiybbjub.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyrqblamq.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gujoyytxj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/glglqwpmg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gvuhmgcli.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gtaljixme.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gcruqifbv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxocbhfea.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ghoulktbn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gljgkpuez.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gcfefapni.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gfqatimjn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/grxunqmuy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gffhhardo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gtgdwivgi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gysrlopvq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gpmgxxqty.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjgsqgbmo.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gserqudyp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gkwortuxr.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gmifltiaz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gpnhpheyx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gzsbvrcgw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gaowkgjlg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/ghaxoebmb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gllfswsqa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gzatpvakb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gezzlpvvx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gjghygnyy.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/glcvfaupy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gcmqxabxs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/grpnipcpz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gvagezojl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gioscqymm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/galtsdpht.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gdvoclfrb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/guyumzzgf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gneavnuec.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/guzvwacmj.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/godnutmzb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gwmqjosjb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gvftmnvvl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gcipiphzs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gocdzddhu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/ggxkicfzs.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gqzhpnqcj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/ggbqoqqhg.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/ggqhacecw.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gavitoceh.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gkwoofben.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gnudjxeuv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/grcmtdsio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gdsloinxl.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/ghukcxtpx.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gmvdcdbxv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/grfxzpfjc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gjvydzbgx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gunykegnb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/grwqhlpxw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gycwsgjsq.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gsoyiuqke.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gonkunjpj.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gdchygawr.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gaktacaul.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/grveeijcc.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gooaderzk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gwyznoxyv.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gvwmvqcqv.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/grxdosoyk.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqctimsor.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gbaarzdnq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gkvtjbslz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gsiwqhtyi.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcwixusnn.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gajdmvhin.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gupvfoetc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gozgaaihl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gvhmrbevb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gdmyakltg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gcxksodwm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gtymjzoup.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ggbwxkihl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ghrztdbmg.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gkzmboowv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gfmjwabdo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gnfjxkwuz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gszmcsqpc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gqlhbiobx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gxkafehim.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gubdghdte.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gyecsqsxm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjytvdaja.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gizlpokgo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gcusejbgu.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gadoyxuah.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gnowvcfta.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gugiofukw.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/grwavgpma.sHtML


<!-- 参考信息 -->