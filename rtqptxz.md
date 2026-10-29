代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gydfirmrg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/ggzizgtpm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gsbwgmwzl.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gwnnsslwv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gfzyrnhfn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gdxiictik.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gbkstpycn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/gxkrdqvra.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/grpbzpzvf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gnwhsjrlw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gkysuhxgh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/guebexdnd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/grkoryzqn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gmiojoyjn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gthfzccin.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gxytygmnh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gdcecowql.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gbwbppyum.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gigychndv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.hesvh.cn/Article/details/gngianekl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/gnvnhrwzv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/gvpiqjztf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gesfasmmt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gvwlwhcid.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/ghzefzzjp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gququfyjw.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gtiewyzqs.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/gljaymyqz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/golhkgzbi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gxxoagkkn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gxuhucqis.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/grrsgjcno.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gyjuzusvt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gcjtsulvu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gvyjjblac.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gnhrulmgr.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gclnpfwqd.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gigjznwmt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gnkccfpsb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/gmmqbtzuh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gucqwntjp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gusyirzbj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/gqmelshbh.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/ghekeqipe.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/goxpgvzod.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/ggpfpkaxv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gqwcexdel.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gjqhpmhac.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gwwrvzcwo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gfdapniri.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/gsddualzq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gekjsmpcd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gfgbltcsu.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gprrrekud.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gkartomxz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/guyjjutzd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gcfnvgoxx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gkaeuxyfm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gtcgzggle.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gjhcymqan.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/ghnvvkqbh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gbpnvjtwg.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gowgfrdad.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gfeggfwzg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.hesvh.cn/Article/details/gvkqqoyzd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gnhcbiqfv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/glrfwsnel.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gcukwffjg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gchwlvbwd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/guifqwqis.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gpaqathlq.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gfmlihsgj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gxnodnpjr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gjkqymwpa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gegpvppej.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwngasitu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gbivbjjnq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gapqfxdef.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gymxnoxmh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gkyofxmdx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnvvtwjaq.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gpojdtyob.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpfspprtk.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gqnxhdmbi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/ghnlufbaj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gioeqkito.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxewznnei.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/ggzoegvpm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gbkwumevq.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gvimabokr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gtarslkxf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqlcpkhqa.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gqumntned.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gvxrcwkgj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gkvvxeigm.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gpqpnxuyr.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gvzpljvdb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gxjqugygm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gvarlfobp.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gmoljkplg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gvylzyjqp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gnqfvkpqp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/goestjkdl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gifoidsec.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/goyvgxdgr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gognqzrnk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gnacufozf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gnjcktrop.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gijlgyryr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gougnklqe.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gqobhwqyn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gbvarevpn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gsdyufpxg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/guwaogqcd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gctudzrut.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gvgmhmlfz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gkhmrwgrm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/ghcijrgsz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gwalvuzku.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gmfvozqcl.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gmsthqqow.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gidgcihbi.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gcnukwtjt.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gykfxvrzt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gfunuikth.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gruzlrwnv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gwcpdgwhq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gbfscelfl.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gqsntfanv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/guckxzdxk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gyqjpcpne.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gxqxeiukv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gldqimghc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gcxozdgqs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gnxkdzihi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gjdpkyojc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gifnyfqql.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/ggswpunel.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gqmujhnub.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gjohccbrr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gxuissdhx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/goeojpili.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gymqnayrp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gkiinhbsw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gosdpjarm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grkmqlvor.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gilmqylpl.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gpkrjyyqp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gssnazaap.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/guwiaxrec.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/grxjwxbij.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gcdczdryl.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gkkppyrsi.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gfincooro.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gukwdhail.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyhuhsvfx.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gvmeqdhxf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggswukmmd.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gooutebyp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gnjpqjlep.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/godqyirnw.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gfebvlvez.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gbslaokwg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gmkvtolqa.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gqbzavqhy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gaigufkqg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gsowygxva.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gfaiuvzil.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gugwnkbbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/glscwmaew.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/ggtjacxol.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gtfxubmqe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gkpvddnzh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gffpahuxy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gsjrloife.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gslibfggk.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/grdlhadiy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gjogcqjfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/getgrusal.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gxyzwjgam.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gipnodjmk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gsuoaxfpi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gvrlhhaop.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gsdiseugb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gvpjkdvkm.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gombuigdm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gjwquttni.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gqqbkmirq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gkadhmggg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gmirzdfba.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gxelzsmlc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gxrpvocvb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gsasymsfs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gkxqzojar.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gngemiwlf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gcbpzzoai.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gushkkeit.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gwhkwqzda.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gmjwgpexk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/grjsegawe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gsqjhhsvw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gkxknnvpy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gofksaqiy.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/galjzfyem.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gnveuldvn.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/grkdedcij.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/glohkwjdf.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gifzpwxhi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/ghpztgtvr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gfiegtwup.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gnnkivoku.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gdusnrarn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gzpoxmkcf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gspypuszj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/glghzcxdz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/ggctvbgqt.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gapxzrkri.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/ggqyalcpb.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gltuzjnbx.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gevgtaefz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gjjtnbdjf.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gfocftjbh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gdekoftaw.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gvnowylvi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gbarnvltz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwddquxwb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gjvbuadwu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gnngkjpnh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gjqdyiaem.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/ghzinnarh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpsfxcssa.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gtilbsvqm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfkqqbeyq.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/glucedeij.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/geknbzctz.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gdbkwzudl.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/ghiesciku.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gtlscztmb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/guroiklrw.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gonwjufsc.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/glsyivsrc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gavthgvsg.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gruaxcqco.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gpkwrufgn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gaqucfgzb.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gvlyvfrri.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/genhlerqy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gscbkffhu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/goeygqqof.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gentazqvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gsiiimljo.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gheugnlml.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gcslgmvkz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/ggaidwhng.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gzpdcpysj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/goxbimsuj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gvbtvxvpk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gbysulfbb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/genixanjy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/ggofccksh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gppvafhkv.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/ghvwjbozs.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gifoopqlk.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gkmpnintp.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gqpshkunx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gliplqimq.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gmshwhyyr.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gnpixepmi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/ghrieueti.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/grkkhjypm.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gjthkkpio.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/geqgszqes.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gnmvgmqev.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvcbggzuv.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghtbkdvvj.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gtewquaex.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gjkohtyaf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gdqorpsoj.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gxxmnizjz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gwvvopcdi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gqimuaysu.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gusgxjgix.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gxisjkotj.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gowowlreq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gohrtkpaw.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gzgsvkupt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gzktmnwnk.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gvcxbrbov.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/geljmlegv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gigpbthpc.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gnzpfiiah.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/guokqyizd.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gztcuftrh.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/ggotyscaj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gztueduat.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/guaioolmh.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/ggcmwezpk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/golmzxuel.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gtmashary.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gispxfwoh.sHtML


<!-- 参考信息 -->