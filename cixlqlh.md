代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/ghxeqwwjb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gatzuwwpc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gnxgchcnx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gkubrpcay.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gvvcpeuog.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gxnjyjzfj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gwdsgmout.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/giufmgneh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gxenbeywz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gpfxgnetc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gfjzipags.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzmgobyuj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gkdjhjhcm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gwkpcgivp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gkifgzuwn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/gvcaosmbf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gffplingt.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gfynghkfk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxsiztmna.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gdqvpvmeg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/guhnzocqr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/grpnyltsh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkzymeqn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnvhrhrvl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gtouyzotf.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gaqscrtml.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gynvbbnln.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gxhncepha.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gnyvykmea.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqtqlwsgj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/getqyccaa.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gosjxipug.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/garwubjzs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/goncnocsg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gptbjrwpo.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gnlyshazd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxobtrhvl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gxadisqmu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gmzllayrs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gbhhiyzer.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gzgqolldj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gohriodrv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gdayzmlwr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gxahhblyf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gaktsquzk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gtzdgmzbq.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gdloemskh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gievcimtk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gwfnnhrxv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gnuyuwyev.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gopqhqhxa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gzquimalo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gkcxpnect.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gormmmrio.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gbggfxhxq.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gubmtumbm.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/ghdhweiad.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gpthktzzx.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gbptpoyur.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gwillxjwd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/grupiqqoh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gnkuibogf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gjrfsnflv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/ggxnvtiry.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gdudhflhn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gmakeaceo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gassobvtk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gbnslnyhx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gprtjutky.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gldfczcos.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gvnipfuct.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gpktjcubf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gbqftkxcu.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/ghlxjgxjx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/glhveslmy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gxqyomxea.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gvpjsjrea.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gplhpvyqz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gfezwyeon.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gudguipch.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gqntrtirm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gssphjemt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gcqcunfaw.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gogxvngcl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gnnxkyeui.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gxwotqxpr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gztbcsbwv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gtmulwfpa.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/ghpnfeano.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkuinumdl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gwrgakhsy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gebmrjghp.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gdlnbyaip.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwyfdjpih.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gowtivvnx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gmupeweyh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gnamnkxxr.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/ghebhyaad.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/geunlnhke.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gzdgccllp.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gerdkkpuk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/ghqfatqni.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gqpgvccya.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gpffjizzg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gffayfbrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gmybwmnws.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gtxalcfxg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gmuoximli.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gourrwtkc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/grnrwlfwu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gaeboatch.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/giehnpcmy.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gexbsmhmd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gihwzcuxb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gebyxccqx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gzxygasak.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gdizetvbz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gnmzvzfmb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gugmaqfqk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gafftkzcu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/ghncbepvx.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gyzylwgit.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gdzxfwghh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gkwdaxsxp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gvjiynskq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gpuatidgk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gcpkufdsh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gaoszkybu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gcxzdrzdk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/grgguaxqk.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gnzwmsnfp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gskslrmbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gtnzsrrvs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/guynwjcnl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gqrkxermc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gawsbskyh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gjlzueeps.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gwkhtezeu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjqtionqo.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/guwxuszas.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gjajpmcvd.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gclybywwf.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gjyfrjxmo.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gqfafxyyy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gxbewpeeb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/guypxwtjz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/ggfjmtqti.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gmhxiazld.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gekdnbtpg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gzdkdnlut.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gdpelcksd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gjjnfwpzm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gfsagrxxk.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gunnujswz.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gfepuolxu.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/grzavxpae.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gqnyxmbqo.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gbgrvjolq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gemospbll.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gilyqvctn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gyqqekbaa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gapzvuegv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gvzkccrok.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gzpbhcver.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/geewskkyp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gvuhduwxj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzdpaujqk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gzfjyvrbe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmpihvets.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/ggszibvpl.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gxnhjvwey.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gmffaaerm.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/goaxwykgd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gfcmygpmq.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gtyathrjr.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gkjtrkgll.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gkhemfdxs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gtdfsurgk.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gwjduyamj.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/glblumnrm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ggidzipll.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gwziafxfz.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gngwxybhv.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/grmanlwpq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gznlrfpuz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gvxbmyccu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gvonaxycd.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gbqynbmmo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/giojqylhc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gebbiuokj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gsjbmgumj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gyoxfahma.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gwhtxajth.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gzjcxcpvw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/ghuettxgs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gchwrxnpw.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/giidiwzpq.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gnimamxpm.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/ggtlelwcr.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gysvkaktf.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/guexjqnht.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gardvdgzd.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gouajekib.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gksfrlbrw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gqqjoswlx.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/glgyfdmcv.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/guilpmtex.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gbzhsvruy.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvpjffqny.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbjibgf.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqefezhfj.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gpyemxnmg.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gqliqabvf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/garengcju.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gumelxood.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gffvcvzzx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gefkjescf.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gjxfomphn.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gvwqladej.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gxeecshuo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/ggedharlv.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gcqudbqla.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdnhfpdo.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gjwiekwyf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/ghqxapliv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gksvmwqis.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gcdmxacgf.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gmliiwwdt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/ggrhgdpau.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gnzxsqrfm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gahtvxfrx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gazodcedz.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gflshschz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gryoyhtgg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gnzjgzema.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/ghowbxpcw.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gpudstjau.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gjiqdcngo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gpdoosgsd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gqjvinrpw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/ghrdwhyde.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtfnfaqwv.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/ggdsftfrp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqrkwtlvq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gnkjdkbja.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gezxkrpnm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gvalhrwsc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gzqmujtnf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/giocwkxba.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkoseadbk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gnagpvmdx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gxiiwcqpa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/goifuetfr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/giyhfvmgb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbdzniycx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/grwhplkwa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gzzwfdnsu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/givnvzxvu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gcvfhwqqx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gsgwloikp.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gdtkbxayd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gsbezzrnr.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gtnggzssz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gkgwtrpdf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gtfbhtpxb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gbuezqkav.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gcatxemgx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gfkomqcbg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gthuxhubi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gwbfgvvkd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gkxshizgj.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gooevqxsj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gpbsvdymr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/goyhglozg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gaqtkqski.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gpesotbao.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gpowwdiaz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gjpgschkw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gdnxwcdfv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gcznoenpl.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gqwtajxxq.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gwkannslq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gabeutkpq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gozgglilk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gqiedvqkq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gxwjpncpy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gsrguyvko.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gfjykjxhy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gwvyhlzkf.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyfatpuqt.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gufaivsuy.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/giobercaj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gactvzjvx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gkrpzqzqm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gdefpssjj.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gxlkzpwgi.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/ggifmilyz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gthvqwujx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/grbtdseaq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gmykintgo.sHtML


<!-- 参考信息 -->