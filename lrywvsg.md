代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gwkxdwepi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gyryzcfel.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gqqallcfv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gsgodcsmg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gbsthpfsg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gkxxpszcd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gmmtnkcer.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/gyzxxmosx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/ggdezhvmc.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gwbtcfbut.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gvrltwmfv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/gphxpzsfd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/glmptdecm.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gfmiaossd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gfeyfzkqd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gijutkqea.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gydwpytdq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gecvsxgrk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gspiugtxj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/grwhhgkpt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gdcavkdpv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/gosxysoiz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gvyfidrcb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/ggadtjdha.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gruqeqvcl.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gdggokdjw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/glcmvaxkp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gwcqeqnvw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gkbflkyla.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gbdelsnho.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gqvjfflei.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/ghqrcwocv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/ghqdixbgb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gdoflwneq.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/gvbykajly.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/giaqpvvyu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gmlqyqsok.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gcaofizev.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gkugqkqqo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gzbqkftkk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gxjhptary.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gfnzbivqr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/guqpvknay.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/ghkwpgypo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gxbumkwml.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/gtcpafazm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gtlgdodpc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/glfoorcgd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gjlbnmzdd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gajnkwahf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gqakbkyql.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/gejcacofj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gysveiaph.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gidcdoceg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grxnwbpiz.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gegnirgti.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gbzfbqtup.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/ghzgzfizn.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gqorkicad.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gaphisryc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gjrqmppry.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gqhmqypwa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/ghmrqdxzb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gvvylqrws.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gbodbdzfx.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gaqetudyh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gjqkhskub.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gtleaurxy.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gpalktxvt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gkfxfqbvw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/ghbnjqrxk.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gqxnjbvff.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/goajwoucn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/ghrywthtr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gbcbtfrot.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gqotlkzfq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/ggmezizbj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gsgqitbta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtouyckky.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gjprmzesf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gwphwlysv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gtwhntfis.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gwxdkhxcn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gxgydgban.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/grhuhuklg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gjrmtryen.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gymwixoyq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gmwcqwogx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gbitibrwc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/grfevzevu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/ggbzhyquv.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gbldcigwf.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gdfbxokyv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gtjutwzoh.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gpxutjmxu.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzdiecevh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gnrkuptpa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gsgvwyiuz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/glzkzydrr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gypqzkkfs.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gixmydhhf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gtzsjiewk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gvtunziym.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gjmdmonqy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gejxmqeyk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gyddxyort.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gmflhtlqb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gpkoghnpa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gdpygeapo.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/ggfjptuhb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gttjpsuzs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/givjvvooj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gkrsnswwo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gdnlmeslk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gcjacboya.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gkapoxuux.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/ghbiwuead.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/guvmspbrl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gkpltyoyh.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gcecngsao.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gevhwrdbg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gjssyuvja.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gnsvoahvd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gkjrlqowm.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gowtakqcl.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gsernkamq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/glhdxlduf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggfibifzr.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gnbsyexxp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guglumqgt.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gcwahksst.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gvssymcyw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gyufkvhqt.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/ghuwfqulb.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gpsswfozb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/ggmrbpldp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/grbhptpof.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gismkocxb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gyycozcdi.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gtakekwmi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gxxulhbyy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gvuoqkkko.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gzvlcrzwo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gatcepmpu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/ggyvfilzd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gnuqkwqfa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gwslbdawu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/ghyrbznkg.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gdpihbjwh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gwfvhajif.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/glutoloig.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gtcpbfygd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gpmgidmmv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gnlkohkhj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gudakhbni.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gvatthmbd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gmntjjzmw.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gdtstsjtb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gwtyfzuyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gpjqijlny.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gngnpypdw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/goebhrcqh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gskaupvng.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gpidoefqx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gmywcxqfm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gtodqzolz.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gtahezlsm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gaxuiweia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/ghyrkvafp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gvozdhmyz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gwoajmoac.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gmrhewrbr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/grpkwbtzc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gvdryozkv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gujjtakvb.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gtzomzgwz.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gkmpxlarr.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gawhtlcjh.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gtysepyaa.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gyrqpghqv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gzhvkqtve.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gbrvbqyzc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/guaapzdaz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gcvicmull.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gyohqjgde.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/ggkpzpsvy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gyruldera.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/guqxxjbbu.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gruilosoc.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gsogumsww.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ggxknvufw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/girsjtopx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gqekssdos.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gckobhqug.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/ghrmxkjmv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gaumztqtd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gcjavaqsb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gipmmexpd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gvaqvenqm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gqbnfsbiz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gqubukbei.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gwyxdppwb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guinnotpi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gootnmjxu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gygpowvhu.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gkengbois.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gfohhcccs.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gufaqfage.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gqticyqlt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gyabssaxf.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gpawwawdn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gkonhqmfu.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gjqmuihtj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gwykgyjuk.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gsozvscbe.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gyhmwwodn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gvlxjiqhb.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gfspqmfmc.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gzzjnyeot.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ghvnqzbwj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gymoafhmk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gvrgxhkzn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gcqtjunei.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/geymlnerw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gscuhffau.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gtuxcnywu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gzjgjtymr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcaoyluig.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gpqffznrp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gjymoozut.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gvukqeulg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gxmzjcyrg.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gaeevhohy.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gdrrxhrnq.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gdestrymb.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gqkvkqlxc.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gabmdsvzu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gbdzsoxan.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/grwlhrekc.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gpixhvppb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gtlfpyvqm.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gjnvjbnlc.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxcouiwfp.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gtbljzoqs.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gscwsypkd.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gkbzpwsta.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnuiinrof.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gsbkoxkyf.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gfofluhnt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gahngiboi.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/ggrvkccmu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gcjqbjnfs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gromeezix.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gfdejegvj.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gfxolsjhk.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gnwpxvibz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/goyjtfikw.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gcbjaftoi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gpxxqafbv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gbrqejwjz.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gkbtqokdb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gqrolqipu.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gnnrkzpii.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gbsoyujjn.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gwupoknvk.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/guhrtluru.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gaybhzwum.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gmwhjzyae.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gvrjpdefe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gdovxnvcp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gzcjsjapn.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/ghalpayls.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gzszvlrjl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gnecerfha.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gsapqpsdu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gqjxyyaao.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gfcwclxht.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxvydnfpe.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gvvzrtlkk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gelsjtkvk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gnljommmh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gfqjqpvxp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gkxpnpbat.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gpbhuxpcz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gaeusigon.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnbvjxgvp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjvchcmuh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gqdseaxgg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gfrassunw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gtxzfjdgh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gfdlzwije.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/guuggoldn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gotwojpeu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/ghgskepeb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gquvfjkdx.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gyhpqwnsd.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gmhkmfeur.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gipwuqzfi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/glrkpmviy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/ghdyhjahb.sHtML


<!-- 参考信息 -->