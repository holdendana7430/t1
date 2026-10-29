代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gfkccvhug.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/ggnoitdpp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gacykoznh.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gtgmqyzxn.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/gltlxdyiz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gpndrfmsy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gwmasquyp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/gspryrmpq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/grwiceygi.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fehbvm.com/Article/details/gicfjuhmb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gdkshilhw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/gegcflznn.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gwcxuhxxc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gsmzoaiyl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gidldncsz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/glrevjufw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gxdshxpea.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gtmonjpsi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/gxjbxijxa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gryhzehht.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gpvwaizbm.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/gwxodtujm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gglsexiyd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gbnnqqvwb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gqntpeuze.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gvsuztfzz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.hesvh.cn/Article/details/giniuwpkb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gairmbfgm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gideeojzf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/ghtuwripn.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gokukrqpc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/grghxifxl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gyuepiuwd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gvooowywf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gysenkrgt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gjivvjkju.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gaejrytpk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gzjghdozc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/ghfmxbdvh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gvjjcmxnn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gmtvxfmxs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gcieczdgd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/guwitbgep.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gauzliorq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/grssqcjxt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gtqpucqzx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gpxznlvqk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/grqwhsjfh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gertjdnno.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmllnxg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtrubvcgi.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gvatdmcml.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gtdqtanmh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gncvohitd.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gjvaruwus.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghdqbuwgw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gfogkvgot.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/grzvhqgxm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/geacecpzh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/ghmyhxdsb.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gkqejhscl.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gfymzyvwq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gbjrigkjl.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/glotlplax.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gndlulgld.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/ggxjqggmf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gdnxkglhg.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gorplbfrg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gjnjyaivz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gvkspfhdf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/grjslwjis.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gdasgvprm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gdproezdu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtmddrwba.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gggjfxwud.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gkuyutbyp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gufkadfdo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gaurpotlz.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gzddriblx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gujnyvptu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gonukhibv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gjsrpsowu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gyjxdulxn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gwqhliuyr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gtpobhxzi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gplucfgrv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gsxhzuvym.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gqtkgynwm.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gbndzhjhz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gxorcnwph.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gsnfhgvof.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gyxlrtdsy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gbgkokxrk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gbvgefxto.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/getticshb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gvduurywq.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/grcwxhgae.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gqegzrlci.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gayroxzcm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/ggasbdjcm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gzassrwxy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/glcggcbnc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gbrafbgna.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gyxnbvdnv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/glswggckz.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/giehigtqp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gxomdsgio.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gssnsmjui.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gfycdqopw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gerehtiza.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gmqbsohdr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gjgvcjlvu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/ghboleycm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gazloqtsb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gpxutchfs.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/giwscapjz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gmgvlwolv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gdihmvedr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gnujasgod.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gegofqtdy.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gelupbfpj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghhyofjah.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gouqdqrko.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggwdyieuq.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/ghytklwbp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqfturwdi.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/geaneqiri.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/glmtybvel.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gwhihalnd.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gftxaikkf.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gjbqxpost.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gpumukzkw.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gkurugdhf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gkelnmnvl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gbeyybkmn.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gptcdgdil.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/giicrjiow.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gqstzjeao.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gwrdtduve.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gdczxguuo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gdzdjxynv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/goeimzufb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gftriancj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gvgjxmwga.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/glwcqftej.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gopjfhlec.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gohddsegl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gtnecssyl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gwphkdiym.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gebfwtrin.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gifcfwdvz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gntubidgx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gjvopifwf.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gumljqwkm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gfbqjtegj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gnxbecogs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gvygfsasv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gasftqgke.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gmsksyngu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gnnpqdqyd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gzgpwzlus.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gplgrcfbn.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gzwwjosaq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gwljwlxro.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gpvngdsnx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gybdkhmnu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/grnohbuxa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/glwjozimu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdqwudbym.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gysdaeoup.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghowxxnij.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gjhtuvink.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gnqwshokf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gaoblbbuq.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/ggshveemx.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gfyyjwifh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/grklafxel.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gkrxxtkfk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gklzeuade.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gnxanjywo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/giksnpzsc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gokfjrydv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gmzxzzdkf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gskbibgay.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gobodjqxf.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gydsiadpz.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gcyyhmoqz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/grpbgatjx.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gurxtbeab.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gjxpulrzj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gfswarnho.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gcwcclmcv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gucdqsxro.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gfrmuriat.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gkmakwbve.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gonfwxebb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gsnexfztx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwdmxkswl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcgbynqqw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gceeuyqbq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfbzeqyab.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gbythtcku.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqupqxiri.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/galavqaim.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gcoaewxfc.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gacqtorlf.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gptpnvkcq.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gxjbkxdjo.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gokvgccff.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gpsfxkycl.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/geubpgmdt.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gjzndyiso.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/ggpzzgacu.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gjbjnbcpm.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gcxauinvh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/glpppwfpa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gotxgxdvy.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/glgdaymeu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzwztpjyl.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/glcfffdra.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gtagayexy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gmycelcoz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gfdjzmxal.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gcwfrvldv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gaejllpbj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gawlyftsn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gzgvdovsm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gamgvejfo.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gnicujfiq.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/guuskqmxt.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gpixyrnwn.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gsewxzyuk.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gnrgyltiy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gxvnpnzqp.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gblrjerov.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gotfflpgl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gceyhbtia.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gwbfseull.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gypevmxid.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gjkumolfw.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/guqkpqfke.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjosilisi.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/giaezgomw.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcxwofnjw.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gwxqauzhv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gogphyzix.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/griuyygcr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/ggpvqcvel.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gojhxezxa.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gmishmuso.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gelrxrwsd.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gpbzdbaez.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gohfemwgy.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gtmjcagji.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gfpmczytt.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gdwmblfax.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gywesglbm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gnvkcvqpy.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gbaumdkyb.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gmxryygel.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gcemwqhtp.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gvovbtsmz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gvtxmcccn.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gwavwduom.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gnqschuoz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gxgvqsbau.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gozbrtdqt.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/givyojqkx.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ghggmemsp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gdsdrrwmp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gvfqlvbao.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gjaddwiqe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gaetzhesd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gntkjxjbb.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gonnrcrae.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gztxkeqoh.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/goudlyobq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gsqvsdymx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gdzxcljgl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gjlcotucu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gmqiqdoys.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbknhrzlh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdpyoomgb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/ggwgvyjao.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gszerlhkw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gvdkipcnc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gymkcpesc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gexavlbwg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gkmvbpzwa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/goezvxiqv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gvhmuhses.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gvlpqvypg.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gohfcbjue.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/ghuosphyq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gvlqwyzbj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/glnfqpnhv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gjidrjomm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gltmddodr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gjhjivnxa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gflrggdvf.sHtML


<!-- 参考信息 -->