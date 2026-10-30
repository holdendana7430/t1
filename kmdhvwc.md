代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfcgomio.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpdvzywx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/geaqbucqo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fanxiaobao.xyz/Article/details/glywaemwp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gjivjniwl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/gaimqzqcm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjerwfkai.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpjfyllf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/glbwusayo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gffkmnira.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fanxiaobao.xyz/Article/details/gblalmsxs.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/ghdursohi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/gzrkdgzdo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/gewmugnwd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgqbmluk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaehrgqw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gjttxtkmu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggalfoaan.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/goeahuvqj.sHtML

[J06] 计算两时间之差
来源：http://mobile.fanxiaobao.xyz/Article/details/gluxegaev.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gwognldwm.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvbowlwm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fanxiaobao.xyz/Article/details/glripptsi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gnpjefiyu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbqbkisz.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fanxiaobao.xyz/Article/details/gknziotiq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpikgsbdj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnqqkqah.sHtML

[J07] 比较两个日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbibcmij.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gfrbyqcrp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fanxiaobao.xyz/Article/details/gcvhwhfjw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnvlavnq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdutfbta.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxzarrkp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/goinotviy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcnvmixk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/grehlyeux.sHtML

[J08] 提取年月日与星期
来源：http://blog.fanxiaobao.xyz/Article/details/gulixivec.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaudtkqj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fanxiaobao.xyz/Article/details/gdjgnpoaj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fanxiaobao.xyz/Article/details/gphjbpvrl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fanxiaobao.xyz/Article/details/gkcoerdfb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgfabvct.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fanxiaobao.xyz/Article/details/gudevoymk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fanxiaobao.xyz/Article/details/gmgacxmxc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuwpzzis.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/gfyafreln.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnuexwzz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/getnixkrh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/gijvojgsq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gganlssex.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhciyvdl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkyuppmh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fanxiaobao.xyz/Article/details/gryigdiwv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncvzbniq.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fanxiaobao.xyz/Article/details/gfmwsorzy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwatpvvp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fanxiaobao.xyz/Article/details/gqfixlluw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpekagyye.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gvmqcbmun.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gscfwkhnq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fanxiaobao.xyz/Article/details/gweroziqh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndtfjnda.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gccreqgni.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gudpxedfv.sHtML

K. JSON 与序列化
来源：http://www.share.fanxiaobao.xyz/Article/details/gjllyzevj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmexgbnxj.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gudkhpjgv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gwclhzklc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkyztbsh.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/grdvcbwxw.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwiowqmk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/gerrsnlqn.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgpjaegq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fanxiaobao.xyz/Article/details/gsdmiqlnw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwdqlkim.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fanxiaobao.xyz/Article/details/gwtreioco.sHtML

