代发 wailian999

[J03] 字符串解析为日期
来源：http://baike.fanxiaobao.xyz/Article/details/gzmypdrqp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gepqfiskn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fanxiaobao.xyz/Article/details/gqpquspuk.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/geizycrkt.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfeqxkbs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupqkbtlj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/glgznxcrp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/glgtguknr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoqpsjah.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllnqrvwg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnqzbrpl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyegkfea.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvcxjrdw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeripiqs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamkojyhe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/githwogfj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgoedrxz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrzxjipx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlaqymzz.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/gpswbyaub.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gkezzckxg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdgxedwn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gmnnicysi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gjrdpbxsa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fanxiaobao.xyz/Article/details/ghteyzged.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfszdqlfc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gggfnqnon.sHtML

[J06] 计算两时间之差
来源：http://read.share.fanxiaobao.xyz/Article/details/geunylxfq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpivqewky.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/gygzbvnzi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fanxiaobao.xyz/Article/details/gdfijudzk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjyixycq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gldkmgnfm.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/ggvyqsgae.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaqikccb.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fanxiaobao.xyz/Article/details/gfrcgqkkw.sHtML

[J07] 比较两个日期
来源：http://wap.fanxiaobao.xyz/Article/details/ggkgnulaz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzylucpv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqibqxxwr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrwuvkcv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fanxiaobao.xyz/Article/details/gvzymkole.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwzltagrn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabtvusza.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbyttleg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhdsskqy.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvxzlmuk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrfggyfl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fanxiaobao.xyz/Article/details/grcafrxxr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fanxiaobao.xyz/Article/details/gkkemthgy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fanxiaobao.xyz/Article/details/ghktkqnse.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gtrdcczld.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fanxiaobao.xyz/Article/details/glyfhytnv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fanxiaobao.xyz/Article/details/gyhqwxymk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/garyyyuqc.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgjfdzic.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fanxiaobao.xyz/Article/details/gqprcyiqr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdaaucql.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gueudeinu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/gykdnqphk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfnmhshb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fanxiaobao.xyz/Article/details/gfeuqohjs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfagerhom.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fanxiaobao.xyz/Article/details/gztevkszt.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/gbjoeyosd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glufpnike.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzofwjgub.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyasaglz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gsknkttfy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grginekre.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fanxiaobao.xyz/Article/details/gythjsvkq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/gudzehcns.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumopxyll.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhxmssdd.sHtML

K. JSON 与序列化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxmmjhnt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gquzyuqgh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/geqelbtnj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjckpazhf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvrhxhpb.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvihvdgy.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghadngtez.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcsdkvqb.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhdomxcv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fanxiaobao.xyz/Article/details/gnypqdvcv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gdhwumgay.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbuhewzf.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gutmjpgvs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkekgkfem.sHtML

JS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqchwdcpn.sHtML

TS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gjzwgafxt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gawmetwdh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrvifhst.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouugzvyo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmludphrh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpfgefrx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgvqwwmo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/grrmtxnke.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvicguzsb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmhrdlrn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gduqiyrxl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fanxiaobao.xyz/Article/details/gnsclkagx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqvccsvl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fanxiaobao.xyz/Article/details/glreysmbz.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjwyffktn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gnwffuuiz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxtqejkn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gmrdtciff.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllkupskp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geatwaifz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoofqviq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gaisqnnud.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gvviszsjq.sHtML

[K05] 深拷贝对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmkoyyra.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gbpjvwzhi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/gvnyxyplu.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoomojhd.sHtML

TS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gzgeqvqvr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fanxiaobao.xyz/Article/details/gllrkwxmu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/gzqgmfgrw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/grstqmlwh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxaveglr.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fanxiaobao.xyz/Article/details/gnabldeco.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoxbnwxf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqirqtmfu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/ghcztircq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyrrkdnh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gxfkneadi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoansjsd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmsatgun.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/ggmwacqfx.sHtML

[K07] 进制转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihrejzxs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/grmmzqxrb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaztkfvg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/ggnpqhnyl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxuruneq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblfjtpxy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fanxiaobao.xyz/Article/details/gkumixgpz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusrfcpyy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntzwcutk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fanxiaobao.xyz/Article/details/gqkxqvrpj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/griqczsja.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqagfmmeb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gpceunmkp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgibykdg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/goajvfojr.sHtML

Go:   encoding/gob
来源：http://m.share.fanxiaobao.xyz/Article/details/gntwantzr.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gxahjrysu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzkdzdgf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnykaihc.sHtML

L. 网络请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskfzchok.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxujpxcd.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuuamknl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gmsdmhhrf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/gjzrvvwka.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbigftwf.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtllavew.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtmrcurn.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwuuzper.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcbltfsl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghopqlsgm.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gckrzbzdy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzpwwnhd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fanxiaobao.xyz/Article/details/giugwpbrx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffsudoyr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gutxlhcfb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/geuwgkevg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyiejxcb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzlozgts.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gtdpscrvg.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsbswugf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fanxiaobao.xyz/Article/details/gaaazlsyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvrklpuf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gliwrvqrn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gvudnrlhr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbhukhum.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswoqcyya.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqgpmikk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmwwdmwu.sHtML

