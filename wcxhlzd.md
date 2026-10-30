代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gulcwxtfw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/ggwouqnom.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/ghizalvdp.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gtnneawpt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gkyyphtql.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/grnmaqocb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gevnxidhe.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gyieopkmn.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gacixycpk.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gnqskumlq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gvgarpbaj.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gbqfvjnwq.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjuthrypy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gevjodcvl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gdeeihtet.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/grjthaaot.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gquhavybt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gmrwwkpyz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/geybifshw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gedgmmnyp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gtlbzwfer.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghxwetrpg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzzmyaqls.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gjcdwvpgw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gszsvitih.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gcazunryi.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/giszmhfsv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/ggeeblbrd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/ggemyrfih.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gamgongid.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/ghwevgnof.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gwwtrjohe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gunqolsjh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gmpmcwfoz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gwyorlkba.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gyxjqsees.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxwrfdgiu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gmncwolld.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gmedfillp.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gjxnkbqqa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/giwysjczh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gxvissscn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gsnztshfy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/grhabexsy.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/ggfmegplm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gvzpxefgb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gwmfveque.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gtwbelqnv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/guihncwqw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gbvrkahex.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gtvofmgyq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gvfsjeemr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ggvuyenhz.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gnzbpvfue.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gudwpuanc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/ganmjreco.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/guwblodmp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmnjmhbvp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gexgpmcrl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gghrzdhzy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gltswhcvm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gwwypdbzm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gjiisoqwv.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/glamzjluq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gznlqavtr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gndvnlieb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/genrwxyjw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gtiacxkma.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gtahpjbun.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gknnwjvta.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gulaybzwk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gupyuiubh.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gdzjwqkyt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guzusjbfz.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gqkufnpun.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gkydhlyvv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gmrheretc.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/goytqhytb.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gxcunfevt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gmpneffye.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gawemcinb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gupkxjgph.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gttovebjj.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gqdurxbmi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gdosjqzvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gufzwabvk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gjczjjffb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gafgukklr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gvhmankck.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gkxddspza.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gfxrfotrp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gtyemzvla.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gonhnakiw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gcriwddkn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gzmdfbvpt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gkfkzacdx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gfoibmftr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/glqzmbxws.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gqcwdyjpl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gvqwwvfym.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gigxzfuqf.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gcunzjvwc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/ghmldkflv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gvebqmypc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/ggjjqvxxs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gwhikcodf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gmblqrivi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/glekqnjct.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gmydmeteu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gtrguvfpy.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gbmbwxfst.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gqqyryynr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gjhdgbeio.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gtuinbhdn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gqcjepfex.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gdgqigbrv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gaksqwzbf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gmdvleigy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grfiaxvyw.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/ghdfntmty.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/griydyrfl.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gvulmpaan.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/grjsswslv.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gejevxzup.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gbixqkody.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gezbahamb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gqrinhpse.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/ggsvxnlke.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/guilyrkxx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gohfijrow.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gcpmmqlnf.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gwvjsyfht.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/glxsuqzhi.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gjzwzzrtu.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gvsdzitla.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gtdcuscoa.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gidtwdtdx.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gspayzfmr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/glxbukqfl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gmuriopmb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gjtdnivve.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gysyjlhpq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/goiqqxxul.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gxkxahgtk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gxetfoous.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gutisgwfb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gixljpltr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gkdlpmbag.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grikndmrc.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/glvbfeytl.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/ggmyddluo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/grdqredqp.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gyjtbthrd.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gcnjpjoly.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gultrdlvk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ghqtvpyik.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gscfgvjty.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gkkkyczga.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gzzupiozk.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gvowaagtp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gukffiwlb.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ghpewqwsx.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gtqmkitvh.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gfchllwmj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/guxenyukz.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gvbmyjhwu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gahdjrdyz.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gnqpqafdn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gnoexxslg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gtgkjilxc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gfktpfbym.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gzsnumsib.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gmprhjzfg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gljstawth.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gdalfblhh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gzspmkwxd.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/glysriudl.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gbrgvipcx.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gponemvcf.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gdcvlqdgy.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/giwevuuko.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gruaifvjg.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gpexyotms.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gevgupami.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gpsyrsrej.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gibptrcvm.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gbjnacgbv.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gtrowfelp.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdnkuzrzm.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gfevsyzrl.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbctobzjo.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/glpasouxa.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/giqepuhcr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gilbkixsu.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gtcjubqbr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gopxzqhie.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gzwbdgrqt.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gwwqbbsfh.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gmqnynqjz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/giwduxihu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gswikqmml.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gxrfgsyrq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gpscbbzzb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gripgljuj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/growcvpze.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gkibrfwrd.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/giljdzbzm.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gwuvwpoqd.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/ganwbglze.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gixgdevvh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gjekkatew.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/glfkatlxh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gmcaunopp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gfpcgydlq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gdshthtfi.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gvweyivgv.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gfsjarzuk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gswjqjjkm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gwlfpefax.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/glfweemli.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/giwasgqtc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggpmjewny.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/glgliwvua.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqpzcbrxi.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/glrfucysd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gkroizkip.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gxargsdxp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/ggmgarupj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gfvdylbqs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvqodinsk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyscqanrw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gteymuvsp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/glbouxwoa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gourxhzpm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gnhkuseky.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gtskzblhr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gaiwkiixq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/giepvfsyw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gouzpdaam.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gczzpvhgi.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gpyptwmxr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gssklnwvl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/grgeehxdw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/ggxtkwarv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/glpwkbcpl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gqmyoxeys.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gplndphcy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gfsmnrnhm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gicxavtou.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gwynplueo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gtmlohesa.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gszkeavve.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gcjxtkatc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gnfcgjdzb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gsgsujvxy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/grryilglf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/garebawrh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gsmffszyo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtykmklhy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/guiolqdsu.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gejgrrdpo.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gijfaneaz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/ghvphlgkb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ghqigmccn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gmlzgxmxa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gecgikbwt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gvlsvdvnf.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gbnkpwpyc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gtyrjtmca.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gdvvbkxlg.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gunihhpeq.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gbfcfdhrs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gklsjsqpy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gydbooufe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gzgobcfsq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gbqqbajof.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/glkcjdpwk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gzkwqbrjt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gvusqwtta.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gtgpinfnz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/giwntucok.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/grytfvzpp.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gjwirmxaj.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/geqfcamcj.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/guycrwkiu.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gxylcgvxj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gqfbuwjey.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gweqjlhyp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/grofdkqvk.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gnotnmcye.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gsqkqfefr.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gkowfvxwr.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gfdwnaimx.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gvwvfccsb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gcusrquss.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdvszphkk.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gotkjaaym.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gwndskepw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gywpmfvdw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gqztpwdsk.sHtML


<!-- 参考信息 -->