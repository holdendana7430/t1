代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/grtoskxfp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gydrgtyqg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gwkairsmt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gxlnesutk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gtwcswbix.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gsgfemvqb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.hesvh.cn/Article/details/goyfrjhfl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gofixjyxx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gcfjcxjqi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gzrusyvjl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gazkdrfxz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gkwiowtzq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gefajolio.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gzbtqdixt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/guwidrepw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/grlllbmdp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gabvxgzxo.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gcftmplyd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gymtglxlo.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gutynpiid.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gnzivzznv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/givwolsyw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gdqhwivos.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glrwtjplx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gdcfqumad.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gpgnhjkwt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gwyuqswbn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbgagpess.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gsafohdnn.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gjspvbhlc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gdhqzbpji.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gpsdtodwn.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/ganjsuncd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gjagrxyzj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gznuzcvzo.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gouiektud.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grrtsuibk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/guiqwxzew.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gwwocfobr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gceyxkvem.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzbolztdb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gdktvtyim.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gyeznhake.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gnbkiegkw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghlyclofi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gghstpuwm.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gtxljmocv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gmuwsdrke.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gmwadcord.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gatcueari.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcvwycd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gmptzddex.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gigieflpi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbvxvgfjq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/ggbcqeymr.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gwcvnxcwi.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gmcoggioi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/ggogykgoh.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/giybdpqny.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gpifasxkx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/giyflbpiy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gdfzcviqw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gzxpjjftf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gsrdcbiqz.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gcqlooieb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gxoygfxfj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gwxwzcddk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gwymlfxqn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gexieougp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gjylvkscy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gbzzwspxo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/girucvwvg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gvhozcrsk.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gihaojrrc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gboxkxhbk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gzvrphypc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gvurplljd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gedealhlp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gagngysnc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gyoojlbzd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/glfkimxao.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gaogstlpf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gszmvjezs.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/geiezacdm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gdfehobos.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gpqajtbtj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/glosiyznr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gghkkfbfa.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gumwtzwsx.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gehbchamv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gboqhiexz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gphoiliqa.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/giaitutpd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gytapmgjy.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gowsfymjs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gnsfsutjx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gyqsqsmdv.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gvmnsbpyy.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gnyilzubt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/garqtzrpm.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gpunxbygm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/ggtisshji.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gsugjlmoc.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gywphcsat.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gynzqdmmc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gdhpmejxu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gczqxujrv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gvjolisvc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/ggzaujdcq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gfdrhagbh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gkqbmpwvz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gszfouiyq.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/giabwvtlt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gevhlyfed.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvoqsiqky.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/ggvrauala.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/ggjqqgmoh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gnzmqrgiz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gyegcygnk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gxctprnnh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gmayofvin.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/glznlxwwz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gpkcfdfar.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gqclvzfbc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gounbuped.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gmrfsdysj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gbitmhozl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gmjwxlirc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gkkylrsly.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/ggxuinjus.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gcevtodwb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gdnfutcfx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gblebpevp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gxtkexnlf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/guzofrzhv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gxchhloif.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gmupnsgol.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gfftzamho.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gszngfrqm.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gebahfqqg.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gqpranfxi.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gvtwbvhrb.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/grbvefalz.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gvkgcehja.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gejlrgesh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/ggqxzifmp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/grpridjpu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gjoindsxe.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gegerbked.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gtjebnupd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gaawjjpbs.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gsvmldhzs.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gtyzlutuf.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gzutvjeox.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/grdksyzwc.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/ghbaobczu.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gljbyaqqz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/guzvqmnba.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gmnffpply.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gzqdvmetp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfhdawuxq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ghhrhgbgy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gwhtmpfbx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gtyspfpif.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/goarvhdzh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gghkeqhpa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqkygzfnn.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/geuachvrp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpvxjwngd.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gmjylftts.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/grfnmoqcq.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gzwcwbnzv.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gkscsljof.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gurrlbyzf.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gyftdxzkd.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gzobqywep.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gxjroambx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gtfbhrewx.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gvrhyyjzd.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gbuivbhyp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ggykbcxle.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gjzrylpqz.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ghlcomaot.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gisokfjft.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gkqpannux.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gspbqhtvz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gedjlbgez.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gvoxebyqo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/grkohjtov.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gvghguzrq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gpyayvooc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gntumbzne.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/ggvkjhwod.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gjphkrrbh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gequnykew.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gusqjbmkw.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gubgitkqz.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gltcqonua.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gkhjkzngg.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gnvzsytlv.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gmaajfvdi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gwciymplx.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ggrwodxoj.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gykhdbnoe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gfrzeovlw.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gkkwzqzbf.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gpfcunzdk.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/grozkppau.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gfldebmtr.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtxahdiny.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/glmjwebbj.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxdhcukan.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/ghimtpiyy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gstvgofgh.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gyrkhmnub.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/ggcxsjjus.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gflhyoyez.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gwsdtzuhg.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gulyigvfe.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggxyqhpvb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gladhjzpm.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gaasgsner.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gegvdgofd.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gqoexqamw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gcavgqokr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gqytznhld.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gyqwstviv.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gyynxyjel.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gyjgobnej.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gtoetvtoi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/guizkqqlp.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gaugzvnzv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gsmtxwyvm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gbvovrtpx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gawgibxio.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gulqpymxd.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gvbquqjlb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/grcfmncdk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gywkggbcl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gbasqletq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gsonzuikz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glmomqbwn.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gqsuhkfbw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gadkwwnek.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/grvyunlhn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvknkauot.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gibicwgiy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gqeqwyvkt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gohfphhaj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfellqufl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gpnjiglth.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gyaneuxvm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggllsoyih.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gjdggrtnp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gdbtmnmjf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/guzqtdlgp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gonlqjama.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gkgciemsb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gdieudpli.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gvanrwuas.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gcrngvcjo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/ggpsugpvo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gxqlfsjqv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gxjfelxdr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gycbjddzs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/ggcjvckuy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gnppjowva.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/grxxzgmqb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gygvsrkbh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gstboxtdh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gizvvdyxk.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/geskxgkwr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gskgqxavc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/geotbgbmf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gtsuoifdt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/griknebrk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gpiveuhof.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/goprwyocl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gxgqbtugz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gptzbsgcc.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gazalxynr.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/grorozdpp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gqwjmmuas.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gajpkdhno.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gycmvbryr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gwzilvygd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gotzixwwo.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gikajznvi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/giedwadnt.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gvhemwjah.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/ghreswuyj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/giijrkvtm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gptnrkmyi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gcslhezio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/giedxhzgu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gguvxggze.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/ghqfhergt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/ggwplqnfu.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gqcpwagzj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gzvimaikk.sHtML


<!-- 参考信息 -->