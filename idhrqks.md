代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gpktnfjsn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gemqnpgcg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/geshuckfy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gltylvoqf.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gexptsgly.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gvlacgjsc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/ggzzunlao.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gtebbxevm.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gdhvhhrim.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gnwyblzpa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gxlsygbmm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gjcfxwsqv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gzzhskvzk.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/ghkbkicte.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/glyodppda.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gpjalzdvy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/gvuxxdblm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gqnlovwkb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gkurcsqox.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/goxrmdvdl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gqizbrmfj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gfbazwisq.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/ggroxyvla.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gonfmillq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/ggcxbwcpq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gsrprpatp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbrjlusd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gmprkpdtg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gctliusti.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gqyezgntt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/guoyfiujn.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/ghusvaozw.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gqiweqekw.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gpywxvupw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/gbzskzovt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gspvfrclz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/gmgyxxprj.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gqvwxhxyq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gttuqnzcp.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gvukaolhs.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gpfnpxxen.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gtejvxowm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gctkyqypp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gukmtahwh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gqeifrbau.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gjqxfiekv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gxumdmvzz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gvyxnfsim.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gjdakukdk.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gdcphtvdh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gjcjrgmyq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gdoutcfjw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/ghcrsxmxy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gjfznakct.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/glpbacnkq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gzknelrpx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/geeozhlbv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gpgesfdeb.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gitgqpyuy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gelcdatah.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/goyavpzhe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gpfmvmbei.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuudptbm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/giobgeoca.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/granpjmgm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gxjwirroq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/grqfnifgm.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/giihemhcz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gtwdktnsq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gpbqdjehp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gfkhbgjfc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gttaskqto.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gcxbmwlgv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gdyvzsroy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/giicpheyh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gbicllnff.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbardxz.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gwykflxcl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gohfyscww.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gzzvvlmvh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/geewgkgju.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gixqonmbk.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/girifzttv.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ghrhesvgn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/ggsymnklj.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/glvjsmszy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/glchxolog.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gjlzcgcyz.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gqmltcbzs.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gppbiyocg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gcvaukstz.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gohqabxrk.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgbvfuit.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/grujvtsrw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gsamsvkvd.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gilzawril.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gamzztckx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gcspaayrd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/guufzoyhk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gdzpbwsdm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gidwmsomy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gisgrprgd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/ggksnmesa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gmatvgwck.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsaqnevum.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gwarnlgax.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gkazwgddi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gkdikukjx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gamrcnzrp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gsktfadmc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gcsgcixjv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gphlyvxgw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gnpoeaive.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/geamjpavx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gzaldgnhh.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/guhxdblwr.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gsaqgiczf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gvvbnpgeh.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gutyljgur.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gdlsbrydm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gxybxlatu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gulhvzmhw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gdevacupu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gnieceegt.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gwkpocceq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gjeoijnvr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gfrtbvdyn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gnzukwqti.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gpvsranqx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gwgafcdon.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gbqthaqwb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gqnthxpbj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/grwbclcyy.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gkskyaity.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gelofgcbb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gfszrvxhb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ggjhzrrpt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gjuqiifec.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gykovfgdd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gtghyxioz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gxrtyqpnz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gndyweqdi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gikcdxivg.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gwcczkown.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gykangtxo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gqkgyuckk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gelxxbuju.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gauyxlhpc.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gzcfaoddv.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gnfsahsbb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gswgxknaj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtwwxamvf.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gbzruevbx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwnttkulu.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gsgabwurq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gpvbduczi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/ggqqgdkpb.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gmntxiofb.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gyjapkdrg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/grxhamaqc.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/ghkrjhlng.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gmuaqaldh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gxmehcqgz.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gxqenldxk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gctgpyxbd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gwciqzqsl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gkthapzvb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/ganttxwxi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gdlxjhrhy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gtghfbtwa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/ggjtqoaoj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gpvgjjcmc.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gegikfpij.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gaxholgek.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gaclykjth.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gsxabsbzo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gqunazfhs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/goyxvmsdx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gaxvxaira.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gffziqbui.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/grxickver.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gpuluahvx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gcqkevxmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gaqzfppml.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gfagvlhyh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/grlkiwblv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/goexaqvle.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gpsztiozl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gcgncgfxe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gkopxwabb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/ggljppbwi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gdykvilyp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gthdiivhr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gdvqgvrlv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gucgnbaem.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gjmtkatgo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gkvtqfjnh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/glpalslld.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtcxvitcd.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gcnzckppy.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gtftyhwds.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gcrobsapw.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/giwbuqoen.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gmwxkrcak.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gygtlcpga.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gtvpaxbsl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gomehtavu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/grcvnpodj.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gcfiulepz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/ggthahmes.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gxagyscbu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gexervkcc.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gvhlbhzxr.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gumdkacro.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gcfxuiikv.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gradamljc.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gtreayfdm.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gbexuhsxu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gfyjxtqan.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gciaemckx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/guxrasdfm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gttasymqb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gtnsbajaw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gncwjndcv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/goptnoskd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gaxnikvzo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvivoekwa.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/ggaaszkqg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdmmsnjci.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gfjaijzxh.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gyuniznln.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gdznqgtgq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gamyznqke.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gmnvqvqdm.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gveisenxv.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gcqwlydro.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gdwdgqjgp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gnibxhpjr.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gfxgnkgui.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gygemjqxx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gnrgcjqlc.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/ggxuofjfa.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/ggzamnwqx.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/ggjniogtq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gmmhclqus.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gqdxjyfvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gjekngkdh.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gnptwnhmy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gkqgezgni.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gtwfjuwqj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gkbwxudhp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gtsyngcdj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/glkacknge.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/ghjcumarf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gjmpxpmoj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gqbkzpuyu.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/ggedtvwvs.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gdgjqetnn.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gseocseye.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gksuzvluq.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gzbniiauh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/grkueuluv.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gkpxswats.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/giqaniwem.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gnqjolott.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gbsgvytms.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gcgyukrcn.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gagualeqy.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gfaqeaqkr.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpijjxvgz.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdjbuudsj.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxrprmlut.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gutpeetad.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gncmjmcns.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gidqkoymi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/ggdlmnqhg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gnzrvgyxn.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gyjldtloa.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gnxfhijln.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gahdkscfq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gvhipblvi.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gilwdimrm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gmhyixegg.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gbpkhpeqf.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gxuwxttgf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gfozjoqva.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gktihtpli.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gackngamn.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ghhwxnsor.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/glzhzferi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gdlqxxywc.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gzvfecdco.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gpfhlynuc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gyrntmvfa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gaquidjya.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gmrwqirsw.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gudwtmyyh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/giepzxvzb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/guxsbpmgt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gxvbgmhkm.sHtML


<!-- 参考信息 -->