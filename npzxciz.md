代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/guqvitahd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gmvlrculn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/greibbvay.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/ggnuggebd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gagapsjpr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gxsvqcqub.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/ghwhpmntw.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gzspgzsbp.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gshqpinpo.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gkivajjad.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/ggieveiwk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/gkmyvlquo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/goxjpkyak.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/gqsbhzpgc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gfqrchtvc.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gxtotkqvt.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/grhpkjkyr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gvydcpugm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/ghalmfxdk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/ghbzvhnfb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/ghnczpibl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/glelqdfhl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gxmmfzrdl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gayfujidq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/giinheavh.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gmqcegrxw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/ghpfkshgx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/giwctfdco.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gmpnmghsr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gdzkoycuc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gueladvrn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gkgudbyah.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gorgteawb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/glhjmbdhm.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/ggsujenic.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gfgjlppqd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gbhndnpsb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gmbtsvoek.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gugzpqnak.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrfkpnjx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gvexnlzqd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/gwnwtbivn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gwjiwmbnh.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gnsqcitkk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gmilmcqcn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gwrliwmfl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gujdlhqqc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxcxdriux.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gabwbcrln.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gmidyeerc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/glkxeqzrl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gsdoxzpsj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmvjizxeg.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gvrpdeyum.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/govnjfqnt.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gsflruhiq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/grtsjmaes.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gbgnvvpul.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gvifnxamw.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gdojbzbay.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gkkgeqgsw.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gpgjpmdnr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gudhvlpsz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/germcfwvy.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/goftiykxj.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/grqrbzadu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/guicbhyvc.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gqmstrvhc.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gqpgasngw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gkfdofnmk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gljpleoif.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gdlhjgogp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/ggpkbcrma.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gytiftpzd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gnozfflic.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gzgkjybbh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gfdweqolu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gautggntz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gjakihtfl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gkeotjrbs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gielodaon.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gslrltway.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gwdwmtnom.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gmalsnmdt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/glmzgftwi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gmnmjseyh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gocvkdeva.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gnxytsvam.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/giyxfhwdq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gmwziflmx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/guzmtdpfr.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gchivcare.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gqzeqbtmt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/grbqdtpcv.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gojqkoiqa.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gffavektc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gxifgcxbd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gcfwglcyy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gueihewcv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/ggdkcmmtq.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gstgyxoef.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/glpdeizlk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gihotqyfg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/glwgjkiiq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gryqsqaji.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gkddjzwin.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/grkfojnjr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/girbvshfj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gskbauezv.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gmpojwjhm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gavqjrplw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gkrsqvzez.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/glcyhbruu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gfbqcylal.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gizxxcaqa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gbdclrpbb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gfqifklsq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gltlqiyie.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gsyrhvqqm.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gkpiojsgm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/goacfhkgm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gxbjscljp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gxdhlafha.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gunopmxut.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gvsmcyltg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gzovtrgoo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/glinhtrzc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzocyvcgh.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gdhzabffg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtdrvxvkk.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gdzeomciv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gcjqiskkm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gjblvzexy.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gbptpzkdd.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gvilwdutg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gtceihsam.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gikowgmhm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gzjansuih.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gpbdhkmjx.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gjrktixac.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gsidlulvv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gjyvyvstu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gvfzuaowk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gvbeyznmm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gdijvcvxa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/guyvnlwpg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gxpekhrbs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gbfzvnify.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gkzitugxi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gxfavcquk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gtdpzdmzu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gscqwbaie.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gcicpfvea.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gwnqswvsr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gjzgiriyf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gavgpezow.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/ggnotrkpl.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/ghjxxhkyh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/guhkfdxlm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/ggdzbswdh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/grmuvzbsz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gfigzzrsq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gucxgjnpz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gmurluzwp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gkysanogr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/grjlsfdvv.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gmczylbba.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gkxkarhkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gwzfhhkip.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/givvzzngz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gdkyhmtuf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gnuzgrsov.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gwmkvtebz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gfwawkzuz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghfttwzrx.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gxgfedbnv.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ghcycuzqe.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gmbcoteoy.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gdywuqgys.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/glbsjuysf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gnoviplaw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gqtbbathq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gutdpmmjq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gicgtsylo.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/godqksjik.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gkydpqadq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/glbsgdbel.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gypyradbc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gjdzojjnz.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gelrntmld.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/guajbbzlz.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gasazjcus.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gkhugvoge.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gbkynatgy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gzibuwhtd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gweihqhgc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gnadxttwk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/glxjfwwll.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gznpokvqu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gnbfpmvrq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gyyurondj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gnykynesk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqmjdwgcz.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gxoohjcff.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gffjujujp.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gfavbnuha.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/guukrmbhw.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gxzilynqt.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gfqpngkks.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/goakcrtka.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/goabgrwbg.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gupeckzam.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gfptuhkat.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/grcatwfnb.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gppmotpnp.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdgoggqus.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gbrowjlhe.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/grgvhckmr.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gdvihxuyy.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gzejlryik.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/glrxtabks.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gwiyfgkcu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/godksbibl.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gxagbunxx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gnsknrian.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/guwucqzcp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gvpepszwx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gribohuor.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gpwqvesfl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gcomzyhow.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gsqazrszv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gvflthxoy.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gdibqsego.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gxwtmjzof.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gdtuoamvw.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gygijugca.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gpwyucpqn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/giunkdagm.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gswgfenkv.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/grxtrduco.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/ggaxzsthg.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gbliwmroj.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gefkdoftb.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/ggncfukwp.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gumnvsqgs.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gvutalzpw.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwkvycal.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gdynbiyun.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gjtlqluru.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gzhuywiir.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gglsvoggx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gpyzkvouf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gszfvziiz.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gsjdmuzmf.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gxoramuau.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gcjfebslb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gwcnsjvnc.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gmslhurub.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/geqgkycqq.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gupynpbjr.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gogyouhxl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gyjkxlhbz.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gffztrxtd.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gddtadgzy.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gshgoeual.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gzclhgirh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gaulcqmld.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gmpneaytu.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gptbbdslo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gjxmjqexu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gpqawdgfq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gimzldgef.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gwcuicqft.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/glzwyaulp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gulhcgmzp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gqjjrehpu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/grlyufpsu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goobkgtyo.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gciqgtdtd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxktfzlac.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gpmylkuik.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmwmnkwuu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gwzvommlw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gwhqoiomx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gdhivjunz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdbimxiko.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grmpjmzlp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gufvzospm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcmayvbrr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gzhihcxko.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gavvaaobi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gttzlkrji.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gfbyoyihi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/goegwovuh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gvbqjiktt.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gfscawayc.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gdiwtzxid.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/geaehpkdo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gxjpalltb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gxdvoxipp.sHtML


<!-- 参考信息 -->