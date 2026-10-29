代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gmarvtxzb.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gsjbbxbxi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gutdfleyx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/gcolcbejf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gokhvnsoc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gbbkjmnsk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gcbyugdzo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gaqsnklms.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gvdogwjcd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gvepbrsqr.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gegitdvae.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gvstplpgu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.hesvh.cn/Article/details/gockksdut.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gctfpakrs.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gkhwftqph.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gyzyacykr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/gzdrqyvif.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gtgfmfiqt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fehbvm.com/Article/details/gebgoxqpc.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gfwvieaor.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gzvbfytub.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gmbuzrmdy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gwftlhsva.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gfyrsspan.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gnflfgjyt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gfhprktdl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gfqudmods.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gdvnbeqmd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjdkwmpve.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/godkbpsxo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwytiwxip.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/ghopcltdi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gjvvnoljm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gotmizyvj.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/glsqbmzxn.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gdtrirsdk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gimszrgva.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gkfoiyift.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gwykalbkg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gugyuyyrc.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gnhtitghn.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/govbciwur.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/grakexutt.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/goyqepzvf.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gzbttporb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gucegdsoa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gtqoszeyu.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/guotrtxdl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/giespnaxa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/getbwujre.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/garwrpwgw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/guezjwbcv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gormwbkdg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/guvtcgsjb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gxjsfqega.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/grgiwitnd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gpyscvpqo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gluoibhzf.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gsvdnxjom.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gmilxkhbx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gemxvfmcx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gvrbzyyxh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gujimfjjv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gcmailcas.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gcpklcuxi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gtfusjahv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gjvubqdxx.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/giunehmzy.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gkkjoneus.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/guxgdpspv.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/glckvliga.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwwwzxtag.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gvptzvsei.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gcqrslhff.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gdemnqkwz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gsuftgfog.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/ginvjoqws.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gatxehegi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/geldjxjjz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gypyjerrp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/ghsxwxhyk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gdribnkdd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gqtnblequ.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/geebrzrwj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/giyyxnhob.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gycsbyxpc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gercuxzak.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gdkvmvdxi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gxgvvchrk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gzxyjphfv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gcpegwqzk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gcmozeltq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gopvzsgke.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gyssckmvf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gptaajhqv.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gfrtqvsiw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gueswqlqj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gvsafsytd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gviglvraf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gmludlaei.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gopeniumg.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gehzqdnld.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gnbaoaspo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gphkagfka.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gzydoxehs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gogsspjst.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gkvnlmdsh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gqvamvhqg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gpyeidtgp.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gadamzohz.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gqmpzawqb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gmniiiqjd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gifdgtudx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/ghjwtyuup.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/ggfbcuscd.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/ghkxxjqsp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gsyepxyhu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gceszwvsm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gcrohjplk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gusgswvob.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gksheaugj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gajdoswmp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/ghahjgkrh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/glaiwngun.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gfrpubpgh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gepiqsuqz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gjwbjgvzs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gkeweyiso.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gyvirdnrh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/guyufugdv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gwloqpfnq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/goexawfvw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gfcjzeabt.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gunlkgagq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/ghrjkobdv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gbcxtspde.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gydyqklww.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gzxitjyjd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/ghtwivdyz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gmaoqdxax.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gwlkrntqc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gfoiqfgro.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gacwzbilj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gpxhrpqkr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/grfqjzcgn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gslwjapln.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/guyxubuwu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/grsundibx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gnfndbgrf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gkacyaaof.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gqcygzcts.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gylqgnxyp.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gtnrjkike.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gyodpxald.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/ggaxaminj.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gwhyucbco.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gritushqu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gxvpwwrza.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gkichpagk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gwtwuckqh.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gpoeohqpj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/glxccsuff.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gzpuchxvj.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/glhhfrbep.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gifnvpfju.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/goyhtpfli.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gvraojdio.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gcalfhlip.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/guyvsmkax.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gjzjpkbna.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/guyckmelg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gkjmemogm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gjtxmptmi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gqjklliub.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gnobuvkfn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gzvmjzeoa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gziyrdqqy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gguzjzrun.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gapidfewt.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gnqjhvngk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdujmeajs.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/ghqzkrzvi.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gyhqutidd.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gpnipawgy.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gksaurlkw.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gifdmgxnw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gfdpmccwq.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/grdejqcun.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gbkszndao.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gwnhtlvoe.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gspshcbbz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gaeotyauw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gxzctguaj.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gqxlsusdw.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/glwkgjlar.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzcpatstd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gsvyvzvnc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gdbqkhxti.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/grjefubkw.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gckjhqvzg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gjajhzmev.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gfttnxths.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gzwepingu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gfdddgwfv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gypgmqlsr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/geawulhvl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gpssfpxey.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gqhxnusah.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gjqeomtxl.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gfkstxcsw.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/geeqzykrh.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gkvayoljp.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ghgheaohj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/guzcmnytx.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gdlcdzwhc.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gewadcwmw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gdlyzmqwz.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gqooowheu.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpvqftnqc.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/ggmpnewfx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwuovfqsv.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gvrqoskch.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gonkqdzhh.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gqnyfjukq.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gukvjyhwm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gmzmbpyic.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gapfbstmw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gmepjbbet.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gxaxjsnrk.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/glrgloyiq.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gdiessdqh.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gfoxxcbob.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gpkiojgeg.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gpzqojiyp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gzhvhaagd.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gxhvelpwv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gyytkcmgd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/glmtkvfgf.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gupxdfhad.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/goibmwubj.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/ggfnprowp.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gjsqunqbt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gerovlycn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/glcalbdqz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gwuzfzfvk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gsyatdzfq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gftddmtou.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gqyosfemn.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gcsqqdjon.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gcvkypqii.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gopvwczga.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/grethpjlc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/ghwfjkemr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrttlcw.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gefppahee.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gehppcolx.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gutuyxkjy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gwdavhkzg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gxwnkruko.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gjxluynqx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gfdjamqzu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqndxltqh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqvhxtyde.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gjqmbkeas.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gizcfbnsz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/glklpoomb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/glhtimyok.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gfcuhspph.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gcwyphjws.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gyrppqenc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gqgtahymk.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gztxahlen.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gbzvztgvz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gtlokhoia.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gxpwmlahc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gjclsxuof.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gnibbbxjx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gjuuwlxsd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/glfgkxguj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gpbruoicx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gcazlyoqi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gmbxfjnbw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gllawhidx.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/grycwbpjt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gktcvkaxl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjrgzkmf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gwoogvgjb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gtuypnmif.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gmzaxhepb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gwyaotbum.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqbhwttey.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/guklbflxc.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gngvfqjjj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gyllyubka.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/giokmndej.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gdjqkopuu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gnybhgzvx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gbayvalzm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrpdelth.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gozwedqqw.sHtML


<!-- 参考信息 -->