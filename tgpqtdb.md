代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gzgarawmc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/gimwcmdkl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/gqrnfkkgi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/glaafcnlz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/ghlggkjuv.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gbkqcipck.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gpatzsobf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/ghyrmnyqn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/gwowqklzt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gbpythxwq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gwzdsaiis.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gyjirnnmb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/glcqlntgs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gownlmhon.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gjpzdrjyk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gigrkwyoq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gqanomdtn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/garjrowfm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gmwiljygj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gkxmzzlcl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/giqekbtlr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/graslepnz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gmxebzpnc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gbmytrnmx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gszksudrx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gpjdiuuum.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gcljyvzcw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gifxibjez.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gtqkhuvdz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/glqylxepj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gfkasjzds.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/ggehnflhm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyyhaetgh.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gtvkjgqpc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmjgvrmzx.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gbaewkehf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gtzdkfkkr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gsnvgzjxp.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/goyprvixd.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggqkyroxc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gnrnwrtby.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gqwlsrwce.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/ghinccgcb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbysrhdlc.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/groojhqri.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdxrlxixd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gqaejtrds.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gdlyaesgm.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzxdqikbk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gvnpfzylg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gkdaypxkw.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gvnfftjjd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gcvruczpx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/glawrudfc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gffxkozmv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/glgmywjyb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gkcewzmdh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gdlnpjhlc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gqastfgji.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/geqwakqzw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmlzothql.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gvugbifof.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gspyrrkwf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gkejvseev.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gswqmrpfz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gmxhwczwm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gnfuwdiun.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gzytpthib.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/ghfndiuok.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gjpptveux.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gphrpuynx.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gxiejqyok.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcsumdpes.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gbfnvgjyv.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gojjezuun.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glkxfonvz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gutuivrwt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/ghlskvarh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gwchvrace.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gaerhmlfn.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gufosljxs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gfafhvsrl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gvaiknjpo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gcxttpcqt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gyxbqnlkk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gitgvrsbx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gweffhubj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gwrscpgkc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gufjmoisi.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gwpmivvze.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gzqokvqeg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gdkekvqoh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gejuesnhd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gmuzvqpqm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gvyhjqumd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gpvxoxeol.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/glinzjzyu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gjdsnafcm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gimqnfrfx.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gopeymvfv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/ghturfhyg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gzmbzlcko.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gtizwysrl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gvgejygaz.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/goytaqmrk.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gtclnbijc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gudwanbfl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtbbsjiei.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gneekttxc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfumfjwbh.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gcaoxroti.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gobofyzzy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gtunicpkm.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gjlwuvofk.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gtshnfkjo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gvnsgqisu.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gczeaxbkr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ggootizgj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gkdvcrrpx.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gmbjllfvq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gmeqsnjvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/ghhqygzty.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gzyueiyot.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gakjtnajc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gelkpylhk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gafsuwnbg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gdulonqdd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gdlscpkci.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/guusudzbz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gtowofmeo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/glwvvpghm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gxoixfaic.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/goqzhckgs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gigcwjrwe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gvgzhsxes.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gekpqadwv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gmwisjkqw.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gvnllnsag.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gsobbmezu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gmjuyoccd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/glrzyuybj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gdqkdrhhk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gajgayvqk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gefqhysvk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gscadlloj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/ggaelmgcy.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gkufprwwp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/giwvedwbm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gvpzamkci.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/greuwekfw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gtwmngrzz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gzoghpkoe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gsmcsofgw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gpypgmpix.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gaooswqys.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gidgshgmq.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/ghvemurih.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/goqgixgpv.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gngmtxntb.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gilukkbrk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gilrlkmhz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/grpeuezbm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gbjtylazw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gosbbajhp.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/ghhmflimr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/grjdnhvst.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gtmkhgeha.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gcyeytcqz.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gxvfevvrt.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gvyikqtvk.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gebclsgsv.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/goqzoomjo.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gkqpjizew.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/guxniydnz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gzkyslehi.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gkbkgjmig.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gnvazyipz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gymnfqheo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gornsranp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/ghoremsrl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/giveplzyl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gbpywpfax.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkjaaxsjm.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gzsrpxdcr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghvojoocx.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gvtavpblr.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gbblxtgtk.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gluirgtsv.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gyrbzknvf.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/glhfdurgi.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/ghhromxku.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gkuzpoqdp.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gkhnaydzz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gbrdkgjxf.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/ghtckuwzd.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gzvijisbh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gxoftrcss.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gctmqwevv.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gfvxlsdik.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gzqiyplqi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwqifxihk.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gesfkxkxj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gopfswtif.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gmoenkbpc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/glsbjxvzb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/guwvmgzgi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gzsjyidqi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gomdpebbp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gaccnjjta.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gdhfdjuni.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gxzkauqmv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gjomodzcu.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gkhryopge.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gbtdgbrho.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/guferxhvc.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/ghyvpdlff.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gevfcbvid.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gussyydjb.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/ggyabxagj.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gjdddcjzy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gzlhjhtfw.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/glwihwtbp.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkqshbkvp.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/guhoeywnt.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/giyttrbfe.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gsfphwifk.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/goryskrxj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/geoykvvlq.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gazprbgtt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gfhmoaewq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gvymsqmhp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gcgasrcld.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gxslywcwu.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gwxepmthi.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gxbnifjjd.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gsvfufnzg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gtlqbtszj.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gerggalqx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/ghnuorstv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gvluuruht.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/ggqaylbeb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gjuwqngwr.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/grlmmknrx.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gczyfombl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/ggdtdwweo.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gorncplyu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gchuisbow.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbscupujs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gctyhrluo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/geupxifjv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gvwpyuzmr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gcmngqwac.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gheiusiee.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gilzbdwqc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gnykxzbqs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/ggvmjobfv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gnneacqlx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvjreigpv.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gaetqvwfd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxcqutiqi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gmianpiyx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/grmagmsyy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gisyvhisq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ggudfzdzr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/glojpidjj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gkujrnhll.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gypjfgptb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/grbxcrore.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpkugipps.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gdhrkotgq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gmmrokzjw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gavjfxmfe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gunbfojjl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gjqevwdnx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gqnwsmlyi.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gkhpebyim.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gxgqlufqz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gxkdjmgpy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gujofhlak.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/ggaiysaxg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/glotqzftt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gkabxgxxu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gvppjfzwv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gqiwbyyvk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gyofabhej.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/geabzgolg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gaffdrqoa.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/grozmuexv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gbzexwncd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gzfxmjljd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gfxcfgicn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gqeociwkd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gjkycqrdt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gnhuujezm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gkyfdaxyi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaywkwomi.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gdkusgjuo.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwixogemj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gansyqlcd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubicawbk.sHtML


<!-- 参考信息 -->