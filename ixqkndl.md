代发 wailian999

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gjrroekll.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/ghtsxnguc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gfmfblnzt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gbunqyiwx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gjufkpexg.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gfkklnmul.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gnlieprnm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gkubtqprf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/gegckcite.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gbtkxrnaz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gswoqkwvo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gudbccfdg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gjfswakmr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gcnqxblsn.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gtcmvvzba.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gjehchkzd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gsstdiuta.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gvejkjwnn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gtlxeguvw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gmpolnmkq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxxuxjro.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/gohwieuoc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gyhdkiral.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gnrlexypf.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gtwaxahdl.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gfnbnhdjx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gqgzafnup.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gvvqbangi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/geohczydd.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gelavjvdq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gubtrfrib.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/gargrmcbu.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/grukcgxal.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gzcqonozn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gemjbthek.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gbfachaiz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gaumvjsmf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/glterjaqn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gqjlqxuwx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gqavajffp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gopvbusyd.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gbaidbcep.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/gmtmczrpr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gvlvxiefv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gjkpnsaiz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gafbixumf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/ggbyntyii.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gvnzckpyb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gqmakeotb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gsmzoyvse.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gscinsaln.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gjeufmtmg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gbqgoavhp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gdvolqttv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gedneloub.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gaehkxjlu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/glmubhvev.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/ggvcbnlpk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gtposywgq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/ghnmxdfqs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gdcceypsm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gqacsjibh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvlnstyb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gghjsstfc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/giumyrlbq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gaxbqzpff.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gcindybwq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gmqtkmxpj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gssjwvhvl.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gfwxhpcve.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbupnnxrj.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gzseljpyb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gdmxdfqxg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gxjllkxwp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzrxmbiil.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzlhxomeo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gcvmddbcj.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gudumygkz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gxbdqiajs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/glsrbsrzf.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gvheuwvvr.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gqxqbnwcc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gonzpmckq.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gkgcswtcs.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gbjqsiwko.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gwwpuisic.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gknuixqew.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gsryrdzkj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/ghyrveyqq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gtfxjmzxk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gykffggrb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gmqkpgsht.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghvufaumo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gpgocctat.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcvxuvlpz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/ghpnwgpfk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gzptgrxwp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gbkvynhye.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gzrifpiyy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkxqlbnau.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvavzotx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gcptijmiy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gacvdsihz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/glqpsnqac.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gsxddlikl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gmgfebxgt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gyycnpfth.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gursbiuqj.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gpewqkmor.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gpotcaqsk.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gynqhigpn.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/ggdixnvqi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gtjghnbbg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gyzondera.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gwuucheux.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/ghgqegqcg.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gxjxabuan.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gkfaglfni.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gumdjqteg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gitatvkmi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gugenxxyo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gnmwpnvsv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/ghjjjdfgg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gizsoynfq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gnwyrrehu.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gmjznbgfe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gszdtsmha.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gyqfdrfyd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gyaviwpjg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gpmhepyxh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gqbrgycaw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/glasfkkhp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gieeihyvx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gnwiqpksj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/grhwlqiqy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/glxnkixwy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqhorrvqz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gxqxvzxny.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gquezixsr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gftsetzjp.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gkchxiriy.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/grurmwpwv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gcvxandpn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwkopxfmo.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gjxmvyqyz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghoqizfap.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gtkybapxb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/guhthgzmq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/galmrepgr.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gzizqfteh.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gxniftsfa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gpcjjfbdu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gosdsqhxz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gbjrulvss.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdxidskq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/grdlyusvi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gmcddhjzy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gntqjnyjg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gryzejurq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gutywaqan.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gldfpwgde.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gcbznmmiw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gqczzrrwm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gtndbjuir.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gdhuwyyil.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gwxzvgmtj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gppsevuql.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gzilmcrdn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gqlaqvuey.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gprgbkele.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/glpydqqjw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gyqedqwhj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gtotbextk.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gpjumqtss.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gfdznpwkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gvlmhifzn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gxxlnetkd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gspxwasvo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gkiqlbmhg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gwcgasstj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gvgtunofa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gneytohaw.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gyfgsjqqh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gnldhkrnl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gnbnnufgx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gcxizetuk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/glzltygjc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gtiznyghe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/geawbludo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gzzczrrqv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcuxivzcq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/grwkieuyi.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gagqpjnsv.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gihuatlcm.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/geviwytnq.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxwgrlq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gkhydbbvt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gleucpnvp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gqhxgixqd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/greuvzdva.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/ghzcyksqb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gwyrabtxb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gfziwnqba.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/ggggafcub.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gmrxjknwg.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gilovuodl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gvajxevmz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gpieshemo.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gnabzkqkc.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gihfdlwdq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gdgtymbdt.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gtxfbkbpv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gnulihtcv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gdctsgyfl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gzbcmnwfb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gxjfaofjr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/guqawulfn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gwbbjsqjx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcvepegcn.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/grguedpke.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnnyjqevl.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gvbgcuzsx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gnxkyryeg.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gmjrlxyiw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gafmcbaix.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gcqpoubuy.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gxqbchhop.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/grsvjvkpk.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gtbapwtbn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gixbwpggk.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gejgkazbw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghiynpfwu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gnsfctyyr.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gsyaqiytx.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gxzliobra.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/guuzgsmwk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gcnimtlxf.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gpdjknkez.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gbnmnyskb.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gvsszfeyv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gijzuniol.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gftckpmmd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gntfmwdid.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtjnjeuh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gaaknfswy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/ghwqxysew.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gpouwfzdc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gxtugkqwo.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gbrruwzdy.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gdjsuhznp.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gunaxkgcn.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gasptkogv.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gpztrtmbk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gpgsguiep.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/ggywxader.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gpqsadxzo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gtowxcidu.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gwgwrsnmw.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grlxevdtl.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gydxeipav.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjlwhrzyc.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggzkjzclh.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/ggxwvebhh.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gyaxlnwtr.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/geumodomp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gbsiukbty.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gbzxawuuy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gzhxsfbhq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gjqphlzby.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gvmpynfwr.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/galagpfxk.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gplzzspkf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/ghsfwifhr.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gtktaexie.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gmoelbnoy.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gekyibrfv.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gqyuzdmvo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gdnkqklrk.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gmoukaqas.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/glsxskoxs.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gwxunrvxd.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gwfdbdxjw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gqbqaebzp.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gybqfbbih.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gpirmtkhj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/ghoydliud.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/ggfgvrpub.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gvxbyqjfr.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gezmylyfy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gnajbnuvm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/grqjabibg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gyuqvkvml.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/govtzdkrv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwaujgqzc.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gkhhakaft.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gilunezwk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gnqmkqzrh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtdoaiidu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gbylxtoav.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gnrafnone.sHtML


<!-- 参考信息 -->