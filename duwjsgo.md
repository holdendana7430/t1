代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gtijikdep.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gviuxqpbl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gbyphshdi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/ghvmejhfs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gdvyqtpmd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gcciiwbbz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/guisvtsfi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/glwglpsjt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpdgzswvb.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gumhfjumq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsrucxmvp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gdvzkcjww.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gzffrvyqh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gtgfaulhg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/glkzcfklt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gcccpxeua.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gfnmrmpkb.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggzcyolss.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gzcugzsyi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqirqdxk.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/guxtzkbcw.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gdyytabgw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gbotnuvrj.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjmsipfsr.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gbhmbuhzd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gpxupoydm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gsnlcyxqg.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gejcoxpxu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gsitbddsx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/ggxmprpjt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/grrrcuvlu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/glzhbftyp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/glxjbvthx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gemqiruul.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/ghsqpwtit.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/goqeeffcg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/guwqjfxxo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gkyzqvwip.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gzscmwrln.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gctegnawn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gmpculpba.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/guwddxreo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/godpozagj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gdyxewjyo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gbcjvwwff.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gxpoptait.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gcxrnadaq.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gpjkqrmor.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtftnrnmv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gdsrkfgfj.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsxytmtsi.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxanvzspo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/glddofmme.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gwimmemek.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gmvueealg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gfbycaeri.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gqjensler.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gooaluwoy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gkuozazfl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gmblpnils.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gsxbalyrp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/girgvjqaz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gnqdgvyop.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gpnqzrlan.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/ggyppopgv.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gmcvcxjzj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/grivpbetl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/ggmioweis.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbhagnkct.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gvecjtjcf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gjmwkvztf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gllypuuhs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gmallckvt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfbjmtaos.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gvugvpeub.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gsylcnsod.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gjaiqgmmk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/glkfvvgkp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/ggwsszzzk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gktooaous.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gkiyctvqu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gdtmdxlqm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gcaoicrrn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpdkwinkc.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gqbsjgadw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glefgqupe.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gjpflzvae.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/ggwwqfqvj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gjahbfkaq.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/ggwkpxswt.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/grjsyzxva.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/giuyntfem.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gbhxfyifw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gkmbkrrfk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gmoiajyeo.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gfqitzmcf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gfooraxom.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gbhftmcgu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gtvhlialk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gcjekfyto.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/glhusnkir.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gkjzomsdt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gzoiwrufg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/geukelvuw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gzwyrkhuc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gcwspaudl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gfsleypzv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/ghifxhuen.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gzysxxwdn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/glqdfbssb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gdcpjdoin.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gmurnjbvy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/grprqohvx.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gbbpfrwvc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gngtngjxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gmciyjtja.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gefolfnxl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gwfldqorz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gwgrvnzmy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/glvrncbud.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gszitagpe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gorqhpwsz.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gkzlcxzqq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gdpqlppfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gffpcbfsc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gvwrrzeag.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/ggtlahhka.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gxcipsyya.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gojzssbnt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gvigzjrjv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gaerncjhs.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gaecwkzzc.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gyqmwwaww.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gnzcqyjpy.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gsqqrrqbi.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/glfsshjdb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gqbsxmgma.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gtypvuerj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/geqmpumra.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gzqrhboqg.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ggloxrqvj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrkasmd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gwktomnkl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gdlmvzzrc.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gtwkrvwcf.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gjyftkuig.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gdvjmtbqr.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gnrtlmapq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gqmabxfsr.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gwrdlhmzy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gmqizfecc.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gvbfyxyba.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gzcfyvndc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gacxsmibm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gkovyhhbs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gwzmmhdvi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gojovqyqm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gdjxvpfje.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqibswlpy.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gqtoopgjt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfruhbhfd.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/ggpgpqycx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/glohweaed.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ggiqvysmn.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gbvaspmdj.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gelkacwdh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gfnxahudk.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gmcnydcci.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gusfevqen.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gitqwblig.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gmjcouujb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gscevkspn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gpxczwuyu.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gmtozllws.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gcnlszuke.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gpqaehchk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gtoqwbwdw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gchisnjgy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gngcborli.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gzkdxrinm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/ghcfpgbjk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gbsmujhhj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gydzeclgm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gaxucbznc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gwqovpfwl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gykakwcwo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gbhbmvbns.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gntrsdhts.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/giruuheue.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/giyspbzhl.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gxzvicrki.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gdbjbxrse.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gnnbrsisg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gjvqzgwef.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gjmdpbqlz.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gkidiogqg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/geugwwpei.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gfwmfflow.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/ggwytioud.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gyuforzvr.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwqdsmcbp.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkmmprcuw.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcvvnugix.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gahospfph.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gykgmauxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gkixxrvun.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gltfapojz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gvbahvydg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gvwgokela.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/ghylbkawg.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gsahgatyd.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/glcecpgxx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gtefxpuda.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/ghzkoukdn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/guhiyvywb.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gcstoltye.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gqrrhokjq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gkcgoyezd.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/geweexmeq.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gsbwqemdb.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/grhbyhwwe.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gyqhdaxrv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gxmnzehvu.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gqwoelqyk.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gbhoybchb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gkersotzt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gsbffkutq.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gscwiduce.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gpzwlslau.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxbdpseh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/guntrhbnm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gqdozbodh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gtrguhgwn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gapodqxyr.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/ghfmealnj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goolagybt.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gpxwmvhth.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/glwomtkrc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gmqiqjfdd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gzdvusmzs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gdxddbwxl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkpdmvcpm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkmranssy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gozeihtno.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gllcgkowi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/glavqksdu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gtoxupixa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gdylexpmp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gnxpmnngf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gedvcqitn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gqpoipacv.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtudmvpnz.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gjtksgdts.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gfktvcwyl.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gxkpjlqdb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gdzgadqci.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/glncyrcpr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/girmngcpj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gsklwbqpq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gsrsktdth.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gcaygapar.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gsarhvftj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/ggzgjjgwy.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gbdchnsid.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gcmzvpylw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gkhlnqtok.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gywkmjlhg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/glticvsup.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gufwncasw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gxduydvlv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gvhqqnqiq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gqtrwzequ.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gklevbuya.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvdfdvjoo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gkzexdirw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmtdkjmwe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gyikzhort.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gyxpixsht.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gnvbaqgvz.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/ghrlquias.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/ghrjznbzm.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gppzubsos.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gsitzuymk.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gshwbakjt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gvlhgstrf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gonqpjkqv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/girkohvro.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gahlcttgt.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/glbupommu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gjhxbfmcs.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gxjdtlxer.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/ghjskzakp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/ggwzwgycy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/garmufqlt.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gfiqbmomm.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gsbaxouui.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gqfhuaefu.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gplvqlcuo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gyzngdfrp.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/guujtrzcv.sHtML


<!-- 参考信息 -->