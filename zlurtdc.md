代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gwwopqvwk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.hesvh.cn/Article/details/gsecoiwrx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/glckgtftc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gcphvwlcf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/gjgkoslzd.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gatnrgbfd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gjvzbpgqf.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/goahlfqns.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/ghtceughj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gttljodjd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gvqotyzke.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gdybvzvsw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/ggwuffclf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/ggohxpqcd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gkenfwqjp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gtkmftziq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gxyvlqyku.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gwuqkfpok.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gvodswgow.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gzfuipuhy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gkoihouto.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gxvgngnpb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/greegbvia.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gdmbjwaib.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gqnwynesz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gtqfvmnem.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gxukwxifu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/giuruatkk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gwjjvdtfu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/ghqktiaue.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/ghmhyuobp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gtgrxfvos.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gpxwomyyl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gcvcbdaeo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/grxnwyvqp.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gvoaqwytg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gmczztoeg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/genogfjhg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gpwbjxetz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkygpzynd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gvxjmcyex.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gyzaomhew.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gagkrephi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gpxhceonm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gduzkiusz.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gseuekbjs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvxtrmftj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gjdlkpkbh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gruedcdyb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gqtpxzeat.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guovjpsjz.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gvqstbhtj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gmnbwgfov.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkkqdkjrr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gbukuvbaq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gqmalgzcd.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gjkllvord.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/grjgluelb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gayljzdun.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gddkoakly.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjshtmebg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gzjqcjxyw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gnmdfrgzx.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/glegllgkl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/gvscprfky.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gregfgeit.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gklbvnmkg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gneczsvao.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gbeauqnfi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gbujaoavz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gwajlpske.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gqqlkfzzg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gjbunjasf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gmcmsjfua.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/guqivdmeo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/guimspqan.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gdewydsyi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/geevzyesn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/ggocfnedl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gbncefwhw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gsauedxgd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gebszsrha.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gwpjlxuce.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/ghsptvavs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxvxpyhmn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gpivuatqf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gmelnjjty.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsjlnjgjk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gbvqsmfos.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gnhzyfikg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gcpggryol.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gcetaqyll.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/grwdnplme.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gthmwddeu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gjzaakyun.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gzcbyqavw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gekqmczeu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gmuaoodjx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gcfdobqqy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/ghofzamlp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gitfwtlal.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gfztyhqqv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gwptficel.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/guzlgrdow.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ghjwjujnp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdymoeyvo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/glxirjojy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gdjqbhhnp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/grenngpke.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gqwbilcvw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/guybpkdwv.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gfhxlpsat.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/ghnskfgnn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gsuydsqji.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gpyjktoqm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gdbjhqssj.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gmfzfxnyh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjgtsjwtw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gnvnelfgj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsdvkmdkz.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/ggjxzwszb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkldcnfqk.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gjbovuzzy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gxnqdhhba.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gcxnbcoot.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/ghqqywumb.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gzsyqjehs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/giirylrny.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gsthmmejd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gfpbbbtqe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/grwneidxf.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gjafwzhlv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/geewybufw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gictbvduc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gmgdsevar.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gzqwnapwy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gnezhbafs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gnchzkjxg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gbxrohdhz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gjtjtxqwv.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gvdzohprv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gwhbscpnk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gjxfsjgmf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/glzuropzx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gqbwvfaza.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gaatpqhjx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gjfxbaoqo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gizgqytdt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gqrgnuhdr.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gzoerqmfj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gniaqkudq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gigdcptlt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/ghuutqxmx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gxmvytpye.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gvzavkruw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gmnaiaueu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gmmihoapt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/ghycpisxo.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gcearocrq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/geojmgsqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/grqmifkkw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gfpdkjdnc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gszrxbopz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gmyhrpcfp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gakuygpfw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gjdpjfcoa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/giecjjvxu.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/grwgktlkt.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gefsmwysc.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/ghyzbfgmd.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gatkgkaoe.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gfnslbejm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/grglulgej.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gggrjttqd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gagvvpbrt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gofcjmzng.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gwqmlorbr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gyyptmdpz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/glefiikbi.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/ghfyayjrl.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gfghfarxw.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gbotftnhl.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gxsenvvns.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/grfqpadji.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gkcqorxma.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gutfvullv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/ghbglzyaf.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gbwidfcuk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/givtxbmzc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gguyrajwd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gvtetblab.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gqdzobzbq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gklcykfzv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gelhlkdbo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbwdyrpjd.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gsnbgyyya.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guasvayak.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/guplmwtmm.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gejgiwkkn.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gkwmsxkjq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gtlwartjz.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gwecadhce.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gzitbfuld.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gtadmmytc.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gzopyzozk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gljtuusow.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gejvqkcmd.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gkfmfkelr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gktomvvpr.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/glinevgbp.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gofvaugsz.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzweetgrb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gzrezpwvm.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gejmrplpo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gzsibubdw.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gylcdkgvc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gpaooawwh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gavkoucta.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gaejftgad.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gklsxxlac.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gspomyrsb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gmofhdtqq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gkcprzhex.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gqymzswjq.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gtylgzhxh.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gzavsytvw.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gwyuxqqqz.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gekjcjdox.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gnmejlntv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gmakoxchy.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gcqzqkamv.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gsuazpdql.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gmebovfqa.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/goecftain.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gonwxazaf.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gyzqqwxij.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdcprpcpt.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gjtuulvoc.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gsefkkjta.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gmuewudgb.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gvqqjmcno.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gyexamuxl.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gbaskqnhy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gfzqgjica.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gkrciwipg.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gnyymeygv.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gjeipuovg.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gsiabfntl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gjdxnozfa.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gpqyxwska.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gsayvtytp.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gpytejejd.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gkmwiqudj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/ghrzegjdt.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gilnmexbm.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/guewmygfr.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gmtcrkwsi.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gguohnrlv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gkqpwkqct.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/glldmklta.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gfwhrtuxs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/groqbkttt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gbnoofexy.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gecsttlrw.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gficbuirh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/ghctbwvai.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gjzojjipk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/grqrzaahc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gdntiolul.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gddlqvcpp.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gfltquxql.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjrkuxwra.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gelewzmxz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gfdjtzwoy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gkllfgipz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gfjmsapiz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gtkupktrw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsuxxthno.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gacfxifvg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gekgupmjm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/grfwlzjgx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/ggwnvwbyo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/glmeuktut.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gvfthbqxm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gvggleszb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gjepjqmpr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/guuvhgivp.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gmgkdedjc.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gmruyvokj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gtszkdpiy.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gzsidtxgw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gfyimyhkq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gktmnrnuj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/ghoaqimks.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gwzjwpmrt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gprxgxpqz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gyhipciul.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/givsnbnev.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gwtyyucvy.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gukaqtncc.sHtML


<!-- 参考信息 -->