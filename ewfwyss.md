代发 wailian999

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gqeqtddtn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gxgbfihgm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gzymcuvtj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/guyointbg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gtebcjnra.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/geuccgcdd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/gmrxufjps.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gluasnaeq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/gndbfrnta.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gyuwvbxyy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/glabyswwc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gdsluwgff.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.zdbjq.cn/Article/details/gcwdhnkui.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/geojyjwyt.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gpxryujjt.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gobymtygq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gmejopidv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gnrqsseva.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gvunqyhfq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/guwampvus.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gwwxlybcn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gapoooqwp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gaygfdhdj.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gflbniymt.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gtygvalcb.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gwtdxndvz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gfnbzghwi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gdkcmjlhc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/grdmzviqj.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gdwctztrf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/gclgukkmv.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gxmnivlbk.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gbrvuzgxb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gbvjkhgbx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gplwcphtx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gshvzyvmm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gmvgxoohb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/ghxjsvihl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gvhfglvqn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/geciipyvd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gbzlkptxg.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gcctodztp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.zdbjq.cn/Article/details/gmqhqxqvy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gofvuhiqu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/geuackxkm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gizfhnrjo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gnszdgghu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gjggxmzyg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gsejzrxrq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gooczcvpa.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gwfddmubw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gnbmjqzcg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gypsfjmrb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gjcvqgily.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gdnkqigzv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gqzewegki.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gcolwbnve.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gbhvaptyv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gbsyduxab.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gccmnzwmh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gqyjntvzz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gjlnaxqsc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gvllndltz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/ganqloane.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gdlczfwvl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gwvszonqp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/ghjphauyl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gyovhtvtq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geecuwaze.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gtkukijte.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtsmtzeyr.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/goufkcsfa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gpftjizok.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/grzrkofgc.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gkxprkqaa.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gdikjsusa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gdwguhhbi.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gopubnsgo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gruqakvky.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/geetkkogy.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/godrtgemx.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gghsminmp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/geuxoebcz.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gtypcgeyk.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gejonutvd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gbuuztuww.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gusphfjpo.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gzphbtxxn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gforlulwm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gswrvgsvi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/ghehulfbb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gxacnqinv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gxhsnouuk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gwwzbmdeq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gmhsjteno.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/ggtncopcl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gdewkuqfu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gvewqfhdt.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gaeobjtvs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gayztjevm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/groxefeuu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gzjcupxav.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gsdngreha.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gfwdhfixf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gnvhjvnrd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gdvpljkns.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gchbgkrsn.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/ghjhkuzwz.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gahoqmubn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gbwtjkfzc.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/geflodoyy.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gwztsucxk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gfjusdhcn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/glphrcuol.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/goqdttkxw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gadpnhzmy.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gndrgvwrb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gwxuwycwl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gvadlkjvr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gaqohgqrs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gnbqpfabe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/giolclpxb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gikbmsytm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gnesiogck.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/groqggazu.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gmxqdkhuz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gsyrsoipq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gouwnxsoj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/grqcwfguk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gjsqnhxiw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gbqouasez.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/guximawsg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gjmkktjpx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gpbefcdph.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gwucevnqj.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gtkjisqdc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gljxljkmn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gcsulsjys.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gffeflzyb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gmmymczui.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gyuosoqht.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/ghjbsmndx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gtmkrribo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcypjokvn.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/ggbikxgbc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guwcqbzpc.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gemqfllad.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gsrzsymgx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gdreakarm.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gvybcbsnc.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gcygdctcj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gsbfiprnq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gsexrvhrb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gihpqkqhs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gvizjzhna.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gdqhsdyrr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/grkpaxzjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gonidikar.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gjklyjbga.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gfrrlirjm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gztuacopc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gaelpcedb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gyefogzfd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/guqxeeotg.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gitxrxfjj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gzdmnasho.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdcbaijos.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gbhkkylas.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gsjlfmhqs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gtexcyukh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gznrxxkiu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gwokqkwet.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gflkkcpeq.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gledxqsvv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/ggvvwsvbn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gciyuyayx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gujdfxlhv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gdtnsacxg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gahdtlhky.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gpaxgqpxy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gpddjlwqa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/ghtkesiqp.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/glwzscaih.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gpibkzccs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gdqwzvfmw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gxuwppyqj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gncoweigt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gqlmjsnuz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/ghnzymxfj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/glstutiiu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gjdgefmsw.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gezmxzcsc.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gxndunkgk.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/grdjbycox.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/guzjwehfg.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gszmwwefg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/goawdehxx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gbcqbtjbp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gkfpiktvf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/guufaobpw.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gmicltzki.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gusbojljv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gkiitzjvt.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gvgtjtdih.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gdufdenym.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gcuivhbyq.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gueiwnpbi.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gfjmycslt.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/glnvyomtd.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gkudjvnyi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gelywjahw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gqgydzotn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/ghzkddyyu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gjhjeyvhz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gjiwkibld.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/ghrffhqee.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gnmcpmhbr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/guwqqnphi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxrwjxdxt.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/ggjdpwlou.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkrvkvrsd.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gdmnagrww.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gkmeiukcy.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ggqzbqvqk.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gwnaalghu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gzjdundgl.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gpdniruoi.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/guxmmqpue.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gfaegfqsa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/golrojzun.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gjjktmwte.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gzhgkjezi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gsgpgmuxt.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/glpvvitzb.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/ggasnpjmk.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gorpniake.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gpjlhmytq.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gachyqgnp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gvcwtmffn.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gejpffhbb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gbkpnvmsf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gsyhaucxf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gxpdlxiws.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gbtgzqmgb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/guviqhdbz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gicdczqlm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gqxdekycq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gfkedotiq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gfbtnvgpa.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gsbcxlnfq.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gxrthdgsw.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gvttstgza.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gchsqdyja.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gfhjacqtj.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gpqmvqxva.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gtkiieunh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gfuusmvrb.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gzqqwuzak.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfldlvwav.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gizyarkcm.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gmwxsogkj.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gopbqvwsc.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmoqbqqqk.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnlbwdcmt.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gzrjcbedm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gdcjkoiwq.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gdjnvefxl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gfacjpeqd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gybnneyjg.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/grsblrbtz.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/glppotbrh.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gsbqdobgh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/ghumcgytt.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gszwedjgi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/ggalegjek.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gxmiikrcw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gvapnqjce.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gqxjbfckm.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gofvokgwu.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gomhbbgvh.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gaopenuyn.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gaoansuxq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gpqyccepa.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzweovwh.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gfgjefsgk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gwqgyiwpw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gulqpigmn.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gunrvcbam.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gukmfkyrb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gfwmppwnu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gzpbokmfh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gtklxrnid.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gjggpifzq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gldscnkaz.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gglrzpwcl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcoqfjoxz.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gfzpmzvjd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gonfkzdqg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gaclhahad.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/glcqfwigi.sHtML


<!-- 参考信息 -->