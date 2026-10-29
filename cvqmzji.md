代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gjbnwstba.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/geljsmnwx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gutyxzipp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gzufxpbke.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gmappwzzc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gjoquvhsg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnbszuxai.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gvjagndzv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gvicvnacz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gyvztnhhk.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gclojlzho.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gryyychoj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gwgdtjsox.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/giudhxfqe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/grsmvlkfd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gliajkycm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gviwamixl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/ghgrlvvgi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gstiuzdpa.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gsfiwaupo.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/giptcjkax.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/getlzoexh.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gstegykqh.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gikwpciah.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gnkexcyhf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gcaxyamrb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gsoljepbe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gvphmtmje.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gxprxaocy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gkdukqser.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/glqwsapsp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gqpmsbepb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gzvpscrli.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gswtvjpxy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gzatomovj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/ghpfvhvil.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gelyttwnl.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gydfkylqj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gyapxplwn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gkokwoncm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gajivxpva.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gcfpdhevc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/giovnfvwr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gjmvnetco.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gigwwbsdy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ggugrekeu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gyceuiapb.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gjjhcldpg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gzbbgemzs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gvcqioqcc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gmntdhqsc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gpsecyusk.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gbjtfzcuq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gknbbrgeq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gusstnajk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/givnnegaq.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gydssuhri.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geijnnuec.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gatrmlxwt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gzwcsclbo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gtmqklymd.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gbkpikayl.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gkpaskpkh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gxkimkfhf.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gvrtyjcvc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gjfszdckv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/giobbvifd.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gjcvdqsuu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/ghwgvqaxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gavncwmnk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gvqbjagpv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gawjgfgwi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gifxsadnw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gwvqruhll.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gnwtlklfm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/glqgxvijm.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gblvxosdd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gswyodvoc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/ggrswadps.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gabtowldg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gdwvglcwy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gzvdqshws.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gbytlmfvp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/godzbqzde.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gjssijvco.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gxpeuufvb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gtuxxbsao.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/ghffzqrrv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gyrgvrefu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/giaykgwsu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gwyetlcdt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gdmbxdcjq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gxpupstdm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gzgpwetuw.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gxxwqrlwq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gchyyddat.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gjnmxazti.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gttbyynhg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gazvkndcp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/grvfvawgk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gcxtgmllc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/ggntpgexs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gowusvahs.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gbmubwrkv.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gpcyugmib.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gbulocwnz.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/geofseqoa.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/geierfxpu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gnqzpltwg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gpsvkqcef.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gqyfudrve.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gwgcvoclx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gudlcruue.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gcvxmtccu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gnibaucep.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gjzaycdwq.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/glkegpuxl.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/giuicwvtt.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gwrwkcaaj.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gcgvploak.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/glbccmsse.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gapiwtyuq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/geavmkoor.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gxtpnaqsb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/glvtwewnw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gvzusjowc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gscanwgrb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gnjsgkyii.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gidatyarn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gxnbbyaaf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzyjvuihb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/ghqhslbkv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnhtfszdt.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gcguvwdlu.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gibymxikv.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/ghlslqdhc.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gjcczipqx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gtfdapzgz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gozakzpep.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gmozfgfvc.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gbmmsgtkk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gqzcpgxnq.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/ghirostsv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gosopzkbv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gbtngnbdp.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/ghsjehzry.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/giefsyovb.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/guxaakqix.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gtiowwnck.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gkldhspir.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gpinhbgux.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gchcdibil.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gonjyzcss.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gwwjqaqsu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gbnaxrgkm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gwqaabjkw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/glpdjgcgs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/giqzuhadb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gfdlyaxtl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gmvvdfpqk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gbosrcdlb.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gemfmkhju.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/ghywerdwq.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gsmiiklko.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gjkegjuvi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/ggmhffnwv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gbfcvagxe.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gydpauwsd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gyigxnuga.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gcwlschbv.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gwauqfogm.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gzdsdettv.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gkkujxiov.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjnekfnfl.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzplmmxtw.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gtzmygsee.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gbxezwevp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gkqxuwedk.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gdrgklgrt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gspssiohv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gcgmitwjw.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gypdyntfn.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gujxjscpd.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gbzulpccv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gsczdsody.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gaelzqwdo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gxqtqwihk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/grbkljipw.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gcsdtdzwx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gongmsxau.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gobfbekhe.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/grlxakwuf.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gfjbyyhhu.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gohpxjlrg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gkskjwkne.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gqqupqogd.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/grxtmyxxl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gvqnzwrat.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/geldjinuy.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gwumvpqvx.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gtswrbans.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gfijnfcyq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gkrrigkkl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gjoaanmww.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gskupwlfp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxmgmzhgn.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gtnphzkre.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyacfelzi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/glbfcyeqc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gywjsjgki.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwwtisiyd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/ggaiwxlei.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gxcpayokf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghyvxrtqd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvporjbad.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gggclkiaq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjwfffgwr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gldgoqarp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gdeudlbac.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gkkygsuqj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gamimiebg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/ggypjrpjy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/ghuxtovrq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcpwsiami.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gheamcjro.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gmuhshkmj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gqjdgoppa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gxxtsjydp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gebmprciv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gymncjaml.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/goyavhfxn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gnyfkyxrb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gxyytcnml.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gymhdqztk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/goleisbdq.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gyobcxvfy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/grouthzvz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gtgxlddnf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/glplbccbk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghwxepmyb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/guquihckx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gxpvbsvvo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gjqacrknh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gifswjosk.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gbeprdrsv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gqdgszkdi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gjelpqwhm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gyjxqbxqo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/giibekbkj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/grqxqdcgz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gmlgglxas.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gutwuepcm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmezlbpel.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gapizpmxd.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gludzzpha.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/glzlrkaim.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gudmpknmi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggjavvhgt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gpewtegbx.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gvxmsemcr.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ggyjzkvdh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/ggpkphfpk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/givocoehx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gddflwbhd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gmnijynxo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gepleklhs.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gopdmphec.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gwtdornjj.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gmcyaxusy.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gwslmwgou.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gnbyioslk.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gaoaxlpwq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gygabopwo.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gfckqisls.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gvzzhikgb.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ghbujnekp.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gdiyvcmsg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvuviaxol.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/glithqtko.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gntwsnepy.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gehohavru.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/ghylvauoc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gzqdhaldh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gkghptzqx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gvzebnqix.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gbzdgscuu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/ggbwkmtve.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gtnpwevvd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gubqaqdcu.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/ggheqafan.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gwrrwxfeh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gqiigllbi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gigveugsw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/golxiunxj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnygmxfdd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/giidfvyhs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gjmzhlkur.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/goeevztcb.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gnzzizrqu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gwphfqsks.sHtML


<!-- 参考信息 -->