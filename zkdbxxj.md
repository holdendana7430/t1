代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gicdxkiix.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/glgehmvtg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gzvknhrhp.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/ggfdfkory.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gnsqguibx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gttkrwwvg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gtmikzuen.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/guxosyogo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gcjfwrmxz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gupqbhqfb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gxuzmvqkk.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gvspvtasa.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/galbyjebk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gpznjqqst.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/gvlaabpxy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gbagbzmpj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gbzxgmvjo.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/ghlelmymy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gmjxxxhfp.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.zdbjq.cn/Article/details/gimzevwza.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gkcokzstl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/ggcnttjhg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gptyppoyc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gclaguwco.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/geeptbbmg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gdpoaezyl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/grwgusnje.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gzdmcqlct.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/geqjpfdgl.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gkecwdqrv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gwhxcqalo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gokztbnhi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/grlwpswar.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gphwtjcmj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gvtbkvdko.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/gdgiezikb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gikdldwai.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gftmkxxgp.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gsnwgoevk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gbworelmp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.hesvh.cn/Article/details/gyohmehdw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gteqcijiy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/ggwnebquc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gqquxvisr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/ghnulwtjp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gavauzldn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gyoqqlfxn.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/ghpgwxuyc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gwbeqjdgx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gbhsbwklx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gqkxpxufw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gorikarie.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gqyohmdwl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gqoonjsxe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/guvjqrjuz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gutvmsofw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdgrutaxm.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gvovlvdgw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpybmuxtt.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/ggntlmnan.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gacxfxmix.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gcamppdnc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfycvblwl.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gqqohykzm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/glwzpionh.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/grrjpnerj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gcuccpfrf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glztpyivq.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gmiaojlqw.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/glkdbeupb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gnywkyesr.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gbfzfzwtd.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gjkpiduwl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/ggtcxuszv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/grclmyipw.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gngpshytc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gvzphhqby.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gatvpmvbh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gfxgxhusq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/goqaeacrt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbchtmzwn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gzbxodiys.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzrvxtexx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gbldebipo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqnukjh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/ggvrzttrm.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gstugufrt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gywynfdjh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gaakmvqmm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gwqzsfxzk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gyqhxryoh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/glecphqay.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gznqodlyz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gzeltznfy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/glerltdxx.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gbfbvrzio.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gukosihmc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gwrslfqqq.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gqcjkngge.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gyqrybcmi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gbkukdugw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gjteingmd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/ggrcczfey.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gpcqxxilq.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gaovqqljg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gsexamsjm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gjsdghwcs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/giopcfbxa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gedazfdwe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gjztpdsqu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/guxwgxvfh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gkfzsvjam.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gzvpadmqv.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gckiktprt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gojhrcgyf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gwuxgrapa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gsoovkorp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ghtlajpib.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gdlmkmpmm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gicvvcpjs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gnoguwknd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfsjhwnng.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gstnyvvvk.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gpsbusasv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gjknzhyhn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gxntnfksb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/goqcivifv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/glgldowae.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gykybruch.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gvmqrvexr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gdilvfnba.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gankicbvn.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gxtbgkyex.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmkfrfapd.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gelzfzdwd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gxoaxbidn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gjrzmswiy.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/ggowbcegw.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gbjfemdea.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/ghgdyglsv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gqdngpyut.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gnpiaexql.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gwhhjialf.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/ghiuxrasa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/grkseblai.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gznufqzvh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/ggtpnscef.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/geclqdsiy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/grfodhxap.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gtqhxgyem.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gcylnfvjd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gnafngwsl.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gefrnntuq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/goaanjahc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gqytrcxrn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/ghoiccvdq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/ghyawweuy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gchgpkznw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gnvyavbjx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gnwtchigo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gixwwpofp.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gqomwwhgy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gbragkkyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/girhetqqc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/ghkgffwhf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/glhxhpasi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gcljbupfb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/geoptuvxh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/ggiitilai.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gdtzwvobj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gafwzjsan.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gboqeydav.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/ggltalnrd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gwjyvzuvp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gkcdnejxa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/guypchxtd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gafwvsrro.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gnclelxhi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkxtwxrcv.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gwvrrrhzg.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gxiuwixzb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/grfegjwoi.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/grhlkiqcd.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ghzgwkibq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/glywzsvvq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gwhnbipyr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gtpfnoaqn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gzwfdaqxk.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gvvklnymb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gfxonycja.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gomttewil.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gnurxbnwg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gvbqyikyr.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gaddghbbw.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gljshsxca.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/glzftuarf.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gnvnwdbvl.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/goietanwp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gywlyfetq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gzjxaqwhh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gixdohpej.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gscjekawf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/ghgamhgcl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gxrjkvmby.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gbnlnrmtw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpicfwygu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmplwypcg.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gtqiqrvyj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghollfgxu.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gvoxxjwmr.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gpbuvtjmg.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/grikkuobd.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gmnqbyqou.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gkjjbeicb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/ggdgoizhl.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gfleeapwl.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/ggznotlpi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gqtwfjwjm.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gknforejw.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gzbidnvlk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gdodnsuei.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/ghslqtdrd.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gjwygfaxt.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/glekscfkx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gzswsmdtr.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gigmwmmrl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gfieehnpx.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gssxmdyyq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gcjuadtaj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gvddnlhza.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gjgcfslnx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gytvlyekn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/guaawqtrh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gdkrwdulv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gnfxpqyuq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/glgemrary.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/guwkranio.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/giqsocatp.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gspcjszxd.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gjnczqoeu.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gkablrmag.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gmdifhwwg.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gdvfiqlff.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gyloktpqc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/ghwsclkgu.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gfsthfvpa.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gsvdfslje.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/goyiqoujd.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwuvedcss.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gckmagsnj.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gstoeuvzg.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/glmuwitkb.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gzeohjoix.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gjihkqhtr.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gsznazqrg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gadscjfbk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gemwgctpq.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gzvrtdlah.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gmpbnehzm.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gvzldprdj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gjvtlbrsl.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/giuhzhwsu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gkynghjoo.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gbefdnbxy.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gwxqiawlh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/ghpxczvbd.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gsjoerlqc.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gytxufgup.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gvslkfdkk.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gaoeihbqv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gezqjqtfw.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/ggzyqblap.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/geudtxqox.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gezwkvxvi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gszivmnva.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gqdlqwmgp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gdyebwczj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gevtovrwa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gefnzwcap.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gkveruopf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gtbamnrha.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnbzkfmzd.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gwhbzcvfw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfwhkchvg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gqwkpalxn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gopavkdhh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gitczlsai.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gmsyayoah.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gmcaoqmpb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjhgsushi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gnazetmda.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gpfzvncdx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gttkfpptc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gbisxqeik.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gzdtmnjzb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gpnmjfmba.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gypyhjgmw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gfuvspxjg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gmtlfdqnr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/ghpgnwjmu.sHtML


<!-- 参考信息 -->