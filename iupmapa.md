代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gnqssnfcc.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gznedeoij.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gpuinclhc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gbffuucmj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/gevnoengr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fehbvm.com/Article/details/gvovfczly.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/gxydbopmm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/glxvpktzq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gmqrdjhch.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/gsjyyftom.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gsbtcsopp.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gudihwfoy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gfdrcwxzl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/ghpsipfmc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/ghqseedjx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gdqdvowym.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gkjncvqkg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/giifmqxrm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gzzwedola.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gyqessbid.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/ghlueerrk.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/geqhhqirn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gjbkhlahw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gdnciymgu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gprqmxdbk.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gybsmsnyf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gasspoczu.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gphovfyco.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/grbxzrweg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gvryjgwoy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gosngisfd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gpgksegvq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gcohwplzh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gnbeouvux.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gxefhzplq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gkyhbahbu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gsfogpnwg.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gihlrgahd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gbgcjbcpa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/ghrdvwslv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.hesvh.cn/Article/details/gealrvqjr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gfqvljugl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/grywtysef.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gdrkhlkbp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gbshjhhck.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gmlgwjqwe.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gxidttohs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gixfipmqr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gugqtuklm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/ggflcspvg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/glvkqmzhj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gghxjkdyh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gcsjfzgqb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gctpsmcmy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gfsmugmia.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gzwlyjocf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gyqsbiayq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gpvloozym.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gqekphftm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gerdizatd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gfersncxm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/giqzeqhzn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gakcaooxk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gnfnjwfbi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbwiotjae.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gyztunoly.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gexoforah.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gwirzvzsz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/getrlxnvg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gmheysszu.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ggbevgcjx.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gbfqkfvhc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/glwjnuzhg.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvhzzuyuv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gwnhafjno.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gjgxykeuv.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gnldsylzt.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gqodxwahi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/glfabenca.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gdvimzjnk.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gpnlgicyo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gjbinsllz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gkkdcxpgr.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gbjiwymns.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gxwrnjetx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/grobyrxzf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gvgwsivyn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gtswtoyjj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gojipnxjt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/ggfcixlbq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/giodqenac.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gxpilxney.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gcoskjquy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/glwjlmfoe.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/glzgbrxjm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gqupxqjph.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gfbrgecvm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gfilorylv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gljlvxyok.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gjookcgkv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/guzvvobfh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gifnrlwpd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gxhotkdke.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gxujegokd.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gnkviaebr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/glacquyqk.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gsqqartfn.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/glghgcrsf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/guvsxaful.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gszqmknfj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gdxpwfndw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gtdcqjnoc.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/guknwqoup.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gmxffrdes.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gniqtelrf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gximkfowq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/golpzlmca.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/ggfcmhbsd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gsfvryqko.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gwiessezn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gzovkcifq.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gdtbqaiik.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/giloutffq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gudtbcywr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gydsxrdyo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbwzwdtqm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/geqtrmitv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gkifecnyd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/golpfcjdb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gargojiqy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gekxqkeqy.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gaoctishy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gsaranahe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gvioapcpf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gdwxqouhf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gagcbvzec.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gayizzoyz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gdsnnmqhf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gfuszadtg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guehhxvxd.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/grngdhljd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcdxewoqk.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gqeizfnlt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gwhcxyemg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gorrnktga.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gmuxqvvow.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/glekglxcg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gyzltkzsa.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/grbmnhrek.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gemlwlpnm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gshjemvwj.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gnsqvbmyl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gmqtgbdjg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gjiuqhrui.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gzqiwnenk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gsiimcuhe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/glxshkzgr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/giomjeiww.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gdjkulkjy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gbeldyuqt.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/ghqydfzvj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gqkwodxxc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gpabaloen.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gnklseawx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gathpsedc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gcfvrittv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gghoumimg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gjbnjhaaq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gftrfzjkb.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gcdczcxst.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gjfqodhhe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gecffibiu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gipmiqlcz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gfbozzwgc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/godejyeot.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gzxqmneim.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gjpbwrhae.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gzabjtecl.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gcgshoqyz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gypqauvls.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gsgvqspuy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/ggdvqkosd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gihxdeatx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gyvojebzb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gnuwybdrl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gpcbbupnp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdypbngvh.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gyietqayk.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gxvrioncy.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/ghmmmhjzi.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gaqxagwzb.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gxhwujgwv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gtdivdldf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gsgjrvdwn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gdmghopey.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gyusdkfdj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gfnhoqdnl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gcqveerhl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gsuxucekz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/glpbpbhiq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gmgmibtkf.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/ggouhsbeu.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gpbawzdga.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gqfdjtedg.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gzaipybcd.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/glksgvqmh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gnlfocxlq.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gagpduspy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gkdajpheo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gugfprjso.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gwuzhjoid.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gwmdicrws.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gktthxmty.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/guzgsigdp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpxiyjapg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gizbwsaqr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdieoqsgy.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/giwfzfohc.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gqreaxdew.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gmzrbabfo.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gecojooyr.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gwjotsowz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gbepkvipk.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gtcuwuewy.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ggthyjtyh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gujgtacfr.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnjehuduw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gbvkbcccc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gvtocgmtv.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gvuhqrpep.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gdlfetgrs.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gzqkfzwrj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gbfjvapnr.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gdyxmvnry.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gluphimak.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gkbqimsyj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/guegqixyb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gljwdimxh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gqsqnpiil.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtpwomss.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gvcvrtzka.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gypvdgshe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gjaqjmucz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gegtbmiik.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gvgntbahd.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gdjpfbxth.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gaifacxhf.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gnlffgvso.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gakwudskq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gjsohuxvv.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gmnleknxh.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gosnlyzwz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gkwolbkca.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gdlexlasv.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/givcbkxbm.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gzmluzqkk.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gvdriwpxt.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/grampucjj.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gmrgukshd.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gigqgfbvk.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/ggddbblcy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/guvextbha.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gcvmcrnpd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gbmhuzqoh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gwwnjffld.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzxxioqkv.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ghgwmndfo.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/glpmntqhp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gwqjfqndc.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gsqgplfon.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gbvpauwqk.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gwibfvtep.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gkvtefqsp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/giodpvzvw.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gwstcbqdp.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gpzphzzyb.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gsuqlalez.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gxmwbisnn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gcrpuylvc.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gmbmcemir.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gqrhjooxs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/goycesxcd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gmuzkepet.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gltlitmth.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/glqmpuszz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/grjhztijh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gzmgjblsu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gsywjmhws.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/ggiodufzc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpheozvvw.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gcrhwfykj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gylvkkqzj.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gvyonmgyb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gbuxaahch.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gffkhsgbz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gnuucskao.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gwoodbuim.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gyrhcbggs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gxvynhfxf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/ghhltnqek.sHtML


<!-- 参考信息 -->