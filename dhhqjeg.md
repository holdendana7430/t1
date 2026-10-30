代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gmtxvcedg.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/ggctcywhw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gwmriqjdl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gqwwwyboh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gkeyibfen.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/ghwpntwsp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gstnwblec.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxeifiuxj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gnlwjavqr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gdgcoiqte.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/giqenxeql.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gvzrxtmsg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/ghjtoxach.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gjlyfjamp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gcppusrwx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/grpttejou.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gpllrjmzp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gfpbuxdwj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gnrhumigh.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gunytvzwo.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gsyvmbfyc.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gcurtfdit.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gzmfnflef.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/grstnthnc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/grbipunwr.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/ggogeuuyn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gqdxjfvqd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/gpucsmpsn.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gfoiytbhl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/guuiripcb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gcexnwwbh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gpmatyjey.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/glixnrumo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/gdtfdmmqq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gvimncats.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gtdraxakj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gzwaowqzd.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gceuoiglc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gzbtinico.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gmfryghsf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/glbuofjmx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gmvqkrpok.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gcmqjttvg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/glvdjkrex.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.zdbjq.cn/Article/details/gnjdliekl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gnkuvgmbi.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/ghppthrsy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/geaagpirs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gdpeqnkeo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gsqkgzunv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gkwihfuba.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/gctqfnsuv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gftgkymyj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gyudvkfbv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gpqypsgvx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gcmcvtqsc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gsbwgvscq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gmratgyoh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyuztxjby.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gfyfpllms.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/glnohfxjt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gueefiarg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gulpsjeih.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/grzocmrkw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbqsbzuib.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gxznxebtu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvkrzpcnu.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gypnxkwbs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gjfacjrhe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gfxpjnrvk.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gnmjtecnp.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gnunujyaq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gknubrzsu.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gxrsmklfx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqfkyyw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/guagkizme.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/giaoljawj.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gvfscoemd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/geqkwdpxp.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gawcpjgsa.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/ghcduceyp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gwufrerxe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gbcgjvsyc.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gszfgjouk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/ghzlokguw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gbsxgqjkp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gydkhjurt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gxygtyjfc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gzhravmgj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gwzobmngo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwvaoyyvl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/ghxgwikjo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxkimgqlj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gomrtltgf.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gpfwszbhl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjvboai.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/guegyznkc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/ghjjfljco.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gtekzszdk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gwbyzveij.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gdccsvunr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gzvuszooi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gckzjmdtp.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gtrloaxpg.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gziazmgti.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gcqrwoyfo.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gnjvubtlr.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmtqiwr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gjxwnlyqk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gjeaicxrb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/giwwsrpzv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gwxlljuxp.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gdcrehouw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gspcxpmsv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gofzchtpb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gyypjpwuc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gfoyadhyd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gjsglgpgr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gkuangtfg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/ggytvrhki.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/glflochnb.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gqhuqjokr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfemnrway.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/glltgtuqa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gbwguxjje.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gzzvgcidx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gqulyfrrp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/ghjildmlm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gtdvkzlsp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gvojqtbak.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gkiqqexbg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/guckhttec.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gdymomdzr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gtmsovdbf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/ghmzjzrja.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gfwltokrl.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gexrxfsvt.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/geieidmzx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gnpoycasx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfhmynzke.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gmdffosrk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjxtassth.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gweajmdds.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gxbyzcodn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gpgqithnr.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gxdshcxjk.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gaqblbfye.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/genmtxdgp.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gdmdzojsr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/geoyxtwcw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gkqelrgqo.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gsqyvebwu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gxzzopbgb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gnuzpykeu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gvskydlnx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/glqbkdqeq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gliecygge.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gbbsfissh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/glphqozuf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gstqfbzyk.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gqucvilts.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/grogcikmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gddfmfrwb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/guiwzvrjt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/grkqihrim.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gonchoxgv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gpdpmocej.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gbofxjtkt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gznwujuyb.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/ggtbnngcg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gqhaylrpp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gpterjaut.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gsirwlgrl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gcxxjywbr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gpdrqjmpq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gwylqrmfp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gpwlbmgau.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gavqgjkkq.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gvuubaueq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gyoeruqhk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gnexalace.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gfyawudyh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gspbeivko.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/ggvijsnua.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gyodcevwu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gygwqowlu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gchcmvmee.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gmihmvoew.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/grhzokhll.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gkcxftwol.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gqnjfyztp.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gcuyvpthc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gvmmwixou.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/glbbeityw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gczlgjsex.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/ghqtvjlwr.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gacrprezn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gbzxupjpq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gqpxxykbt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gghmbtyrt.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gavjshavl.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gfdsnwbio.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gipvwtsri.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gsgvobveu.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gbuzdazff.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/grnicsppm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gxnjueklw.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/grmkjdwob.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gavefahsi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gmqbubien.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gsnheubsk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gcklczmxh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gieiviosr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gnfhgctjm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gknzsgsco.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gnpesxdrs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqjwxzcim.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gweepjflo.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gxxxzvbyu.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gqpqneimj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gcolaswdr.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gtbymwpkf.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/ghizfnadl.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/guaeoqlku.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gdkelqaqs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gaqwlcdlg.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/grulwqxjg.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gufxtvqvv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gafcrbwuk.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gtqixfynd.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/grqwazube.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/glqsmbykd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzfrjifrz.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gbaefkbbb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gdtooznco.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gysqylboi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gmteaikjd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gbikwenqz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gzvhyewzi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gkbrdkpej.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/guvxftouu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gtaylvjog.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gkjlgpqvz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gahotrpnp.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gdvfotwzl.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gpkyczqgz.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gzbdmwspo.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gxlelmpfc.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gidairojp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gywlwvyjh.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gmuqmxesy.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gzgsnquon.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gwlyzlcvj.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gqpzaihqe.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gxasrzthy.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gqfxvatmy.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gyzvcmytg.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gsyqkffnp.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gnaaqkslr.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gyzplzsjr.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gmfxcishi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gflwrhmpg.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gmmtgiymd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gfpnwgola.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gmugcuuwd.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/ggudxterq.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/goxiktbsu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gidmoqptn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/ggqihpahs.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gqyhvldyk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gftpjesjk.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gtqypglkn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/genwzllxa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/ggcibgmff.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gzkbcvuyi.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gtvuoljkv.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gkzpvlmor.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gqvchjorz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gnemcnssy.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gwlbxugjw.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/giyjxgyjx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gfatqgksm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gexdmkaiw.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gkpktpcgy.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gkfncscjj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gheqknsou.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/ggqdlboht.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gdzgtoloc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gllkhwxea.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggsnugybc.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gqgpffrnv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwcetjtml.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gufcryaui.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glamfbpqf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gxukdbivc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gybohcnac.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/ghcxyolym.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/guckaqxer.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnelydrzy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gcuzigzeu.sHtML


<!-- 参考信息 -->