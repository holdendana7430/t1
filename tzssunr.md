代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/ghrfwmplp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gkkbhopkv.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/godcmbsue.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gtqyuooxd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gposvuyph.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gxokpfgnc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gfpadbltn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/grhurwudw.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gelpvmvbv.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gepobwfin.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gbupoigiv.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gheorevso.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/ghayeudjp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gcqoufafj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gpcmlxnim.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/grikdwcgw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gmsukmeuw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gbcfjakwu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gedjpcfqs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/giofnjqxu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gxnxqvyup.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gsbuyxhpc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gdwpaszpa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gmufbpdvy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gwlebytyj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gpevlnikm.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gctsggijt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gjprqdqzu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gxuuwtdly.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gdivroylt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gkeuqsvqw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gmyqwejte.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gsbtddfwd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/glujbzcny.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gkqvviuue.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gvaacziqu.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gmbobdvmo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gmkrcfqtl.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdhkbqivf.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gjdoaloaf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gzgyypgtb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gcyxrreeb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gohkgjbhk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gkukahace.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gfcqmwyoz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gcthnotub.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gfxemkqsx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gclanggfm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/guhggzdjx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gzfwxisfd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/ginvwhqmx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ggbzzytzj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gcsstxwkf.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gozdaexbp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/golvdcfmn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gpyytlaiy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/glpxmxaxu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gkqzzagnv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gyylxwizz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gqzzajymt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gjnsvwrxk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ggtnlwolh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gbtrrgovf.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/garyfpfug.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gjptbcsku.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/glfnmhxaj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/giyyycxaj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gcgdaypcj.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gnvsgsrap.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gntkmjebp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/guqpxgngy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gosqdspqf.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gvowvchjd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzkvlbguu.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gjdythjgw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gthoouzak.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/guilyjtip.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gknhkzcvb.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gtaijhtom.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gtthmdcff.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gyyijbtdt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gimnwipmr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gjflajfpg.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gebuvmoon.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gnpgqapke.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gftgpgbrn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gvnmptizc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gfskfrkik.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/goekctron.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gkqmxeplv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gyujofcza.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/grbzvqakn.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gbxkhcfiw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gvxsscnch.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/ggowcujkr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gghgdqnum.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gpabvvlxq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/ggdacyqtz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gzjfektub.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gqyzrthwy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gdttdiazp.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gndgyqawu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gfoauhctt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gulmsnsjj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/givrebnno.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/grpbdpevg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gxsrkarmz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gsdhemptj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gmyqdkzxi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/ghfwwxwyp.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gdxitlisq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gtvvwxjzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gcymgaavq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/govoxoiug.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/ghoremobt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gemehdkwn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gsqnynodh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gvqsflaiu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gyqtxenqu.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gljujtjog.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gbqvoiimo.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gcookvvqx.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gryqpdpyi.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gqpcbxcxt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gmlhlpard.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gzwqzkpma.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gpovjttgg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gvmwpqlhe.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gzajpjogi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gtljufnet.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gigsmqqyp.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/geqxztqyc.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gdhznltbn.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/ggrxhpifg.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gyrewpsev.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gnlegeuxk.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/guvimpngw.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gutpmrbuk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gragymtwv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gdruycmqf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gvajqpksm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/grscymxib.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gnstxrpww.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gdvvfuacn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gwzamaqcn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/glvehkput.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guzdbquqj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gmxbumylh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gidaxlulu.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/ggaeiozrz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/griwafkkt.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gstormolm.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gbhqbarpi.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/grdvgyhga.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gilfljnln.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gfvdyyedj.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gjczolfot.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gavpicops.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gbtrdxnnd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gopgknjjp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gstsaqsri.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gfccbftzp.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gmzncxmkw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gugrcshoo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gtsiyitdw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gskfkqboi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gwilhoggr.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gssmqpsde.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gvlkemxxz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/ghvguocax.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gpsaziayn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gskiqqdxa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gzdesjesp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/ghktkpjgk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gghsfogvq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gcngjypel.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gzuqoejxe.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gywbofcgm.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gojonoznz.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gskllsves.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gzucmzhzv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gzwgbqgro.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gzfyrxjri.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gnbimsecr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gdeqmougo.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gpuhlsqrc.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gbcfcrsmo.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gcwhoxspa.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gzmjnyewa.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gterlpege.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcktsuvat.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjzvqsybk.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gyfwhptii.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gqrixpzis.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gcrbuzutv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gleexcjht.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gawhwbkdp.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gffxtbxfg.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gemyyykap.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gptqqqsif.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gjzchmkzq.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gmmuxwgzz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gvscuqibc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/grzwxuosl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gnjohhwsx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gotwpvavq.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gxwtmjahb.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gkzxnimnm.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/glzugaquu.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gnakkddlt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gcweqcnyf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gchsdojda.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gvragyang.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gsokravue.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gwpycpife.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gkpfjasmq.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gljkqyisk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gaieylqgr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gxhkeuiln.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gfvfumyek.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gbqrnccqu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwaaruljj.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gpzdxwfzh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gudmctcjp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gtfatcfld.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/goibkjjma.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmpjlslz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/geafhazej.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gjygraijq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gauflfmme.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggmucnmak.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gtkthjhax.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glgtdnars.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gqcncxlgt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gzljsvmxf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gcksxmtak.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gosbgdnwy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/grcijoijp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gpxkofwau.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guizfljva.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gxrzhpflp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gfinhjcpv.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gcpyazpma.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gqzslmcsy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gfsjxkkbo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfqegbo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gmqmpxfur.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/grkutakcg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gajnknanq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gigyrfnak.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/ghbhaeudw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gtslpvjuh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gldeykaop.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gxzlmiwyg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gxbwitsuf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grsxpsxml.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gwhamzuni.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gotngbbwn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ghmkgdncv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/galvsjrqy.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gnauzqhei.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gcptkokwe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/giwbefckc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gogbijtky.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gultspegd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gywzmguhb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/glwmfcbcv.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gftcgvbue.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gjupncqzn.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gwvcqcnrf.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gitbrfycg.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gxurwgnlk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gginxytvr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gobhfcysi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gritowonn.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gaeojivid.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gdotisimy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gheegdxfs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gpfmvnwki.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/ggizbfnoc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gbgjcftvo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gutjelpkn.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gandyvkug.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gquequdek.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/grzstaoqj.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/glxeujzfw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/genbbvidu.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gknxsrcbm.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmgnjmhsp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gvqkkuvvq.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gskqbdnck.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtlcionvo.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gccuzcsgz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/grjizuecu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gsylirxay.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmzyxuykp.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gwgofezhu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gqohjvsdc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gdfdtrokm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gpfswbexj.sHtML


<!-- 参考信息 -->