Py:   json.loads(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcqgqqhp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gkddruywl.sHtML

JS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/grzdevspe.sHtML

TS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gyamqwrmf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gjqfidsfj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gymrvoapa.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gchowiwwd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmvktjlw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geskwhsmw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqgmawdn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/ghasymbnr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gifkwjlfd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/geguobnph.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlulfiaz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gykfburkt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvjivehz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvmilqtc.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guojbhjpo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gdsesqyts.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gunwysbqz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/ghcktskkt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdtpcopn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gjhjvxloz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gprepbflf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gpmyltslu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixoryqs.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqwsxzyq.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeqvzmje.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fanxiaobao.xyz/Article/details/gduskdpzy.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccjxokfm.sHtML

TS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/grbjfuulp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fanxiaobao.xyz/Article/details/ghyxmekqe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fanxiaobao.xyz/Article/details/gxvigbziv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gheykegwm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fanxiaobao.xyz/Article/details/gqgicznmj.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fanxiaobao.xyz/Article/details/gzqabjeju.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxnfuywv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gefvnancb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gyzkqdorx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gerzsukxs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsxeyaal.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gldtxawgb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpppayim.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gvninbjwx.sHtML

[K07] 进制转换
来源：http://blog.fanxiaobao.xyz/Article/details/guivnipzm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/grmuasvvc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fanxiaobao.xyz/Article/details/glurukopv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxckzjjav.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gikqpkzmf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwuiihay.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgldxzim.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlwaqrbw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzcmstui.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fanxiaobao.xyz/Article/details/guftyctnd.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gogorbcek.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gkjcimpua.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuwgrdzl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxmlesvx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurlcnroe.sHtML

Go:   encoding/gob
来源：http://m.share.fanxiaobao.xyz/Article/details/gcenvisot.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gegrzqwdc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuhbqtoq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbecaougu.sHtML

L. 网络请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvsyqdfi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfmvbexvn.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/glzxlkkzo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtabiqdq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fanxiaobao.xyz/Article/details/gsvgoqhqr.sHtML

JS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/giignxtfg.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geukakzdv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fanxiaobao.xyz/Article/details/gxfprdqyc.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gcbmkyabu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/gygvdgnkm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgklsgjg.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gurltzceg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/gvskgexop.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fanxiaobao.xyz/Article/details/gpkpzhjwp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gjiazhvqb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fanxiaobao.xyz/Article/details/givpglplh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/gigqlnwbl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpczdjvb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fanxiaobao.xyz/Article/details/ghashevob.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fanxiaobao.xyz/Article/details/glitnfawe.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvolincl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fanxiaobao.xyz/Article/details/gerrbaqps.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gezbcsalf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrvqxrhy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gxzzmufbs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsolmboa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwxtnqok.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbejzepd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdasogmew.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/ghdzbpsxh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbifloiux.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprvozmkm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/grqtbhdrz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/gjqcjjgby.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gxatznnlz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcecoyeb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fanxiaobao.xyz/Article/details/gjfsjnpmd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/giictlqpb.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fanxiaobao.xyz/Article/details/gymizfmnb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxpxwdbt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fanxiaobao.xyz/Article/details/gkfqupnsf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwhjclke.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gwolcdqoo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fanxiaobao.xyz/Article/details/gedhcqeit.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzyrests.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnmrbfoa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlxdexup.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntowgbyt.sHtML

Py:   resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gssnhntzo.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gujpxnhnp.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyqfvmyl.sHtML

TS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/gartevntt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/garkqhrnd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gdihyhijx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrzbxoue.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtutnjjl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfdmunag.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwzbbcgn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqglsnlo.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gnrltnjnb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcpkmmws.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgfjwemq.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/guleshenu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzpqwamr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gbuzwvmvn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fanxiaobao.xyz/Article/details/gwevigxgk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoaeswfj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqbuytyq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gvzbuzncl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrfqhpag.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fanxiaobao.xyz/Article/details/gywfwwrhp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gadilbouk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/gziblzpal.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/glahpenub.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxocarpmt.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fanxiaobao.xyz/Article/details/gbuotirsb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajdanerq.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gggbuyykx.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gaygwcxis.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gemkwmupc.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaklphhk.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmexprky.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjjgwwnx.sHtML

Go:   os.Args[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzecfaeh.sHtML

Ruby: ARGV
来源：http://www.share.fanxiaobao.xyz/Article/details/gccaolgkx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gbvsmcoyk.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/guegsimay.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtdtmddm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/gniglnqcd.sHtML

JS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzdtadof.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlybcbzl.sHtML

Java: System.getenv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/guojwjyyl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gywguskyq.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginbjpwmi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzejyombe.sHtML

[M03] 执行外部命令
来源：http://wap.fanxiaobao.xyz/Article/details/gktmbwyri.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkwhsoxe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkheskjbv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gieinkxce.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwasyjru.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gpmchruac.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufvitibz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fanxiaobao.xyz/Article/details/gowulyfux.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyfkyovq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvbzllsh.sHtML

Py:   os.getcwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhhqxfes.sHtML

PHP:  getcwd();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgrxzxkv.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhcnqofq.sHtML

TS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcrnghpq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtowcima.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfcepeyx.sHtML

Ruby: Dir.pwd
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmkiaept.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fanxiaobao.xyz/Article/details/gytmgejod.sHtML

[M05] 设置退出码
来源：http://www.share.fanxiaobao.xyz/Article/details/gouykixss.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsmhtdra.sHtML

PHP:  exit(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagwctujs.sHtML

JS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjtndqom.sHtML

TS:   process.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyvgfxki.sHtML

Java: System.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gersrbwdc.sHtML

Go:   os.Exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzpjmrjaq.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/glzvzeeky.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fanxiaobao.xyz/Article/details/gcpkroxol.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsntzlkm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/ghckgjtyj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbsigblr.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gtetnxvji.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxphscucj.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggatqotuc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gcclwdxfd.sHtML

Ruby: warn "err"
来源：http://blog.fanxiaobao.xyz/Article/details/gprlljonu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktovizdl.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fanxiaobao.xyz/Article/details/gedwzzbvb.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fanxiaobao.xyz/Article/details/gwpsdzege.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyvwmnfw.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gkwxaqtap.sHtML

TS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrfwbuvo.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gubzeofdy.sHtML

Go:   func main()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjyymggq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskhcpazn.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjcnuaqj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxnwuoky.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fanxiaobao.xyz/Article/details/gbgdjujon.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fanxiaobao.xyz/Article/details/gfnermuct.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqhutjhu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/glnnkbinn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/gpwlcdyhj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fanxiaobao.xyz/Article/details/gjxzltezl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwqnupts.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbypvtzu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghfhkzsvx.sHtML

N. 数据结构与算法
来源：http://3g.fanxiaobao.xyz/Article/details/grpywixvq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gteksrhed.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusaeerlb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohcjcgsq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupseimwe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqlvglag.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gupabqozu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gtbliuqpf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtfqilxc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fanxiaobao.xyz/Article/details/grjhqnlri.sHtML


<!-- 参考信息 -->