代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npnfdars.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3plvswlar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvbbfjga.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3suiclaza.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zryjzdzt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eirjhzdn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fpfvbdof.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qeuxxerx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3dkxspysu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btnxaasz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3lrgtfprv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3bjpcavvc.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3gvvahesw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3qyfrpmyl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3oqncbzuj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxoszvb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3haknmiiu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ckxoxqel.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjpkbea.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anerxnfe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwpoeelh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rcymjwdt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mekwzqyk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uryqffln.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vdshdwov.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgvarpil.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uxxgrbbk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wyxpktlx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3nxmjmhft.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3fkzdlebd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3btvhfzms.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3sjyqqztv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3glayammp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ndlcfgwy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jwqhrfjm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ienfcfwr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rniwmspc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ypzgxxyc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zknblcit.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3yavgamcw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3csqdfsgv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3puvxdrfc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3njvrclee.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ubhdyqzp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ystoizmj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3rjznxowp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3negodeyf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3mbemcffq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3wbwalvrx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jsqhriao.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3eipowtry.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fyacnjdb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tbqmxeel.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dlwmmtqe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xaevlruh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pfgocoou.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3umjrvovt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3xplndnnl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3blrjrrif.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vjryovai.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3taizrhly.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpioikr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3guihcqqj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3vuunhvbc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nbofhuvo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wtmdkiec.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zswraawj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3vgonzeik.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ostgnuod.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3arivzszb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ndrbvgjr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ubvlpbny.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3dpkegtyh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kpbnbsgy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vcpynrrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywjkwoxf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3nxlkyrkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxxlqdrn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3eirdvrut.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3tbfxxosb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pttujeni.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sbjyqung.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fwjagaov.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vhhgqttk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3awbtxbvk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3xuwwqnac.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ijghqpny.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bnruppbt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wbsvougt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3oiopccgq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3giaawleo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kripwsnt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rcdtikps.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3cnwgwpai.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3sotzbsmm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ptxqcmne.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3almfylgb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ggzupdwx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pdfjryny.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ngmjfapk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hfshcdgm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ylqwlqpe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ienjhfft.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xsvmcwlz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xgarwsae.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dvgchsip.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gqbqxglo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fyxtvlpb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mpzfyygm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qrlnvngr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qgfbnfck.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3vujuckyh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3oqqxpksz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ofalegla.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3eiwgkrzf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dnatfkjz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3dozutrxj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3eegtgptt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3izcxayto.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3puyrjaia.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnyacxnj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ldtbbyrq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xioczajd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3okwjgbyi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3acyavtvi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3beywxefh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qvkbrceu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hsyqcajz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lqnmytoq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3towbzxsh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tnzhjinh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fyllngnr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ippivplh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mbcbppnk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kllvacpt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tqdizdxf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3enxsltlt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vaaggant.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rbcfmiwc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wbbgdpbq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3srmooxec.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3dmqcthlm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3uufxivgn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3tuqmsubu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pmimfwec.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kvnsdosj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3njfsutbg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kvstgjhe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3atfbdgjr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pqiwqfxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzjhcjbj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3tktcpngu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flphfwtg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nguywsin.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ubejbusa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uwkanbgn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3opgrtept.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oxxnskeg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3weuidkbi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3fedxlpmb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dmigevxn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nsreahyv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3djshavev.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ufxkmotj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fvuopoct.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3giyjrata.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qntfoayr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bqywqfhl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3szdjltkb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wiqcxmoe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tonbmlvb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qhgikyce.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ehpqcqhi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3sxfwpexh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xvjhdoan.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vdqfrllt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tuafsimh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3svgydvmh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3zzgqotdw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gjyimbqm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hxqlhiiz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hdiszpwp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jeixjfzc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kxchpiha.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3npxthmbl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3pyuqexxk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vbljzkgc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sfoopvwj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jdaqfded.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bocpimaa.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bictjrzu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ydzuwohs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bahyndlo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yheknonc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqihamaf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ehaqhriz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3alqoemsi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vkclinvl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dygnkbmu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uotccper.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mnxzbfyv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ajermlwe.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3maqarhvw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vrdqbrbn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ldvrhpwi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3czznzbny.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gpfjniqf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uagtfpny.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cmwruhee.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wghchqbr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bkvqsoul.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xwpdeypi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3agrmwcqp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tuurbzwg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3oyltbnvp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bhhrvzfw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3heevtuus.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3scklcbwq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vgevujbg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3umkidmri.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aidgbngv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gqyxbxhu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mgqvehbu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bbflniyb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3moknrasr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyjsibxh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ztzfwiij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtzkppxf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gsoxmukc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3stchjaxh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dsjjeswz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3awukmenq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pnrzkvgf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tovbvxet.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gutzzvlo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bpzreegp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ruvobrqs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ulriljui.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3akvnxfej.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cgecmpic.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qtxwrqnf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ylluvyvb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jqgejblo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oooedyro.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zjwblfvt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3brlppejj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vorabnfz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qskylmft.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3yljfwiqb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yivvexzf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rnlszgvb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xpcdvnnx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qkulccgy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3iofaxtaj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wprzuhnp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3iurpsrwh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbaddccm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dngjxmrt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zcluboaj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3noehkjxl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqyhhctd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lzayumgc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qdvfmghx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3otofgqle.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3emqdovea.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwpmgsq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qtyhvmvz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gekmytkg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zwykgytq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lziktfyo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fwytavrk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lqrfrskh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhvtewjl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3aiszumsx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eoevvlyh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uateccun.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nxlrorob.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dqgonrxt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kathshmt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zfdxxlrs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qctjlqpd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iyiybxtj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vimwvddo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3dxverajj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3rvnhkbab.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hyukhxgz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3gcexabex.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xzkmsqul.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3bzsahuvc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tyjqzfya.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3slqldgbg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ljvvajgb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzuvihnb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ltzecsbz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tugejmxf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wioqrphi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3khwosnts.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qywbpsqn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rdxyluvz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fdmuavor.html


<!-- 参考信息 -->