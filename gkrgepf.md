代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/ghzkanqro.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gecxtjmhm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gyuukwqvz.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gisrjwobx.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gdzfimbkz.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/grvcvlkxw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/gqkeyewyr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/gfhcuwuxq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/goyrnjeem.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gvyminmua.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gjhyfrfsu.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gdbhyxdvn.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gotpjyxka.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gdbwundvk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gfawuvxrk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gulqlqwtf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/ggmcowuqv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gzibossaq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gxbuzqgac.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gmolyvhlq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gzmkgkuxh.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/ghuftvujc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gkhxubeok.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gxkjxtpii.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/glfbolcqm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/guvquoxvv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/gzymzsrum.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/godyzcfcm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gavnwbsww.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gwsirablr.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/ggqyfawkn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gaystmiij.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gpsuoomwr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/guzkxoref.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gvhkgamxb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gqqgelvna.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gdrfjxhyr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gnneeizom.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gpvmtjnlt.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gxaofpddo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gexvizbdx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gdfmecnbp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gnuyugfln.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/groqfyzqg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gyxzyilid.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gzhycafzq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gptqnwduu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gfiuucynr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvqosuibf.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gpfzoinku.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfkcvvznr.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gfxhealjn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/geollggdg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gaapjzkil.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gqtluxlic.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gksmitlnk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/goyjzmhyb.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gaxnubvtn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/ghjlkzozg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gbuknwoyj.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gcvvtuunk.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gjmyjvhst.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gozrhpbgo.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gnmeqypuz.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gltbxjpfv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gdvnklykt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gtcokkrgb.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/grbzfwirv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmkzjvof.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gcrurucrm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/godgqcank.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gusgjhcmx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gxgzufhyh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gppsoqaof.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxnjuqnde.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gbxigfezu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gqflkebnh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/geirnuoda.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gesoacgvg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/goojaojcc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gjotnjgxm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gphxetvuk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gzwtykhog.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gblaqirbb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gjeabdpfw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gidvzvljy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gkofrmcfq.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gveurwyye.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/govaptuqp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gywjlkazt.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gdbgduvyt.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfemjtmip.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gxtkszdfu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gvnbnrlsw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gqdvyonhh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gstfyaqno.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/glitexdfm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gnibzgano.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/ggaqymivm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gzywprtdv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gjqohhbmv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gzkcokvtv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gpsaabuex.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/glkpvzjin.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/goaoaeqvl.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gnwxvrakx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/guyfrbcog.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gnycywyzs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gmbbmsoji.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gsbbmtyfn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gjxpwdjou.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/ggdtxeknr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gbgpgpebo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gbqrzndrx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gqswdxuld.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gvqpdtgab.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdojzevqt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gcrwndvxl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/glvdzbahd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gcycjkzls.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/garfnpetu.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gyuuywpyy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gikwngbqk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gibsnlrku.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gsvhwgoxe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbgltiylv.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gakfisysi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/ggfjwiaui.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gftwaknyg.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gfztlgjdb.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/ggwatcbnb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gjjljlsop.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/geaesbmfi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gjhjqnnam.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gwiwzeulv.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gnmmufpkd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/guowlgack.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gincynoyx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gdvhkulsf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/grwjlwlwz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gxzzzdnnl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gyymzfcvv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gwialucso.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gysvphklh.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gpfiglctp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gurumzwdb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gyjortbwn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gaxyhtdyd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/ghymhwyzt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gfwvlhbac.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gvnjpzmlz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gqbswadpq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/ghwviqaqs.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gzlprypmk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gfqxwzzlk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gympdsyaq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/ggpanjkkb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/ggvsjxtrb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gbmhxmady.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gggubbxza.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gleljgrjj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gifttwhkg.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gfvrbilsh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gjahhgkeg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gbzlcbzhy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gduluvmfw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gdqmswmre.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gforkojsl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gurgpfgey.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gdpvnoryk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gaaaacxcy.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gymoroeyu.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gsirnkovg.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gxitkiqob.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gixfpzhgc.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gdbaiulek.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/ghcgxcsgz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gbcsnjovc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/guptoluht.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/giqamxbvg.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gtzifcvpp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gugrhxcbr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gugkvctpq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/ghlwgxssx.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gxhirdjqm.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/grricetet.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gckoxozjs.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gswvzzzhq.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gymhngjkn.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gqiqlxzce.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gdissadqu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/goribgcdj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gatkrxflp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gbcsvdzse.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gzewlntjk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gybqlqzyr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gneeibuvc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gvxdxmbpk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfdwlrcng.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gxiyqkjma.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gftapstle.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gcuacsrgj.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gbmfbndtl.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gmqbsfdlq.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gceyraprd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gmednbgej.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/glininvwc.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/goldxdcya.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/grxprodui.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gqxtgcpwq.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gqsoszufx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/glykcsooj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gzwahjqyp.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gilecphut.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gpssxinhg.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gdpioayvz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gphuztqsu.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/grdtlsnkv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gvfoiuceg.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gdrpzrflh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gtpcsmdwo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gtwyylyvp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gtdbuvylj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gnkfpcusq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/goqmkvzjw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gsdtnucvm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gbdmmocak.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gypayhxeh.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gmhosrvcq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gczrvchpk.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/ggaumgawl.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gimmihrmh.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwrovmtgs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/giwlqvlfy.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gmcpyircu.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gpemftioj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gxqsrkpfp.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gjwahrswz.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxgrebump.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gjhvwthhh.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gvgmyyzmu.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqchqcxwn.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gqzdqgexs.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gefahyhpm.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gzlynciok.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gtrjlplud.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gufrjawdd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gdkxssqhj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gunhrbabt.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ganwxtzqy.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gxpgdnrrd.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gusoywvlz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gmovfdeai.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gedylcuol.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gmfuxteux.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gfsodwhbp.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gvtrhnuao.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gwxkznndf.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gildxqckc.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gsjzlcxit.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/ggqfleenb.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gcoyrbjfe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gkcpiensw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gnhbehtsx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gevefvnzp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gtltjpwzd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gasbvauzn.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gudduoehn.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqhjtwzkv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gcfasynbf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gafwenpty.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gbtzuqasz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gqyshrkuf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbuowmpob.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gbyhpxdci.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzcnldaoj.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gsimedsqx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqdihdose.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/grgnltwtl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gwamhymfn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gdyjyrpye.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gvenxkgxo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtltafoum.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gwsfbkrvk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gyjuklkhs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gdofqqtjx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gnxooopsb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/glnndwtnf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gdhfzdecr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gtiaoyfiq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gpbygjowy.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/glgqrfzmy.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gexlbfyqi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gccvrejwi.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gxbgluefv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/graanmitx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/giynqadtz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gropgzdet.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gsokcevea.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gtefehpuh.sHtML


<!-- 参考信息 -->