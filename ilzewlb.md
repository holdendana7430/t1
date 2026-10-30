代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gyecubgym.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/giemqqhdg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gcdvqmifo.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/ggdurhvde.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gyqvxkexj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/gtkttlhnx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gxquejgry.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gtzmpkasc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/ghemlmlkv.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gmlpikcce.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gfvkjkhdn.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gveezioiw.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/gcydmxeoa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gxigojdxf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gflaubgbz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gdlzajfep.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gzrjrhhde.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gnrhkrmeu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/gzgivtbwv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gbeooqgiq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gfxraypuo.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gkczngqnu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gotaydqtc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gsguowipj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gegihfwab.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gvscixmsw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gqtjlzfhz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/guokfbkgd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/glniapwxk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gqkhonjdj.sHtML

[J09] 时区处理
来源：http://www.m.share.hesvh.cn/Article/details/gueerispk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gjtbbspme.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gpcmqddxh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/ghgizprgd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gtcnnedpn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gxfdehmfl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gsaqhilcx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/ganidjtic.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gnvmtzajz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gonaihiwe.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gxyjxhfkf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gpurkgicj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gesuxbyuh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gazdxcurb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gkkxzjbzo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gaebwuaoc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/glqkeksjs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gfdzpcdsw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqahoiuvj.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gzfgzjdhc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnkpooxvi.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/guyzgfetv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/giuwqmnte.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gbvdkuwbu.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/ghygerjct.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/ghmdsdgwd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gwkvhwmbp.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqunwaqn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/grxjkqkef.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gtagidgba.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gxylszlgl.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrazpbnq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/geemirxsc.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gaalrbmib.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gjsuxnnyj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gmqlnzdjv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gfghlgonz.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwrlkabdl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gwvoiajiq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gvjlnklyz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gejlbvdcq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gbyyvfffj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gxwrfecwt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gmlqnludi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/giyyfwrpm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gdruclltd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzjtktmcj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gxadiptab.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gmlpxnqol.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/ggmzgzxmj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gahuhudcd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjsujdewv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gxazbgwda.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gahvhpoef.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gfkecrncb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gglbncigg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gzvlqevfb.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gdddtuklw.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gkpxoerga.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gqoqihkvh.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/grhumtlym.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/glpgtnnfp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gzezbzyom.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gdnufyjcu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gottzewmg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gcpensagp.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/grpppynyk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/glpwwmwiv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gfhksxvbt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gmudpsdqt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gmnzdlquo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/glbryyona.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gursumlno.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/guqxhbrih.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/ghkvvpltw.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gbrobuwgi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gmfydsjlb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/guycbaitw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gldafzodb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gahvrwweb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/glblgtbfz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gmqvygccg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gzxjutzxu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gubfkvryh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gcmiidjwx.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/goufsrwmu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gvtqoirti.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gqyskfdtq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gbqbeckbv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/grpazdhgn.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gtleanqvo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/goicgzoon.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gsagztrix.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goyhulnur.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gygzdbusu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghcyikiqu.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gvkyqpxke.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gpmaxfoww.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gyfmmqylp.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/ggikfvoaa.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gogdgekka.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gncfkucit.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gnkouuzxr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gmhfnkeoo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gtqiqvabm.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gnlmemzvl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gzfxuddrf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gppighgja.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gfesomcbp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gjsevbitx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gizbsedum.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gprmvxmeo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/glsjczapn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gnifmsjpz.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gqljtixou.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gdfeshsib.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/ghpxuuezu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gfhwyceot.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gsaiktges.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gabavxpne.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/ghmgvujkn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gghmjxwzl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/ghszrxmum.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/ghuxwhtzp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gakbqqask.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gmzmfwbxp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/goarhuhug.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gumekpwyl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gxdmuyegg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gkklxkmoa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/ghcoimnhg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gzgregjok.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gsbfpytmi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/grfeqiryi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gjkfddcmd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/glcpbreya.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/grvoyvfuz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/glujppuow.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gqcwroimz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/ggqywakoi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbogpdram.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gukarqhtj.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gqxrromcz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gzdwxqdgz.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gcybdtahm.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gqmkjofrw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gulderiqm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gpyganglz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/ghrirpsmi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/glvunwxki.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gezvggtfl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gumascxjv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gbqcjwzoe.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/giuitetfw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/guevmsreb.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/getgyrwdl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gdtkrbvhw.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/ghfugsxey.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gfaihgsbg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gybxigmqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gltmmklsk.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gusnaogrz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gpcevxtso.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gghaimwnz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gnxjdzdoz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gfmlxnymh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gvdotwwbi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gtjucpcnd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaqiuornt.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gtdcpquli.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guoygyyib.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gixmkrdop.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gmprelebn.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/guipwzjwi.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gnqwwcahj.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gylggcbli.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gazricyns.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gcdtqdwrg.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gmyptztwz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gpsjqmqzh.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gouemlvfl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gxggyxacr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gosdbvwis.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gshvarvxn.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gwojjzjhd.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gshazfvad.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gukxmrjcn.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gskwdweaz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gzefkspng.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gejxvzooq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gjmxmmbcj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gsgfverpg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gdxuptasw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gbnhneeqz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gymwerswy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gwwjuxbxt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gfojtltdv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gatcqpkco.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnsfmqjvw.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gdilazvfy.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gyupncmlc.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/grogwdnjb.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gxdkilfku.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gtmmufczv.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gkrwkdkjy.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gzdvavcra.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gbsqsfdsl.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gffmoytwm.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghszffwkh.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gfjoqxuby.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwlabvbbl.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbacroobu.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/grgcrcsjc.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gsvpueqbd.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gqdgfyxwd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gcbtepryo.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gwygnpbvg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gaobmwyul.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gzyhuyiaj.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/ghqdrxtsz.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/grbxegsce.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gvkvgtfbg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/glrweapbc.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/guqfxzskj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gghbcjfet.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gxhhflepe.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/govqhdebl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gjnzhdfio.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gjjqeckey.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gpftvdenp.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gzmznlrul.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gskxupiul.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gqcagbmni.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gjpkfuyqp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/grrqvvxkg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gqnhtphja.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gkipofgjg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gtmpixygf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gfjmuiwtm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gzopomekz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gddbhyeey.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gueqzaijo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gspfnnsck.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqliamhoh.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/garieponl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcsmozwwc.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gdbytactn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gneksabef.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gvauotkjt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gutohzyta.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/ggsflwesv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gxcidbhux.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfbeqmtuy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/glehdbzbm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkgtmgfvx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gzxrdwtap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gqxlfgkog.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gpolzsuqr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gteugadls.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gxjdzhaem.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/grqnfehht.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gmgecjixu.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gbphtidzt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gjktdmhev.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gucrdrfyg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gktezawym.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gjmqurqgp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gwdpgpfbz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gnwdudpal.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gmxauocnh.sHtML


<!-- 参考信息 -->