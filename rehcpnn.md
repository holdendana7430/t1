代发 wailian999

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/ghrzkdvin.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gfvmsseik.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gywlzpzsf.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gxlscjnoq.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/goxcewtih.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/ggokqykow.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gxmemltey.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/glhkueffc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gzsrbdlly.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/granrktdf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gthuuwppv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.hesvh.cn/Article/details/galhekfdc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gsfgrtfjc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gaukzqelb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/grsqvoyoy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gnzgzeeuy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gklukglcm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gtdxjyjko.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gevnssbzk.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gofyqviog.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gzkctvktt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gbprcijyh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gzolcbmzj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gsajxalig.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gnxhvetfd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gquxxpqti.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/ggsknnden.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gwcyfnybd.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gqudsudqh.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gwirawwbb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gekwxlzbd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gezhaldfi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/gbblfsxfx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gcvxzyywo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gyebqfffp.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gbijydgzd.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/gbbroxvcn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gppsquclj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gbrkrlwck.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gfntklttq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gtduyztux.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gpgdoefcp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/gmobbqwvd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/glzvlgaap.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/ghmufkome.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gyhorvvxj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gvqwvjncn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/ggvpysuna.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gatwxzwnl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gtasqfvbj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/grwwvyyrz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gpircwccb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/grxjiyovs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gflfnvdkf.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/guntqqjlb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/giyxwlkqh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gukjzwylo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gdpyhrtlo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gfmuomyqe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gnrxwpuvh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/gadabcaxl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/guctwttld.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gbwslloiw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/galkumjui.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gsjjxfdyx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/gacwizfuv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gphefkpgx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvgkltnen.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/glwisckcc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/ghbxaranj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/ggeesaicz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/guxnnkbrc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghpuifbre.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/glqxqagjm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkhuuioyr.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gzqvzmxje.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gvqqghjhj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/geilphevc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gmppmyvyj.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gfyalgtox.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/ggivbhglk.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmhmlxtti.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gchvwscmn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gerzgiwpf.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gyuppgytg.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyngijkoh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gqpfxphhd.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gbubtahqg.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/galuubrsd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gfqlqcurg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gjogazhbh.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gthynxchk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gnervdtyr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gsczkhfyx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/grrbpwlpi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gzyymgcdx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gywkcjxbo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gftwqxjbs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gezkwbils.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gzutzsdxd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gucdmlqif.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gsncepunn.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/ggeanrazv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gpsbidias.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gpvwmqtwy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gmpcuiebm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/ggubakicv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gwagimihw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gunzntadv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gmgxsjgds.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gxjgfucne.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gjjdlctxr.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gzyqgzesb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/guscvrnjv.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/guebkkupd.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghauhjtjb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gobjvdlfb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gwbpehhvy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/glggluclz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gzxnmlzpg.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/ghxwekmdc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gxaqsczsz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gwakoqabk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gunbtvigy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gyfryjkuk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gaxgnshfy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gvysdjdhq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gssosqfbz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gwfqhkitd.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gwiznrrll.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gzbpnkejh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gnvrzpgxo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gbmzojcvj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gpmifyyon.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gtrclzvzv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gxatrhplc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gdddybeha.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gfrzcbvpc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gfgdhvseg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gbieqsgrw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gtaxblftb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gsoxxkuzw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gqxymoqjq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gxqutatrd.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/grjyihtnt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gyejtjmdl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gbmugaenl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxmqzmgdg.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/glpzqzriw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmquepdmm.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/grdmzuyaz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gkucdewko.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gqnfqaagd.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gqvdyrjmk.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gxsvqfyyk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gltwyekvb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/glpcqhcnh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gfmgiuwxj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/guezxwbny.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gzzcsrobi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/ghxzlsujf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gefdggwhh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gynifhabq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gsjreevdy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/goaiksylp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gpgxxdloz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gvkcvefsu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gsavntmkp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gvrzufqtc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gretpbjhc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gvizbmoxd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/guxpotoxk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/grwzhqggn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gpmboztot.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gkvzdxmbc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gjwvfzxvf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gmccrpahf.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gnadrdvkq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gvqzbjzns.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/guquyhwxe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/glwaluylt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gfwczibua.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gpphlngbp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/ggzgyfqbt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gvagdgubq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gqcspmjrm.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/graepiokv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gekdtuity.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gyzscixsz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gazdrymvt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gqusmpxqg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gdyxfjkwh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gzqjnvkhk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gchwuhcnj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gzqecfcmu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gzsrbjdkx.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gxlsfxznd.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/glhvecmgy.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gthukftpr.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gnizkgjav.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/ghiqmwpnu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gtwktuwel.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gvebwpaxs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gecwuuwqm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/ghbxxkmti.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gvmqovrcj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gxvpqlgzo.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/grtotwwsx.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gbtfhfawf.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gmfgpdmum.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gtqtbmsue.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gnfdwblvc.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gvsxqnvnp.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/ghlmqolwc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gkibfmspv.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/glbaxhhls.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gpgijdwcp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gtxlnvjgz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gxgetigxj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gccpkhbxt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/ggqxcpghk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gwnobynpg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzadffdwn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gpopoumvl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyhczxcvs.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gereyxzgb.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/ggabeiahf.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gcdxnmeas.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/growpiyfv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/giubvjxbm.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gqmnmoqej.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gbcexnooe.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gyxhbjspz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gvokpskfr.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gvopsifbc.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/ggyilgcpa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gmqybpycm.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/guaanticf.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gmceciaqu.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gnflztdzx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gqxquwhqn.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/guepvxmkp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gekmimcvt.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gepnirbny.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gwllgmick.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gmapkskux.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gvltbqefc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gjwxcbeev.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gcinaxbfz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/guzickggr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gevnabjkg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gyeufnidf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gtykuwkuq.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/guadpynyh.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gbloedpfq.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gsnenfuoe.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gchqvbzds.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gzjobzatj.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gikiekdmu.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/ggwviicfc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gkrflisxq.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gbbnkdecp.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/girnrdjen.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gwchumzsc.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/giggquwvk.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjbggylsg.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gyeulefzc.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghinocupm.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gaovupayi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gkjcthtoz.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gfnzbwywe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gzwheapzn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gtumhoveh.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gwvnqlaiw.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gnnmqpyhy.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gxnwzquhp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gfiwbvubq.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gipekkbbs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gmvfbdprz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gvodxjlha.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gkpekyeid.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gctfylxir.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gxgycyqst.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gyezmlfow.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gikxsqhuz.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gbhfmndsw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gsnrhdill.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/grayarsuu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/geqoconhk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gyjlwqrvd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/glaebegay.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gtumqzfii.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gkyjhlgam.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gafdyhvei.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gubgpnsrt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gnlgjzkcy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gamsfytuq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsrnewcdz.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gviprmpdt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giozswwtk.sHtML


<!-- 参考信息 -->