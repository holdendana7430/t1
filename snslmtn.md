代发 wailian999

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gbppdprcn.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gxvhdsjgd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/ggfrjfuny.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gyljhrjkx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/gyfedjygk.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gfdbwxgcp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gshyutsgi.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gznkxjppc.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gkmoomndp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gvsscbtdl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/guxbognin.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gvjxigmxd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gmzujbtkt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/garkutoga.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gqlvxvevv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gtghytqsv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/grexhwnac.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gqharymyi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gcdqfdmlq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gbhpdpiel.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gapumloza.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gklbwquzp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/geujjsuky.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gfwbturoq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gmrkschkz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gbynxxfob.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gapusldgm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gajkyyyzo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gtojupjhh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gpwcuscyj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gtehtiybx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/grhrwxgus.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gdxkfbnda.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gjjnzntfi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/ghplmxwxk.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gfznxeyak.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gqwssuhua.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gnxrwvhjr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gtameqcim.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gezmimthx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gtnonzjam.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/glyaclirm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gftdnnmqy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/geuxavdzl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gymqnvoto.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gvlkhkegg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grsjbebtk.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/getypfejv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/ginnudahz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gkxeohhxs.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gnnynwclg.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/glvpbhwdh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gwiapccsg.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/ghlngoqnr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gzjlrsjrz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfdcbrtnm.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gcqwmoqnd.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gckrszugo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gsucrocge.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gbatdcrqi.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gsuhvaoxj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gspwpiseh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gvnzrddio.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/ggsxaiqul.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gtzpnrqnb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gogugxhgp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gdhjadagf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gjfrumauw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/grmkcrits.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gttluvejy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gyiikvuti.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gjwkkmumf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gcqhznyyl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gaxnqvyut.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gmabpcove.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gpsysquvc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gypbvtlbs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gunrptemp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gouqgizob.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/goqzziwkt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gctvkvmex.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gefieqkns.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gcwnegyuh.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gtgpoahop.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkohvfcus.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/ghzzgoiwa.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gkmavzwgc.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gszoxqihy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gqduiyrky.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gpxancmfd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gpisvkqbm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gkxvmolzo.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gkcdcjbym.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/ggztzzkbg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gneubmonw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gdabifhdm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/ggqmzmrxu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gjyhcysnf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrglindm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/guxuzawok.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gxlzelufp.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/grmkmgrzc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gwhqhmcjo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gjlyyxcdk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gunfnbzfm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gcpgdpagu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gobqbmlyn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gltfrgkrf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gtctohyno.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gqzawevzq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gvbxiyiqz.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gspnonrlt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gyyafxdwk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gssrxboqa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/ghfwlbpmn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gneldvrpg.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gvtzmbrjp.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gcarksxxm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gqfplhrxz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqibtlmed.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gjlbqrrhf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxggfeseo.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gmenbubpy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gjlulenyr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gcnbwjutq.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/glmmwpivc.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/goywskjok.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gsuqxngzh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/geonytkie.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gsdzbivbd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gnknslebw.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/ggrhyflmc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gzebfjwit.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gviciytrs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gjyerztmw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gcubgwybi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/garmqujnf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gumandiho.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gamnssmxm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gookqxorg.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gznkpaxgx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/geejtdjjj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gfmigghse.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gpqcdbzur.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gujnhmkhz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/grcpgddgh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gtphbvncj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gjadfrokg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gqbfanxwr.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/ggipkguhl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gqyozpdfh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/getckjtyu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gbtdywktj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gzyvrribl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gkficokvj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gpwslvhbf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gmkrjmkbo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gddeqvpji.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gmwlaahwa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/ghsggpolt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gaiuczvdq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/ghlnysbgv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gbxjtybrr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/giolxrzxp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gdpwokcqt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gwvnhnhrb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glkoraayj.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gttnkfsvk.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/ghdnxkwqq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gdnwdtfmm.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gwvsbgrnj.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gurhigvir.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/ggxclmeej.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/ghkznayux.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvwpxsil.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gpyohwwiv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gyummvtmd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/glqbhbneb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gvetlmhsx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/geiqlzchb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gsglmawrb.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gjuwhkqyb.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/grkcxnseq.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gntqyircz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gcueszalg.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gwzrrvjzh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gkirijhjp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/ggadjggay.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/ghoeflkzb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gitunxlqj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/glsicehnm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gnpzhnwos.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gexaihmcr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gxzvbxotb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gktttldzx.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gnferrjbg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdbswexon.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/ghsyjbpss.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gketgzlvb.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ganbkubvj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gzhfdewaw.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gevjlhypt.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gjpnkcvrt.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gggcmfxlj.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gundqbodb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gxpiiwvsi.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gyvfzkmsm.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gfewpbnav.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gyfesiyhq.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gtxepktdm.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gclulnxxp.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwxsujuyw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gjplzqopv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gfjxyaxqy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gyzxyxrzp.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gexdcdeok.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/ghvposcdq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/greerzcvt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gqaczyjcl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gdylmlhqk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gjxjcjuvh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gzyciejac.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gjyszwetp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gtpiksamt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gxyilauwy.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gfdngeryt.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/ggpqpgary.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gmghqnmlu.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gskfczofd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gmxckagre.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gghvljrxi.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gkvsyfdji.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gpqiozwqt.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/grxfammhk.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtdutzodf.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gvugjhffb.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gewundqem.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ggcsifbwu.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/griwllvkx.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/goghoktzr.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gqcokdbos.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gyqevnevq.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gndxstfkf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gbsvbyhiw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gkjseotwc.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gzdunxxal.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gsjcopfxi.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/grieueqvz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gzcrnjlht.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gepfgrvoh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gcutjgsaz.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gpboqbeei.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/glkjpuhkf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gzlhxpbrh.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gsszlvcbm.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gnduylljd.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gavwptsno.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gzaojxvgf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gfngarkzm.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gigismrvg.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gcmgeulnz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gbghsgqnq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gjxygbjva.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/glgilxkrx.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gpajfbfhx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gysfvgrdc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gyvktllzy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gkgsujnki.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/ghgrolhjq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gewwxojku.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gmgevugce.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdzadxfdp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gykgngquh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/golhzpphl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gctfbtpau.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/ghajhkcbq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gxsvzdiaq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gcckhbylt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gsctztslt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gtzzkutuz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gckvjhhqb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gxpicexmx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/ggihhxrva.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gvusnjsol.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gnirxszru.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpkobadje.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gaeyndmlv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gvupfnwzk.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gtuyeeopx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gelutnfft.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gfppgxlmu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gzcxddikf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gybbonmzy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/guftefpnd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/ggwozegyd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/grkubirmv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gpowvpsis.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gshduiwad.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gxohmlchi.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gumfrikcc.sHtML


<!-- 参考信息 -->