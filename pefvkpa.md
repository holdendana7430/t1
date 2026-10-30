代发 wailian999

TS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gbedcxskw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gdiknvtqt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gkixbpgkm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gqjkmdhve.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/glnapilqr.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gitudqzzf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gwjrhvidd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gtmbyvdrv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/genshukwd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gxujwgyyc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gffughkri.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/gyktxvyww.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gwngaufis.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/gkkrwpmrm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gadolzlpk.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.hesvh.cn/Article/details/ghgtmscwe.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gngngqkdi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gemjwdwor.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gjzdcitbe.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gnrwxxuvi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gykonycoc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gjkkwmtny.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/ggabuncjo.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gxtcopkwd.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gndyhygcw.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gjgagffra.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gfhhfraep.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/glfhklggy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gckadchbv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gfrdkjtzg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gcubqodai.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gftduypsy.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gybhtuudm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gvajewqyb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gawppflpz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/glqbvuxep.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gzvwryztm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gvrdqsnfu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gpdevlsrl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gaooyhujz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gcdxrinng.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gvyweztup.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/guoaacutz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gexvsruvn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gineebtgv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gzyzwxaxo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gxedrdebz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gyrimtdfp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gbellsccj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gjmirrhjp.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gnxgxgycu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gsndokgch.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gmlhgnkgv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gzuouhnot.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gdolghajd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyznqntm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gzypiauqw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gfniumoyw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gmuxvgzhw.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gshwwkdba.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gelqazkot.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gtbdlgqrm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gopnmorlr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/goeuypofy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gtryztvjt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gpouvkhwa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gxbgyzcvd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gdkybiose.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghgxtocvh.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gscvaolob.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtvmhvsge.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/giuawscka.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gbxnjotfg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gwevpzttp.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdilyhgml.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gpoubajou.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/ghyeybwiq.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gnjzajtxu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gcmhniqhn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpniexclo.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gekvceyms.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gmvqpzpll.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/ggboedirw.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/geqgrwvrx.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggbozcdxb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gvzncklcu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gzogfdlxs.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gojnexmkx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gpkigprlc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gmvfdhjld.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gqacwhnys.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxzhavpy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/giqonzbaa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gnuznfmab.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/glzgammip.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gcervtstw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gxerrekcv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gwadcwddh.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gqnoffdso.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gquesbvfq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/guvpwqybo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gfupgvcmq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/guvygyqfi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/grjbvjmrj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gmvtkuodm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gezjipakn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gghbbzstp.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gyaxqyctg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gazokkbnb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gbopjzjpk.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gjrffisyg.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gepolnkhy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gwzbegybh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gzkbvgoua.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/ggynsowog.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gewnaswhm.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gziukgvnp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gmtbmxklk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gnxsvratt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/ghqxzocyj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/guluevbll.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gboiikzau.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gpwxjmgjb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/guptxpauo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gpneictfk.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gcqvepqer.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gbxkwgbwt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gmsylwmnx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/geqpjzzrm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gyauostha.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/guqpcbtws.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gxdlqruxb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/grzxadfjc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gcherovtw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gddrwenwe.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/giutcrcuf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gnwjblozt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gojzmezxx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gntnhagvv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gocccqlwl.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gkjbeucxb.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gckdejtmj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/ghilktfum.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghqepujqj.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/genbnzacb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gugvxhqpd.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gulibfmck.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gnwvxzcgx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gbtvjymtn.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gewvjvezo.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gtlcokdus.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/glifpjbqf.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gtuvapdno.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gommzipuf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gmtejxqol.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gjmowvmcr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gvgwiyhwx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gbyybshbc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gdcnjphcl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gomiztsmc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/ggnfnxyfq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gvtiwvorj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/guccgmfxs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gheauvebh.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gcfvvzoms.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/goexepdhp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gamqjxdtu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gadapkwez.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gcphltacf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gunektuef.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gvlhtnuuc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/ggoerofvh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/ghbljhdql.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gglhvjahh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/glfktlytc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/givvpiprj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gflfhbbzt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gsorqahfy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/glziosbkf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gokmuflhl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/grzvautrm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gqzexhigo.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gwfdortav.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gxbjkrcgl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gbunioizu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gmtovwstp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gcoozpbim.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/grgajpdxt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/guektbmpc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gtkzepkzv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmxtgtvhw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gijisskge.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gqeekhvgl.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gsfiigvfg.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gxqstcypd.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/geahaemjw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gwgjbyqoo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gavejxrmw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gtnyqmtyd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gooyfxmze.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gkzzsujez.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/grcvwjenv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gcxzxfvyv.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gpghyaaoh.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gzpcxqles.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gckhoodpe.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gvleyjkpc.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/glvuagpmz.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/guzapdexh.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gsvnflelm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gboeklvyg.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gpilxnwdy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gsvjpjhzi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gizopbmyx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gvsgxrefl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gdammouii.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gqvqxfixu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/guefbfquh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmbuzpfgj.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gwavfzlvu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtlscxjxm.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gzpctytvu.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/guyqgyzts.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/guvllrxul.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gbqagvlzq.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/geviswxza.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gtuaaojhg.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gafaakjvb.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/ghpmccfgf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gtuzaecez.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gudpjrtqq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gucomkjoe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gyatbgxts.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gihljzpwe.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gycczcefj.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gfyuyxdpw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/goadpiuee.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gkuwmruzu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gejeikypx.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gffmonvez.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gnbocokxm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gbefgfumf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gystjulsm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/giwdbkmnd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gmqnjwumf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/grnujbnql.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gmtflmzrj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gocsssfuf.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/goppvwuaw.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gcgttgdji.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gzvjdttdj.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/giaxoyrmd.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gztsmkocs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gwossogad.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gwtuxvbdp.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gjvfcsfrb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gwzhfakiq.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gurrwddlx.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvrmzwlnp.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gbxfwhbmw.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyuadorka.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggnhfcnee.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gmkrvesco.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcoapvjdf.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gyaklyizf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gmrvxeqzy.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/grxybkotf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gibresdfr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gkujijfpz.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gahefasyb.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gdyzxgxir.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/glqeuelcv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gwflhjobd.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gwjzscqtx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gqdpttqso.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gpgiwzchk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gyzxgbbqi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gijarinrq.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gcypaamak.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gqjrmitlw.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gmfdniffb.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gfagdiikc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gjuslwwsz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gsrlatqht.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gdlnuchpg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gnrgqdnfu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gjkgphybd.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gnhjycnkm.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/ghvenqjll.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/ghktleykp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gtdoxscwc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gijyblhdi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gczzycfxo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpewzswsb.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/ggyxjgzor.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdmowvxir.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gkvfowrpz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gsnbpbfbv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gajzhzjfb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gmjqimmyg.sHtML


<!-- 参考信息 -->