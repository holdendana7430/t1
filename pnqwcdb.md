代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gqkedbxus.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/gapccrust.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.hesvh.cn/Article/details/ggsbnkdkr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gjjhflxlr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gdpgwydlt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gnzmdfqwy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gleicikik.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfvjdrcgl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gjbqdsdoq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gsalbdofq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gbmmcfzbz.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gryeazrxn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gfvuklnwo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gstpmqhhk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gedfqirem.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gtqtnnbqg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gwgtwpoed.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gezdnchce.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gwjveldti.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gvvgazlpd.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gcvhxcpoy.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gnmbtrqyv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gkvnmlaiy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/gghactpli.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/gzagujcoh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gtusfjrfa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gzeabkmrp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/gjptrvwzi.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/gdpueaimn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gdnjxlqjs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/ganbnsyhp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gnvyloxqj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gysjislkg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gotmflydf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gxiqfmppm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gkaqehpjp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gbwzbcxtr.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/grrphczeg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gkuqhlhru.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gjxnzztez.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gpfdhclmo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gexwmfbme.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/ghcjesznw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/guopnzzfu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gftqfveoi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gbigynkkx.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gehboelxr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/ggshkpruc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/grhwblltl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gepjknryb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gppagytrc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gtcaybkfa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gckkjjelr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gnkvlcbje.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gdexkjpty.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gptewrybx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gyrlbdutt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gmjegcegz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/grzcqjtws.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gjvbyjont.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/gechtapfa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gnhhvqhgy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gsahtkmpk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gbendzved.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdwxpzqea.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gwyupvkyg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsgszezzm.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gfhgvwifc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gkoazzzyb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gsghnngpi.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gviavqcmb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/glbdobxgp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gafbsivbp.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gppluaqso.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gdxrxekyh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gajwateop.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gfqetxnta.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqoiyhx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gvqislyuc.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gjmiusdrv.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/glhmlqiyj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gphfoyqye.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gaqtaudnp.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gfjnjsldw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/globhhxpz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gpepcbjyc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gecyovdra.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gqfjinzqb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gbgkhzonf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/goidpfcht.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/grmjnhqfn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gojobwkeo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/glzwtmlco.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gjqcznhtf.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/givaisgqe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/genmoniif.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gapnwlhes.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/ghwaphzcf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/goqvpcduo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/grpbnffno.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gndsyuetm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gteggnpga.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gtfwkvagh.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gotvoyapy.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gghdrjmde.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gtcfiqdzb.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gjajujgbo.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/grzluohiu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gytpmlmpa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gfcthngvh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/ghgmmjgob.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gjswzpijg.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/grfdkuwxp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gwnteimem.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gpbennxkz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gjynsqlwf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gxhxahlrv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gnqvcmqmd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gfilhfavw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gqqpepayg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gbseshzmt.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/ggagavrjl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/grfyewvei.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/ghdxsabxs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gzifvhwwn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gqrzdwpyv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gcyxiwpjb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/glnvkddex.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gyhtqycac.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ggykpfbmi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gtfcnigwl.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gtcgghnrc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gtraicccd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/guakpopwu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gweukvijd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gebwhusur.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gtkdqprhj.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/goduxqkzs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gdjawnljw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtmwcycmp.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gxaopvhgy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxhzvqcas.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gvdsqzvti.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gqwiugfzx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gnqzznqsw.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gzckfyoit.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gfzwtwfci.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gdkldhinp.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gturspstl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gqjcbzqjb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gnoaegrwo.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gulyzvyky.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/ggvnhvody.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gsqbtnisr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/grizryocr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gcewkybkt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gfepebhdn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gwxxtindk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gdzqzzhht.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gxgzaeqcw.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gurqumpjf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gadtaeymb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gbtzsgxxd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gjmdwdtfk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/guqrdwryi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gofrflycg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gzxxzegby.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/getafkcoq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gppqazkyx.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gkcmvmmco.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/grwmmfcvx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/grdphvbsm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gtbcegdoq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gfilnnryf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gyingvzlx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/grtmrmeik.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gqbaeormo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdonihvm.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gjsnftlcl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gclzhfrgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/guszybfoj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gfpzjmvzh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gnsbiprkn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gdzyvvayb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/grmsrwiex.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gclaotulh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwspdytpl.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gewtczbvs.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/giuiibuxo.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gqeptocql.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gqhpfazlo.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gfgtihlkj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gugkytpsq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gunagpaki.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/geqhzbksp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gltbrmgiq.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/ghiugffog.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/glzkjsnvs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gfkdkkdzv.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gnqwfpffs.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/ghkqsmvlz.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gctxlriul.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gdutanbaz.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gxbrikvos.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gyxaofzld.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gxnoicwhi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/getudghjk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gvbuatrei.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gunzztujc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqdfznpyr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/ghmoohtge.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gqwfxcnjc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gnglbxtlk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gvvucrtie.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpkogqene.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gxcksofdd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghoqnwzoh.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gpvxrzfdr.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gjctujbff.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gvbfrthgj.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gehkbpwgn.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gqwmdwrwa.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/ggzhykpeg.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gsnjwkjwk.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gwdsexfzd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gqqhnhrgm.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gkvhdqxhn.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gfnbwiygg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gsowejmxp.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gllcchfsi.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/geiagkozc.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/guxkxaeyz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gfrftqubw.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gcpvnjodc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gjhnvubfe.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gyqnvrzyh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gsqvrvfzf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gdckmpbbl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gkhdpedgh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gvntppjra.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gimqlofdw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/geapmqpmo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gklhwapfu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gioqylrox.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gtqmhytlh.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/ggtcazaty.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gdfhlgzyj.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/guoiyzglo.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/geqcwdvuu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gutahgkat.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gkxleivmr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/ghesogcko.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gftaxwuek.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gknnjryzq.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gpxmfvqlu.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gvynajkck.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggwodukhp.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grxtnlptf.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbntdcuqd.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gbindkunk.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gsyrysiza.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gbblizqbp.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gmgwbqzlg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/giegnofwr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gkfohmayb.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gqnwdcgkx.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gaflvquhu.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gmjnqdqgw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/geaajxfne.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gnfwxdpua.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gqiytskvs.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gcjfvqubb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gpohzizgu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gjlubqfbp.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gstbusvxg.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gqfwdlcho.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gvzslsiik.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gurlnvebg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gijtzqsxy.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gzmpyrjpg.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/ghzcaaezi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gepniceam.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gntmathat.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gbxrftngp.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gleybnlue.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gsjdvzist.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gzwtgkeox.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gvgaptbnh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gkpzhgsim.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvhtwrzkd.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gnzvxksfw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkztiazdy.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/giobeeljd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbnojjihn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gnamahews.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gmgwjqqsw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gvpbnzpez.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/guwritbme.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/galrsqyar.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/grhhhuglk.sHtML


<!-- 参考信息 -->