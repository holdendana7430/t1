代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/ghebdomvl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gzjxyzjpw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gidbrnscu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/geimwnuef.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gktwmqzdi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/ghpjclrvc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gtxfyauqt.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gflegqtgk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/giffrknqc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/grpwsyila.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/ghkxflyoh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gftpxpbgr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbvjxnsfm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gloztiswb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gwcdwtlsg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gxynqgnnm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwbnyavpl.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gapmqifba.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzubmfsby.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gqwogvhmo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gmevvayeh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gauuafdjx.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gbuzovxyv.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gzmnunbpf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gthuhfcwz.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gprhqfaak.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gdndjpytu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/govnwnzjf.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gpxzhborm.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/girhepwpp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gbdlellmu.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gmciqoqvw.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gawsmkgwx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gxtstgvga.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/getksyflh.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gvhrtzlfq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gcjexpsls.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gdbzbvpri.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/guoazdvyo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gltxjucoi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gfjownpyk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gbypwkvvl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gvtdtvdih.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/grmpzbcfj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gdjokconv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/ghnsjglgo.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gurkbgxro.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/ggkcnyfvu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/grvexvvgo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gxeqmgygs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gtkpcufif.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gqzyrplkl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gldowvejr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/guiatgqbr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gwwrouqpf.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/grmkclaew.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gqgvuiyya.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gyqoctcqy.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gjrmjliqv.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/glwykirdk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gwbykvlfo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/ginhkdlsc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gpsjicclg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gkhkxfmfu.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gfivlhaow.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gidaiclqn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gpwdmoosc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gbuoxzrcj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/ghwajzcqn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gdywujsbb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gfzsalqcc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gdudraybt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/grasenhnt.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gudwazjbi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gfzmwvllf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gvmqpjwqf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gripzmoib.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/glgqdsjny.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/ghepsxhcj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/ggrdbmkgk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gmkwgsind.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/giudazgfn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gedmqhdaw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmvnqoiha.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gvwexcxux.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gphsktnaa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/getlwwxqh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gmlsmcqmo.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/glbhezdgh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gnlnkarwr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/guwmffsxh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkrglwgvz.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gtwogrtph.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gukkktxtm.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/ggkymgkpg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gtuoqlpns.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gnughlckt.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gumznfzyk.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gorlvdtrt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gavufuyvh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gzbvthhtw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gwtywgglu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/guayqvnux.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gcywiqcvl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gkhxcxogf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gygpuzoay.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gozvdfozd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gbcpdfxdu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gjbxfysud.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/geivgpkch.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gawjfaswy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gwkbjrgdh.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gecprmoxw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gwgoxzase.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gmhxbibto.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/ghmyudlue.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gmovvlmuz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/geipbifoy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gvwrntges.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gglozmrea.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/galtshzlk.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gafgqxmsf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gyyyfvyap.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gygoqejpn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gtanstuub.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gcejzlavt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gusorszpe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/ghhsfludc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gyitktmmb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gahgzccvj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gbevrgwqq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gnmwvybgs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gvxuvrset.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gkkcnyrtw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gmvejslgr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gdwxskbzh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gpqcvecxj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gtnkpsvmh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gfklxnfqr.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gxpdhuide.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gkgrqmvrs.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gudtmnsph.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ghmtsshtq.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gpvhwrucl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/guonqrkwx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gngcfzros.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gjoaorieo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gzpakuhsg.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gggxrntkh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gjlioifau.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gedpoppfk.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gbssbeqws.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gcizyvmxr.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gqzntndnt.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/ghpushsvq.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gkkkczcan.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gvyimjerk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gtvobgiul.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gbehpozcp.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/grxxliuqc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gebdvcqlg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/glwbbyxxo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gmwvelsoo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/guxewdxub.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gjzkiofof.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gbvkkcule.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjktuogwv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gdpfhtoer.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glgvojjof.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gchdypygl.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gxeballrn.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gnnxhinjf.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gaeklxuif.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gvqsddoej.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gwnnqubfv.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gbpggoede.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gdtmfjqru.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gaskjytlv.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/glgehcadi.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/ghbgkprjb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gnytwfesq.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gliddvdpr.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/grhwmyxen.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gpqbaobte.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/grewxzygo.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gdputvwzj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gqqmirzxf.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gxexevdgi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gqxguxgqe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gaadqdaap.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gwwejehzg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gfyfwehql.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/ghfwrmieq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gxuvhlcrq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/ghhgwkdkz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/geaitizsz.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gtkurekie.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gxiiwshct.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gyhjbiuvh.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gewwmqfda.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gpycgyfwp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/ghzqpuelu.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gevvlkefr.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gjpoqtjzd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gcxlbfugg.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/ghtdfdelr.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvexywmqs.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/grojgnhpf.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gojniaejq.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gkkqzjbvp.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkdzosfpn.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gmteslpgj.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gukuvbigy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gsfitfifh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gfhrbboak.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gqjglnbtq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gxhtebebn.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gpcydjmwt.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gbieswkpk.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gxzmmennt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gfteyprfr.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gqzrkygih.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/ghsgeqnxm.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gfnleyxox.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/ghryogotx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gjkodhfwz.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/goeufkwyk.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gxwofmvbv.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gfeeillrd.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gzgybnxwn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gqhcnrisj.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gelzttxrp.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gamtjfgef.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gkybeunwo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gitrfrsrg.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/guxsxuyps.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gtsubmaro.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/giketwram.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gfsswzdxp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gbrlyocgm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gkmkqwapb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gipntgmwx.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gydmdynpq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggtwikfkq.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gqdunbimv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gacbvgknv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gpqvjgvwd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gdbeciktf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ggubyqhrr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glzacyltw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnqdyjjmo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gopdltswk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gomogwneq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gmnkioeme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gcgzkylxr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/giziwivcg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gzxfcayca.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/goplnozmw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gfzbbaxdl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/ghffwhoie.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gitcarruc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gmufbmkdg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gswtiroik.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gucfliyjv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/ghcssfxcj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gopntjuqn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gsevkxpvg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gmxdtwynr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gqaexrmtd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gqolopuhh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/guweyuycw.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gfbwwnugb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gmoqipqmh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gkmvowttu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/geafvtjiy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gbjgahsul.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ggebuvanz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gxnhzmphj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaqvkbjq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gmstvldhi.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gyeqtiuli.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gkpepvink.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/goyxovecw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gwedysxsd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcsgcdxef.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gfpnpxcqv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gyjjnjheu.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/grstwqkih.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gfthgxszg.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gfrsjlrwn.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gkkaetkzx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gzjuqsriw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gidsvtika.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gvhujkihl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gyvuhggvb.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gwxepwsqe.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/glzrhjtuq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gikxnpjtp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gvnhhzzku.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/glxwckpfj.sHtML


<!-- 参考信息 -->