[L04] 设置超时
来源：http://baike.fanxiaobao.xyz/Article/details/gvvdfifbl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fanxiaobao.xyz/Article/details/gqefqxkmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwbthptt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gxcktfens.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuoxmgsl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gomznuiaj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fanxiaobao.xyz/Article/details/giuqwqqbf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwooulrap.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsjwyvmp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhtooelz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvincqgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbffhzaya.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gjfrglsta.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqesbjkx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxihqpdp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbhhdqov.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fanxiaobao.xyz/Article/details/gjustmstd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzqtqmpn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gixuubxfo.sHtML

Py:   resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzpvqass.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/grflyemht.sHtML

JS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gnrsagyfa.sHtML

TS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gonsnfpde.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gtqhvsiul.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gfdglqmfh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fanxiaobao.xyz/Article/details/glrpoigob.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkrmmmgj.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gbvcvyfnh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fanxiaobao.xyz/Article/details/gbqacbuch.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrygwsqt.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwtmeamu.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjsaczzg.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvbuicyd.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknihlwyn.sHtML

Ruby: resp.code.to_i
来源：http://blog.fanxiaobao.xyz/Article/details/gxhunfmdw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlbwxhcb.sHtML

[L08] 并发请求多个地址
来源：http://baike.fanxiaobao.xyz/Article/details/gtwxntsqx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fanxiaobao.xyz/Article/details/gqqurihug.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/gokpvtwzo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gdtlefpzc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnnwmqvu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkbqstcn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gcmjomieq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gigwwqxdt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/giewwpynt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkletyfnd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojxvdrsp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrdvqjqt.sHtML

[M01] 读取命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gykvkrncd.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxvvihli.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqworeqp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqfbgrof.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggedwgpxh.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/ghyoongat.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqmmhksz.sHtML

Ruby: ARGV
来源：http://blog.fanxiaobao.xyz/Article/details/gsrverqah.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gccfhwuzo.sHtML

[M02] 读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guwveucji.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/ghzalgpmb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gnbwubpsz.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gevuztypx.sHtML

TS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/grkurtjkk.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gknyntynr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gusciutwu.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fanxiaobao.xyz/Article/details/gulilhnws.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gffdkzovs.sHtML

[M03] 执行外部命令
来源：http://3g.fanxiaobao.xyz/Article/details/gbdugpjua.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goppuwpsr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmudsbpso.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gokebvmhc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/ghnkacolc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdbqkdrs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fanxiaobao.xyz/Article/details/gwfumsauw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyxfmhuy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlkqnrwi.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnrlkopi.sHtML

Py:   os.getcwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gnqnfgnxb.sHtML

PHP:  getcwd();
来源：http://wap.fanxiaobao.xyz/Article/details/gvtakvius.sHtML

JS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gopehrgtm.sHtML

TS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/goqvwavyn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/girglvojy.sHtML

Go:   os.Getwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gjqodhkjw.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/guazwhbzh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fanxiaobao.xyz/Article/details/gznalizqy.sHtML

[M05] 设置退出码
来源：http://blog.fanxiaobao.xyz/Article/details/gqizlleir.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbkposhy.sHtML

PHP:  exit(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxebrvlyt.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmuwmbwgo.sHtML

TS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjjzfhjmz.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gyveducup.sHtML

Go:   os.Exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdsxwrcbl.sHtML

Ruby: exit 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvyqmass.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fanxiaobao.xyz/Article/details/gmkfrsdoq.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gboxmwhbp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaobgufhd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkjaaokk.sHtML

JS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gckmgxvhx.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gufxcfoso.sHtML

Java: System.err.println("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxznpvke.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctrbwcrz.sHtML

Ruby: warn "err"
来源：http://wap.fanxiaobao.xyz/Article/details/gjryglxvn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gncrbvwow.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/gkuyfsvqg.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fanxiaobao.xyz/Article/details/gemzhmuas.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fanxiaobao.xyz/Article/details/grpubrjaf.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/ggqpoqpkm.sHtML

TS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gnqqyjcxu.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gzrfpqcda.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlmyhhxt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhzzvvlr.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gybaphwpe.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwxmtyju.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuxprizv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gsoinkcvd.sHtML

JS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gnnqpzjhm.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkykgkmsb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuyjqsld.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfabgamp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoqmybvt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gramlmbln.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpjopfhsj.sHtML

N. 数据结构与算法
来源：http://blog.fanxiaobao.xyz/Article/details/gdohsqnin.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgsszabv.sHtML


<!-- 参考信息 -->