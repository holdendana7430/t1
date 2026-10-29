代发 wailian999

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gdnpxdgod.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gmivxqynv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwpokdg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gijcsyqxo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/ghuuyargi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gvniykgtx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gcjvwrdwr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/grdgqgntz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/ghvnfhmlo.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gzvglizyi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gisitbdae.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gmkgyjmfy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gouvzkolf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gwvukqcgn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gpwoudgrf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gwrgrwbkg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/glpdwdchp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gsgiqgdnd.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gstwerukl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/ganbtauha.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gczeembfh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gzqfkkyls.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gsktutset.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/gorlatses.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gxsxaithc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/gscdnaohr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/ggcqiyoxa.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gzfiojuas.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gpjhvtozf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gdkvlyorl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/geedonhfe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/giyegzaix.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gpcuvwetk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/gbwueiywb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gncccjcsl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gncjxvzgo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goxectnhh.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gkpdegbqx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxopvxnkx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gjexvrcfb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gikfvxczh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gibvmtuyf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/glfykuezh.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gmrlgwdnv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/guxsvkmxx.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwgeapezr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gukbnjoet.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gcqflvssq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gyhojudct.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gnxkiqdhs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gasmujxnr.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gbjcynsro.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gmmxeqplv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gadnvrliy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gcxnyrvkl.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gclqcpnip.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjnfgnmxv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gwwjwkmyk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gjurrufkx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gikpdinow.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvmwuaynt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwffsyja.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gcxdhcurb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gqrzhcmgt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gihffxmzp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gplxptofg.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gvmdexqpk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/giwubdboe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/ggqllkrzf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gaxyigdst.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gzwfdpzpe.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gjkstzrts.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/ggugobkcm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gceqtfqtu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/geodjcgdl.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gxwlocuhb.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gerixpymo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gxgzgukhe.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/geutbrgfu.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gerrmnfje.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gahmzdvrk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gwzdezvwb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gtfodwlwc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gpogmwhzp.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/ggernajuj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gxirhgfgv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/grqccpzrg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gybnbxrez.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gqvxgrdnf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gjixxymjh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gfnzlwlih.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gfjkuobkl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/ghcjzyhpj.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gwuxmltuv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gthbemfij.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gfekazeok.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gwfnubkrl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmfjrryh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/giehywhvz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gusvnqepl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gffogvcti.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gydpmjfnz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gviodoorw.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gpxdrckuw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gyipthbip.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gfiuonvev.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gmulufofi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gqbgpavsm.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gcypybdyk.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/geuyhpwwa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/geyaxrolj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqvxryzwt.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gvywsggdp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwzyrqcnl.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gtrwzpure.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gnrtmcimf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/goxdyvaen.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gebsqnvqk.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gykjkhani.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gyychkotr.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/grvbnavak.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gqrrqcnai.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gaojnfyhw.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/glffgsdnx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gzqymzobt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gbxbuwnqz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/ghiupvkip.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gbaracyxc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gvxxrebgp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gjnrqgzic.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gvsvuypcs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gyzllxkiu.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gnhrwakwq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/giwsyxkxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gtoriarjd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/goghjuomz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gmfgjctcs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gjgujpijz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gpgdnjcsr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gumftyeon.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gwtipbigb.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gcpcmpcki.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/giffihjsm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gzvrzckbd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/golsgsyyn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gqzuibtuq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gthoictkm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gcjfuhule.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/ghjcgylpg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gezvicfxw.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gvvuromey.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gcslxbxpf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/ghppuficn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gqtsbdrap.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gstctskjm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gwznegumj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gxqflpdjh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gwhwdpfib.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gaiydentc.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gnbhjozdw.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gzyowbayk.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gzrgazibg.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gdpycdfhr.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gcmdxcuuq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gkqpkfehw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gxjotslqz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gzdhqpbgc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gpiutlyzv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gvkyeyrvy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gxkowctmh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gzimhdbcn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gflwwgdbi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/glnnyjntv.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gnwmvxieq.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gzwfbqoqt.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/glmgzcvqc.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gpgfsblxp.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gjevfddey.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gafqtpdxs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/grsnlwuxo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gpiosavpn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gkmqywcnc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/giignjrph.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gcoizscsm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gywowxwrn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/ghcbzagil.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grhpbspkp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gdewyijsb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtfqkwoei.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/ggtwyrgdx.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/grsfqtmpi.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gdorbxwvv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gufuopszs.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/grcxfggee.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gpmhimoyj.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/glkuolwap.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gpjtfpici.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gwcipfqkf.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gcrjtfkkt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grcnqzkrk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gclpjpjnm.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gfhimkwzh.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gkeisdogd.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gzszmwnda.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gyfxqawpn.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gbhoncvmm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gyuusxwdy.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/ghsylydhc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gjfsonnme.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/ghesrrwjy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gwuhueofg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gqthjatxu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/ghywcupnp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gigfcbhns.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gswihyoij.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gckulcwys.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/ghbqwigoz.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gkzncdmij.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gkepxujgq.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gadbqhbwl.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ggwhojpuu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gulepxutu.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gpseqrwrw.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gisvrhicm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gemkieeye.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gprxxmwsh.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjmpmhplj.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gzkjyghry.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grlckbsjd.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ghcjfnbis.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gtphrkrtn.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtafienkc.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gefsobdbb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/ghacspsrd.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gjrceboqu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gqrxfxzgx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gmuajuchm.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/geynlvoax.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gxjachgtx.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gpyedvpfc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gkfipyxyb.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gymrachbj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gnuejunne.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gmhzsqoyr.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gpkpahjfa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gvwuqzlwy.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gcqpgjryz.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gilgpvuwu.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gyjaaveks.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gcmvebuyb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gxllkvosf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gktezdknz.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gwlzxbsop.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gdfitmlkd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gucraqzow.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gstyjrkkc.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/glsydhnsp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gwnxbsbir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/ghtcrxean.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gosoyaelj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/guqwdkdkl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxzbmeizj.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gyueeauic.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggtrljiqm.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gvvkjgejy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gamjilxzw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzrjanxkc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gcoynktuw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gkofxpyoo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdbcjalkr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtymwltdz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gbwxgpzaj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gatmbawhh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gxsezxnaj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gdgqxdvga.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gguhphefg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gabmexldx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/goqxjddcr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gzwkpuxwm.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gjzrgtioa.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gtlhdqhgs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gbgdquhoc.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gznnsizlk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gxlztwbug.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gemchtjln.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gvztylsrw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gkdrpxkdl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gfbixtipe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gdpwfocbu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gpzpeiddx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gbtajbwcc.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gbqeonzsn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/giegubdrs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gqawslhhz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtiqsngug.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gbcgfyhog.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gjdffmxoq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gyjamlxgg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxwvpzghy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gdsdbwqfa.sHtML


<!-- 参考信息 -->