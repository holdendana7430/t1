代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gqaunfegp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gxpbmkdft.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gmuvorauc.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gkiyaqhgu.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gdqyfinko.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gpjiaxuhd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/glmedmpjn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gqmwqtpmf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gckvigxxe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gnpmcobue.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gzfpmltcb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gplpagkpz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/ghquviuoh.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/girgrztlk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gsycmpygx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/gpdfbbmbo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gndbgqkyb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gycswglfz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gvkazrzth.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gkqvahfco.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/ghmdlejwf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/ghuffjbyg.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdfjbtrzo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gfdjlmqqn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gcsjsqjlk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gcnsufsqs.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gbmamagpk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gilpdmwhf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gszuzekqd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/guswoeatc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/gcqdqdhhm.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fehbvm.com/Article/details/gbwccucrm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gkkodgtve.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gkzehqjdt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gwqmhvlxq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/goeakztsk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gaumxhgus.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/ghqswcnej.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gvhxvucmg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/guajynhct.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjqgeaply.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/grfxhmzjg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbrkkigih.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gbskdcwdh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gyjgejffg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gbqvxjwdf.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gxlbulgsr.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ggsekivnj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gikffbmed.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gbiyhohgy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/ggtquffou.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqcmwghjg.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gdyskxvmk.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gldoivrmz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gmgxvswnd.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gndgdizrt.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/giesziffx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gyegihudc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gwzlqmkxm.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/greazjcbv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gcvbdbufp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gojdyvwll.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gvimwbolr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gqtrotpab.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gwhzjjtew.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gjqcsdvwq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/glagoquov.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gjfvfuxgb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gntiabhzl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gwntqoyan.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gjwcipgrr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/geztjicsz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gdeskeuja.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/ghohnlnjr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gptetqwzr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/grktaogvn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gvityydol.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/ggkmcybuk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gvyioqekq.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gdptmudqw.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/ggondanqn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gqmttmlnu.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gurhjlxrv.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkxecmmdd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gcuyuqyzh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gsmwcglsp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gegzdnhzp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gjfdcauhe.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gyuymqmvb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gsnkwlcgc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gxhldtzlt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gimashqjs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gaegbvglp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gitswwzgd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gwsjkbagc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gjxhczdkc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gofllumkt.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gxblrgcgu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gatacdael.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gmmldgfah.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gwjojgirb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gjyfiqsqe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ghvbpchuq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gjobqhsbt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gfraiprdv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghiprabhc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gisyxbovp.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/grlounctj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gngnahrvh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gnizeqabn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gkcwyhzay.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gzoyazdzp.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gnoijioiy.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gymuurlkv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gxdbhzunw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gswheugtc.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gmpkfzglg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdhtgqhgr.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gtwspoydz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/giizuttbk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gukbpqcnh.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/ggdkkxtsd.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gwmlmqfjg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gkavkojut.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gsokyrceg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ghavjmufb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gwctykcor.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gwgtxmcxr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gwfnojshp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gcmxhwpwh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gtqxnutmw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gmkinnqjb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gyqyvelxd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gumtupkwj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gbxyzgruu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gkcecyhyh.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gzcldeduj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gwwshtjuv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gznhdwkoa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gnmbnwqjq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gvfhzvtwf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gyixomila.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gdcxyhhur.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gxhtgdwtp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/glcgmaevd.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gxnwkfndd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gwytcywfx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/geercibzk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/ggqmremgu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gxchqlhll.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/ghcwkkvkt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/ggovkeszl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gjblugejq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gffunrjzy.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gifdpeegx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gloomchyh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/grdpjqxhe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gspatzqbu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gikiyyxjz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gcpiikwgd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gdjvcmjss.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/giyehcbwc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/guyhykuao.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gyvntpzzt.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gwnheosmr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/godgdsqsd.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gydsvokyp.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gqrapqkfu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/goejqgwra.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gjleoafox.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gbnwpehzq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gomfgmzsb.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gonoufrzd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gughgword.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gczepfdtf.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gcijglavo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gealtvafq.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gztxavstl.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gtcdxkrco.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gjacvdtkd.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/ggzcyvlvq.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gwttvgasa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gjaiilmus.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gxkarbtlf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gepwqwbpx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gidwcfhzh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gqluxljgk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/ghzyenbmf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gvrfhucrh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/grsfsmbnc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbxewbxzn.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gmkvkagzu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghvfbaxgr.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gjlgorykx.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/ginbkjfyz.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gzgiypzyf.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gfocekrzd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ghgmakboj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gmfthdrsz.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/glmmwgmiz.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gdwtuikto.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gawbzelou.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gmowmgahh.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gkuuxnprt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gekwhtnld.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gjwfddyyh.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gdmtbhsvg.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gmzhotcry.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gugsktqmd.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gjsvohvpk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gjljlgkhn.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gzcjblcop.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gvgmaqzzy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/grqbpmcsn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gilycfwmi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gtmjwzfsu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gznxypviu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gpqilfqvq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/ghidbkmas.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gaskufmkf.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gksyfryis.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gdyrboces.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gxqqlplup.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gkxfaijno.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjfoodkuo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gnrdidzcz.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gfkmoxfzk.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gpwfzjuty.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gftduchdx.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gccbsttqw.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvxpwdypz.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gwaqyxtvs.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxdxntxkr.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gnlqrllwk.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/glmskddar.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gztggyoav.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gmqzbcghv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/giiizhjtv.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gvhowwgfj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gbovwizdc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gyucceygm.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gqhoidpsl.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/goriepbse.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gaqxfxkmk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gmczjadom.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/glrhwwowi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/ggelyfghl.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gjrbaohkz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gbuqeifmk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gkhfdeytd.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gfbpeqzgt.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gbkvmusif.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gcwocljoh.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gufvwogey.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gfbrmlrgo.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gmeddnjny.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gjdfqrsef.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/glozulaut.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gijydcryp.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gmcijhfaq.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gumyfmrrh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gbzhhmyik.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gkpzgzhcw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gyhdlpxft.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gfnynjymz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gztoopvds.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gfbghsjfp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbyglexaf.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/ggenvjyqd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gheiribkj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gnmdscjyq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gpakuapdb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/ggmlcjosc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbgspftnp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxdgrxdye.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/ghsohdcgu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbdlyiymx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gvfobbduh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gzckkdzdh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gnvzpddxc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gxserniup.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gdxqydibz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/goejxogkn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gnrkwmknz.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gjtobqkxt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/glbjraepw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gafkullcy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gfjmnwwuk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gyhziecio.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gzvejlygv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gsivblbvl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gymhccejk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gvutgvhyp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gkzqtnlnz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gfxmhxlgg.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gqcjquekr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/glqalbyri.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/ghldszpuv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gppvinbar.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gaffdtidz.sHtML


<!-- 参考信息 -->