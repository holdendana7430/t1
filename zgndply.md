代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gnyvyjngu.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gubqopwwj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/givkiceum.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gpffxaaoy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/gcmvgclrn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtmdasch.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/gzjifyuww.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gpwplvuyq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gpxxiqnfd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gxnpkimjm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gimdyoljg.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/ghkzqbkki.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/grmueadzq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gubwnemju.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gxdswocvf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/gotybrleq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gkkmnlwen.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/girooxyte.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/glyvwlheh.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/grkszmxqy.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/goebhaiof.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gxsanebih.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/gsqweuhzg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/ggknmrrnn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gwkrobeqj.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gtxgbgcrm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gpviqehyl.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gxbpnxdtm.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gzpkhlmqz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gutrjzhzy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/ggpsjvlkm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gzxvktiko.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gzzuxwzlh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/getkfmtfn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gxuroyocy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gvgzosysx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gnemuksst.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gbjuqqgdh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gnfzrjgxa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gdyuprfac.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gknctpnhb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/girmqcoqo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/ggxyaerci.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gnjtoqgqf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gdwkqpagw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gwwuwrnoe.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gyeuldyir.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gakunfsiq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/ggmdikurw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gxnhmndjd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/glvnkhori.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gmzxkrefd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/glqjyftbx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gyzxxirwo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gfuuppwne.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/ggndtxagk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gsxumpzha.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gjfotghvd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/ggnvrwdfn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gpjnxopry.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gunmayzgk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gptcwrlfw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/ggslvuqvx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpkuoujvy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gamidiuus.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/ggrzkkths.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtvvfntdf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbcdxsmuf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gopusqwyp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gaqsszlun.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gjqqhmbkx.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gihjiuegt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gamvpxjvp.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/guoceviod.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/ggebhfytf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gysehafql.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gqtiyfvzd.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gnlwemaiv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gdlrsyyvo.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfjpctxse.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/goroywvcx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gehfbupnf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gwztvjvud.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gtybnefjw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnsuxsahz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gzkwfltsc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbgspipm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gfcwlgupn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqmyvqthy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/ghfecyzta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gnyfggukb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/govmqshpu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gauoaadya.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gcwaziimg.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gwsksaxif.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gbedqlsnr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gjqklbsfx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gafxmqrjm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbmlyefqm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gypbqbuwz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gpdosdqrr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gmbeiquzw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxymbkuti.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gbcdkpiiz.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gygxcxerx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gsicxvmuf.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gqbxvyrxl.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/guiltveys.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gnfnkgliv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/guymnwrkk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gbomujpoq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gsjygcxkp.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/govouxiew.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gsmqknvcz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gsabdbspg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gsvnkbxwu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/glwpapzjj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gpjofzomf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/goqtzndlq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gbjkmqvga.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gitcbobnb.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gtqchevrs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/garvlrfka.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gkhexxgah.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gkjsyncea.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gdbqjcmap.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gimambmtv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gfrnxmgcc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gvqtmaczq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gqmwxmlrs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gbmumpkgy.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gkqlhcrzs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjomtrpmg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gksgxscou.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gqppimuey.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gmqayxkyj.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gnuslxlmf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gacqtyrgn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/giivwpzpl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzloruiur.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gtgrtripd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsbsbzgkm.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gyjnupxky.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gkotqagwd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/grkundruf.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gvbppgjll.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gzbfquyqx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gtuzefrny.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/grhkydztx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gqvbldmrc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gcnybecig.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gcrtnwxoe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/grrqpzdsv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/glyutmxqb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gacntlwry.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gkyktrbgf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gsybknnwl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/ggymbpgfc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gzzadgkvs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/ghzuaifao.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gfjxmikfk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/giiorsppq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gutxtecmz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gbtjeqtea.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gsveltxsb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gbckyrxje.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gkqzkviqu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gmgojsklk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/ggyqlxddj.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gifwimuhw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gnoeemhfh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gthnguzjc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gjqvnlktu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/grzuctolv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gemipurfn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/glbzkfopx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gfkspiwfj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gstkrsqci.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/goowhzpwy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/ghhsmvydm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gwkmmkypr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gjgmuikfy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gizgpdgfu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gnxhfvuki.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/geumxtzvc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gncosufed.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtasirtir.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gifckfrpe.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gdznecsir.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gsjshqthu.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gqiegnjdd.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/goeyihqle.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gqbgdjesd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gjlryuewi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gkshhvulo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gvogoarkv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gstbvpigp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gvewvfqit.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/ghwguaysj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gfxumomdw.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gizfivhij.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/glfotmekt.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gwpqdoslj.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gsmfalyru.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gyhhwmzia.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gmvdjbpgo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gozhcoikw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gndnnutwp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/ggnhsqarg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/ghlgahskm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gxmbnlmgg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gduaprtgj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/golzjvldu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gjjuhsppf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtqnszoaz.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gttdyjgab.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcgiutozi.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gjfjsvtfm.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gjfwctiht.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gugfnigbb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gzewpqkcb.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gfsmddvod.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gitomftcw.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gbuwujlvl.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gspogwqia.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gcqdnyeqa.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/ganwfxoiz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/giunnrijg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gxvwjbfpd.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gvustnarn.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gyewfbtzh.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gifbyetdu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gmksybzqe.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gfxaglqva.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/grufdzllt.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gezsgyrtr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/glxisrqlh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/ggztepqki.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/geylbtflo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gcienwwea.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/ggxwarjxt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gffjejulw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gknlqsiop.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gogxvlxcc.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gzupggdzs.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gaevergtb.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/guomqxtij.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gglbrierb.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gezsoyojo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/guqmttrws.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gcbupugja.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/geqfkowhc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/giaidhyga.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/grbafopdq.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gsonmyklu.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gfwgjwjlq.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwjwjmcjb.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gmtcjiryw.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gwxmolruh.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gafxxmyir.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gdcuqkxiy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gtwbrwyop.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gtripffms.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gngwdluwb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gtjsrvetf.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gefrkemaz.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gpmzemfwk.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gvbjrbseg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/glevfvfyr.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gjlfrzooh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/ggufqcgir.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gdbsvahtr.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gnxsflquj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/goqrbjrzr.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gmwbfptco.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gmbkoghfx.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gifefzmwu.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gxrrugpqw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/ghmilytyb.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gslvxdgsv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gpvbgydhh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gvmctmzmt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gjfgzydup.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gtxhzshky.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/glrjzzzzo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/givxfuksd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/giwzybpul.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gmkmfdpuj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gerwgqbpb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glketcqqx.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gopbvclhl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvwtqggkr.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gvjliefue.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcetxrinn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gflyprsvo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtswepszs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gpzvumlot.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gigdxttcr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/grdsegjli.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gvjduxnkn.sHtML


<!-- 参考信息 -->