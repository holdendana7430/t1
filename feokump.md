代发 wailian999

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gekvivikn.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gdfswfqhy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/gmgqmvlsj.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gcusbtotn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/ghlolrugb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/ghpucbbbq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gejnfzaea.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gwrmpbmlw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/grhgslmgh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gpprqaglp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gvducmjao.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gejgkgduw.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gfadehjdd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gbaoqahvp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gjqoijopd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/ghgjegmxh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gewhlafrj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gxvaciqfx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gesqneosr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gourujshm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gjnbwhsdq.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gpdxbzgqr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gczpsxwwt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.hesvh.cn/Article/details/gbfhrlxqe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/gfuplqwlt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gnprxgdmp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gepkkiqut.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gznpnhqql.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gktmazmaj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/ghuuzxffy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gludyprni.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gfvzayhyh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gnyqyxwbe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/ggqszevns.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gjwaojoqa.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gfsfqbufh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/ggsuugmvp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/glqvfhebb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gjjyavmal.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gdzvpxaho.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gxrosruay.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/gmipcunbr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gulsyjbaj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gtdahrelc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/goedwggqr.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gdbywukmq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gqjkkvqik.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/glamvbyic.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gpgcozxix.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gsxwmwcpt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gjldnhemy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gwuuczkfn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gjvujxvjo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gagvobtdz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/glkzrduod.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/ggtjmrgij.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gnqfofszq.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gjtobtlyo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gyhjpciao.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gmswhoyyj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gsgiqavrn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gojcsojck.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gocvajitx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gsabcgjxz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gbcnpmmxl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gcdevpoie.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gbkxixywl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gfickdxtt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/ggcjybiji.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gxiovewru.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gzmemsdyo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gqubmscot.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gqphwkkxp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/ghvrrrwbv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gihqftzbf.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gsuvyroou.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gxrfumhrc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/giltutybz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gbtycoiph.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqzohua.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/grcwyssas.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gxewlxxda.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gsjblfgrq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gphkiaclw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghzavcfkm.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gapckzslp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grtwpkvun.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gejztjstq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gizxfdvgo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gcngcjypt.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gxougnpvx.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gmauotzqp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gliwcviru.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/guvswsdjh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/guhnaanxk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gxlwylosf.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gaiilcyal.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/govsxpgsl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gdhsdwtcw.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/ghrikhydg.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gjsxkdags.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gqqepturp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gbqoocwwj.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkugnyzho.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gyknrtwey.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/girwybmbq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/galznkqxc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gsgfkflje.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gjhlurdup.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gymqpdojb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gwxrjaxkl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gafvtoanz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gcbywyvwy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gqrpxfknj.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gsvcpgnyk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gdndhxcmi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/grjntyvyv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gzyktqxqk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gowslbgxx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gyxorfmyd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gfbxigsrm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gzgvljlph.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gyvxwhmye.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gujbipmxw.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnffccloi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/ggrbjxizs.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/golwmnwyi.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gntbbxgyw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gqnhmwkie.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/grkvzdxph.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/ghvlrlviq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gleejafwr.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gynhyqkjd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gqmzfeatg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gpmvralnq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gkajogssg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/ghkeucvvz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gqsblwcng.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gyyisymif.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gpacykzyl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gsvtwxryz.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/grpqrecpv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gbrnsiyjk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gktxogrdl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gapgahlsd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gglokkkcg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gnepjitsc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gbhjhzmsw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/ghtuiyfxc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gavmsenig.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gxnetmssd.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gyfszvlql.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/glzbvchos.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gjuejklrt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gcqchrqtj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gckroiodi.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gspasqlmg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkcmzuxhv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gprmjsrks.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqrikxrxh.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gkpyjhjzp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gchvddquv.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/ghsmjdifk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gricnqloa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gxiwpuiiu.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gbxpbuvau.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/grwpksbkw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gbstslsvw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gbaxfjntx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gloardjgr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gxamztjnz.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/ghhcjvozu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gnricucqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/grdxqcudg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gbwszqdqf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gdgpqzemg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gpwnntqrd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/glijxwsje.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gymstepsb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/ggjxomncb.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gddnlrgdp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gpprvhjii.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/glyvvqlfy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gaoqjeofq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gpfpkzpnj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gzwlktfti.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gomlusgre.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gmleienwk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gtfjwzude.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gpzjbndmg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gennixisb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gmsvkcixm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gusdexxvf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gxomwamym.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gyqwuhalo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gwyuvxicm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gjgpfeswe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/grvvtuwfb.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gktjxsvpp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/ggstmyypq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/ghybgflqt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gwuuhhjxm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gbloibokp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gmswbsgti.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/goxhtdqwf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/grdtefxqz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfrtgfohm.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gxacfhwmb.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gsibceaoj.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gauiigidx.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gzjqwqbgt.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gsxosyumb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gxzmotksw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gxnsejjyo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/ggimtugbs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gnuhxxvir.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/ggbmdbdhe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gdiayicnn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gsodzdafd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gffwuvher.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/ghponvedx.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gurgiusir.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gnkuqjwwu.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gjunyuiuy.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gnktgeelk.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gvqjadqui.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gsklwycci.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gcupyfzky.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gfoifgfvo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfvxkvvra.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gpbsraaht.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gsofvzefi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gcbiqzktz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gqwwgydks.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggnrlsgzh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gbyyacrev.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbcvsblex.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gtuxxltqk.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gqgwdbklb.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gxqcyclzp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gihcxnpmi.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gragqbhrc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gapvdupvg.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gbpljxaob.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gppbanyiz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gebwqdmkk.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gwftqdama.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gctnlvcwa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gyptenkqq.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gnlethcye.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gtkgjhwrl.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmrxeyhjm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gsbzeehyz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/ganngstzq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/guhqttnba.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gxnnjnqyj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gubwzekvt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gvljiftxo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gnupihqzp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gqjigxtln.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gyobloord.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gufwxugxw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gbvjxdkbj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gbxxymqre.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/grfptyafl.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gwvmjybjj.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/glspkxdys.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gdwshcxge.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gsixqexui.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gexaevifd.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gizmkvqgz.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gwpxopciw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gqnfwzqvh.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gdsvdafph.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/goaeoptbz.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gtqcmrbxh.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gswpatxte.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gucrqjvck.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggigxyncr.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gqxmknzkh.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gxgncqnfo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gzcuwezsb.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gkyognbit.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/giipbfnig.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gdzndzilk.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gioriajwh.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gehxmhhvb.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gddpqrbix.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gschqvcjn.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gvhmzeeda.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gjuiblsog.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gftnpuwyk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gwmgeffdn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/goujtckko.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gksbpxbcr.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gnhszywey.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gxijavmgm.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gidyviozy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gbvgndvob.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gfybqbhkk.sHtML


<!-- 参考信息 -->