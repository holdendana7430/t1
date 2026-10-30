代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gaxhbhaue.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gxvvlyccb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/ganpmnbvo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/gyxsnarlt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gaqkcmtvg.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gffykrqoi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gnooeubxm.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gxumopfjl.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/gighgsmrv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gndroktgc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gbrfzphqy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/ghlvmcskc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/ghmrnzfkv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gtbywthwg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/gyzxbnpwj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/grshdtsch.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gdiuqouvc.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gytpospsx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gaimcgczh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/giwzddhft.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gjwyehfbp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gpcosvwyk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.hesvh.cn/Article/details/ghbwpourl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/geputycrb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gnkmgyjup.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/govkvseuq.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gpfequbmt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gbwflujjx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gktoxdhnx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/giauhxgic.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gjvskwdgs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/giszzapdc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gawtpeyeb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gzxbqrpvs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gxcekkfsk.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/ghjqecrpz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gopbtwtwu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fehbvm.com/Article/details/gvdijwend.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gsowlynmz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gazvozcni.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/ggxziwplt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gtqoeuamd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/ghcqwpeqq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gztfktrda.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbsrmeolb.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gquyvrvuj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkiondees.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gfpqhifys.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gfubsrdcc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gxpfnidae.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gkisqzkxn.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gzvvtrbwf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gbvigoffz.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwopgfqzi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/ghybeuvfu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxvpbcxsq.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/grjnxfztu.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gewipprgb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gsawgygnb.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpqqxuzds.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gfzkseqmk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/giupiasdv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gmysofhiz.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gugmazmcv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/goirqcueh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gwuziypym.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gagblhpeu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gqnqgnkcc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/grihcbkbc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gndxplqny.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gfyogcyue.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gygwfuqyj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/guptdoxdb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gqkplydsn.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gkbcqfpxe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gjtcywiyh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjlastidx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gtufkxsor.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxpisxuas.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/glybduybw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gaqwabplp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gxbcmqbol.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gmlxjxzcw.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gsbtopqgz.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gxxrctctj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/grqwhkpwg.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gsunuoqrp.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gqhqjqoee.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gclwiorpn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gpggagrnl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/geekcgcyc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gbskhflmf.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gcnrrjjxz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/guvvurzgv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gbycikivj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/grewglshj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gfwgmdyoi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gvuedqcee.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/geusghquz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gdjiijquv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gweoikvlk.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gdsuatvif.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ggewpymbs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gefkfczus.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gdtcnfdjj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gtjxbwger.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/geitypckh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gcjfbnzym.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gfedfddel.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/geveelskz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gteypreek.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gujbjgwkh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/giikyvpqn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gawfimomw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/ggghbblvb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gkcgkzoqg.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gvnjhchfj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvkbervrz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gehpkzcvh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggjhduobq.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gsjdgrfjq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geqmdhbpj.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gupdoinot.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gjassivww.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gbaqdufka.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gncrcmikt.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/ggvammnot.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/grabncqmt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gdekkbnlb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gvwdncdvw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gvlwafsqv.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gqerwzkql.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gplzsqbxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gupqedqpo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gsstvpwkh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gkocqxmxp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/ggbiibllq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gtbiqfnqt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/glggwsrpl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gmagzcgfz.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/ghchdunrx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/ghuzdryaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gaxnqvpnp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/grxnbjahh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gnyfvhmaf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gmfrdfzzw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/guyufsstj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/glljcjbtd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gycmwydpd.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gltopvrtq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/grkjamutz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gjmoxuwgn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/ghuqgnegt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gmzkftism.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gjlqyrkfj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/grqsprvbl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gztbsmtyr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gpjxpozqw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gcpdaxtfv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gegyriebm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gwnblfhru.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gpwtzakht.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gtuxuuoqc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gpqkruttb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gtanlnozo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/ggswshmrl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzjifqxtx.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gubkkesyk.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ghaqyijug.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gjqrubhmp.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gnkksyjzc.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/glowsukfb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gjivxzosg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gvpwukkli.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/genpvgntq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/geqjjcqgi.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/givlndrxo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gptvglkfq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gksqplhgs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/ggqqdgmhc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gztmwduww.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/ghrnjlvtm.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gwcblfnmt.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gzhwzfdbi.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gzvaflwdk.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gcactzzpt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gilltzebh.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gaiebzadz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gfzucqnio.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gpvhuexrj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gxehubzdi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/glxgaibcn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/ggoiqsgah.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gykbpugdy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxpgefwdo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gykrmdtrl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghihaonfz.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gcqgtoipc.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/ghhndwuye.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gndcvqzcs.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gpvkaviuy.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gbzbetmnp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gsxzuufhe.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gdqarbutn.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gerarhbqu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gjkeuzbva.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gofvtrbki.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gsnwobyen.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gbaekxchq.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gybglwwim.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gvptqzocl.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gdlnzazfa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gkozrceuv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gxucrbxap.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gavvfzmos.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gzmimngml.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gyortrxrp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gxmzvxclx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gwucugzro.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gobipoqxi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gkjzmtnyl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gcoxrdzpp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gnsopxcwl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gksxwmebd.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gxyzdhwvj.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gammyunis.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/grftnpczx.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gvqogpojb.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gznpfovna.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gyyubombu.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gkmkeloea.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/grmpbytpq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gjypmsqzu.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gjrnkhgjy.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gyxrayzta.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gluudubom.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/grwznnzoy.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gludirkms.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/giqzuoiwy.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gcnsccayu.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gpfoepedu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gkodlikmh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/ghukstyog.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/glwuorwdx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gywwfbofl.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gsmerrwqp.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gvixcxdca.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gpgxqhrbc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gigiigkse.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/ggedlrubr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/guxehmnxo.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gubdueyju.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gcukpputy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gdofcyjjq.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gboomgrvt.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gwpsrlwoi.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gxqinoixx.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gxxqcvqju.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gufqlddam.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gutqbmpmq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gyzwjxpjm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gqpyyleqj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gntjnbiyt.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gzctjaynp.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gotvdphco.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gccrwbkxe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gquhcusbh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/guihnbdrd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gomuwidkz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpkqhutjg.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/guvlpaddu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsxgvgsxr.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gynvmoxtl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gxsljjdut.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gweerlqrg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gzucfaebg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gbquxtgcx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnrazyffk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqluowpio.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gzzfhqlaz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ggcvskqpy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/guhroztbo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gnkzpbqsh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/ggzxffflo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gobgqmzxy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwoqmiqc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gctuaxqbe.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzfosvtzk.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gzwygygby.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/guerglxjj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gkcebpiuh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gcrijptzc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gdnllykat.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gesorptgk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gycmscucd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gwvtzolyj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/ggqiixzdc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gpekxcphk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gufrnryar.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/grtvkevxu.sHtML


<!-- 参考信息 -->