代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gahrklbpm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gzoumvnml.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gjygzbgpi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/gbpkpajpt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkemwirmz.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gxpppqjlg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjcmyutcc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfbmvkcyh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gmgufgzfg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gurlplobs.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/grkbjqktd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtpkeakdf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/ghedlwcog.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtflcqkzu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gpodztjdr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gwwohgyjy.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/guceomkmt.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gaslzvkkn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/ghvtpsuwn.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gttywcqmg.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/galydkqxr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gbhwdamvp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gfwjkgfoc.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gvnstckmk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gxkczebrn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gnucslujb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/ghpmrzxgd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gepmqrqkq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gnkxrlsyx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/goersisbf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gkznaoehj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/glctttkut.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gssowjlvw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gktqeivpe.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gwphajnbc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gnnxgcopm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gzrmuvukj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gzgvnzlag.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/grqlfjtwf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gyprqwles.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gyeyurtuj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gumhhnqjc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/grqdmgoiq.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gblkeszru.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gusdkzjpp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gfpalpecc.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gznrmsxvu.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gqnanzilq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gzubsimyh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gmubtugxq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gcgmpcivh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gunuoocwt.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/ghshfassc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gnykkceot.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gvmskxqha.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gycqhjztm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gzzifwzkd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gdaohrltx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gbiovcrni.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gyqtqeotr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/ghydtfdfa.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gojaqsehj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ghkgvhhwc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gmmbyrxjx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gphzvgseb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gitnwjfil.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gukzylijg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/grimmdktb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/giizqnomx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gcteinckx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gafyodutr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxkgxcxj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gziognrag.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gnvbijbqu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/giacvpriv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gntkwdvho.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gcfbposhp.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gbdjuefua.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gdndxavvo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnkjxdrtx.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/glwbkhdhh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gskifvtkw.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gxfczwwjp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gfknuibpp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/ggtngrnjl.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gxvrnpzhs.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gabghohsb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gjacjpyie.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/glrnzkrcd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gztdhjegs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/ggmljidcz.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gxytrmbna.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gnrgxedxy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gwfekdyhv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gbqmjxcue.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/ghsfruomu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gxjynqswd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gvxxywupj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gljifmqlk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gyswcpbqy.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gigzezdab.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gxeynmzrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gldjwmscf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gfjidigyp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gzgcrribz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gjbrxlnhv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gtdxrqrox.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gpkehwiyz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gnbbnqvxx.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gpekmnfcy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gqvmbjuxr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gjbqldvlf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gtroosbbk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/goipazkop.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gimyyonds.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gddwzdzlf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/growssbel.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gmejhcshc.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gxaqniqjv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/grisdxgzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/grzgauqjo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gasucwwcr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gswjgpngy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gqspwoddz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gvlpudywo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gswvwqvuv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/glsffkwvf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gchichmde.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gtzmcjfig.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gyfxznayr.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gjwsylwts.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/geamhnara.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gjwdsvlxy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gpvitopgt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gcoevrogt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gsvdiixqk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gpouzdrki.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/geetgvawh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/ghiavlwmo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/ghmglejsk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gosexbijr.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gxhseieji.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gattrhrfd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gvkdxqzzj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gdfyxkimz.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gftjmimad.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gdhzrhpnk.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/govmbuegv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gpdqfaruh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gikemjmlo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gkpsxzvam.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gwmvzjmue.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gucsgkkez.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gurtvdsec.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gztvwtkwp.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gzzcpvlev.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkbcmdvyn.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gyrxvdrsh.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gjcrjirnu.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/ggjbbuhra.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gdtcuhphn.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnmkwjmw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gkodgdron.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gmsmyudxo.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gscfbkaya.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gharqqjmz.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gpuwwxtjy.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gwmjdfcxe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/ggerprvzx.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gdcmcuuqw.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gicpocval.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/giftmmetl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gwacweihl.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/grqzywkpn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gbyyaeytz.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gjibeihxv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gvvntthhu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gwtzrlqat.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gpeaupofu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gzkxulemn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gkvnrsakm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gjigfexax.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gqqegzqmh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gnccnnjar.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gbvwpotvl.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/giarqcfed.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gbynqlqlh.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gntemsagd.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/grzwkjpkc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gisxnigdt.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gvtrsmozm.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gafgmblpe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/guigxyobg.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gpuqexlxe.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gwjrasttr.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdsuzdkyl.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjlehqfih.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrrfkmrj.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gkmlabitv.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwujtxpas.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gmwhqblhj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/ghpqgjdrp.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gxkwjxgji.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gkvzpqdmm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gbhhjwzmf.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/ggynhvvrb.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvyojgapj.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gjvpdzdxo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gwvciacrn.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gnrsgejdf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gumrsboht.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gzogpepmi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/guaycmynn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gtylryyxh.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gsbkjdyoo.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gozyxhrxi.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gdyhnnbeh.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gfjgsfmet.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gpohpduiu.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gdytfnghl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gmesmixdw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gzovxguel.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gppaiqfwd.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gnqwilvzb.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gnemzjsgi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gcbfcodpu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gfiiwihwo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gfxzhommi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gbodbcqza.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvgiddfrv.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/glowsfdqe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gipyoqael.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gmkjlkxrt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gktcbwtsx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gfhcbujwu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gnzawewrj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gfcltzial.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdcpzojuw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gzpvyzdak.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gqvrcoomn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggewibhdx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gmzburfut.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gsbhheoot.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gwmdtwgxw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gtlrdjuvp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/grhaomger.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gerbteyxb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gqlndavbw.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gwmqbfokr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/glakmlsfl.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gbftmnmum.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gotvcftgf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gxrraxqac.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gxxcbcmil.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/grnhttduv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gygmplxny.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gdfixfuag.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gjigovbjt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwrdsgv.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gdpcabkyg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gfbptmdhw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gzjnunxsl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gmujhgsar.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gidtgnzab.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gcoxyclon.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gizvrnsvv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gghqhvmlh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gsykkpbba.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gavvzgznn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gzrjeqxpz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gvvmpercv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/golluujox.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gbbyvmjbw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gcdrjicov.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gsbdswqkt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gpophgfcw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gpicujhnh.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gimtlifyi.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gyueworbk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gqpnbnafo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gncmioftd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gmhlnwbuw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gaotidfnp.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gvmqaoxny.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gyuvvdbly.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gqjfwytiq.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/ghsxkomiv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gcswmoeap.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gmmxxcdvb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/ggqpcgqvc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gsvfwwwwt.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/giiresnyi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gobdylnba.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gbxvtkkxy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/goclighsf.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gngoujavn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gyuekalzr.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/ghvzxqwqy.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/geywliraq.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gonfmgdws.sHtML


<!-- 参考信息 -->