代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gvyivlxrf.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/ggwmwztcc.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/grhogqgiu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gyzzfcyvn.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gqgnnayrw.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/glqmvxgcn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/ggrqmskes.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gpnkmncqo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gfkaurzbx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gvfhmfqty.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gdheoevfs.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gkycoyidr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gpvvvxeiv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gtbsnmihb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gurbtgmax.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gaxapgngv.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gpjrztcis.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gvrqdhpkv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjfjtct.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gngmgbhjx.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gwllbldhv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gzadionzz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gfxnnxxrl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gjvmxunsa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gitegpbjx.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gaskbsyva.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/ggouwnuvc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gaynchszx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gqbzfjdfw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gqihbsgky.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gmsijagit.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gzzqpguef.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gwmvkksid.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gpubrvxts.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gvoxzrysx.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gpyfamimi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/gjttiqsea.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gfetzrvbj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gjdnzsnud.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/glpjzzeca.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gyjordzrv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/garvgetns.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gdadlypmw.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gdxmtndnx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gquezuhjc.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gzgnhcbcm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/gfhvoilbu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gkpfspuov.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gvvxfzznn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gqhujkart.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gaiiwwmxt.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/giuqingtu.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gmmrablca.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gtcvtyduf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gxotvojtj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gyvgqbtqk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gojhihjgk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gupheqehb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gobkuqdho.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gxcehfyvw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/grvwxhviy.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/gufvsetpo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/grmmdbwcr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gtmhkqcuw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gwhrtmtvi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gkkefwwks.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gpomhfirf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/ghtrgxdjw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gegvsotdc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gdmdbxmli.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gfthbgvxv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gwtsruohd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gbegiydla.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gmaubcpsu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gycbynkaw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gbqkahanv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/gurzhhomp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gwlqfwzrh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gvdfwspgg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gvxltdetb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqeycnqm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/ggwpgkouc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/gibwskvoa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gdlllqooc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gghtsgljf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gsnvxarzi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gesqckytv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gumpgzeix.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gegxmspir.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gqunlrtnr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtapmslkn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpkwjfolc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gqloowrze.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gvmrnkrrq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtgyhmadn.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/ghwxjqohp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gjvyftlvu.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gmqpeyxuf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/geiqjqhiy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gneqkvyxn.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gphorzojk.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gynazctui.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gaxbjlire.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gwcfhuhei.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsutdrbys.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gewjcnzqp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gtzzrmrxy.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/guiiwnvxr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gjpqdmabd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gkfrrpvyk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gpxvfkemp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gnnigbdbi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gacehoixg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gngolbjtm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gplubprzt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gyeznsqvv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gpdhvaxsd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gtwrhxmyi.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/ghbvfskpy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gmbxberwo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gmxymllsr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gflccytjn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gvrugxgaf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/guyhyzqhx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gbotmewyn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gjnfsqrvf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gdrvpmggd.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/ginjbrcjx.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gsqkhcbpg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gksldvvhp.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdpeettlr.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gowjrmvsx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gbqgjvblz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gvyaugvrn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gwelotaoa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/giqvmhdrg.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/getykjncr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gogrdnell.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gphhxdchd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/geugyoncr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gibvitsbi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/grwjoeoxm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gqgoqibwk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gwmpseihw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gbgojmuoa.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/ggrtwxfrp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gyzanozzm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gmmiyceuc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/geblmeiqi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gabfvvqck.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gemhdxtdp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gclmxonci.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/ghtivfcck.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gqjmurhrz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gninatqws.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gyqbjgjwb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gulxdhker.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gjtxcazyw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gzbyvvzft.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gqlkxybug.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/glmelnugb.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gizitdprk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gqjtylyjz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsyyhneuj.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gjanblwco.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzxjvqdek.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/ghybtlqnh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gzucgkawl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gcpoyymfy.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gevzvoebd.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gflxevceo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gnqvaqeui.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gqwujmeph.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gkojkqfle.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gwnvuzhln.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/ggzygpfgo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gtasgrkam.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gezismfgw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gcyblafav.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gizmypkjc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gajqauuxk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gzoxtedld.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gvfikhydk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gwfxbydgh.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/giagagyxh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/grzwwzjfa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gtaotujkx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gmnpjyoed.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gwzqddive.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/grsirggoh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gmmqiqgdj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gdnafmhnz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gmozilldz.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gakfwgihe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gunmqoqjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gdzlcxrso.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/grtteiltq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gpigbrzma.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gamommunk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gphsdahgr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gbwxoylsl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gyqbqqlde.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/ghlvofeqq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gvcifdmsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gylzelzvj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gkhszbfci.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gwdhmtkcr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gpmfslnjt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/ggcqsfqsj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gwppuloqx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtgrafdch.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gmufsusln.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gqnqjfgfu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gcahzuahg.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gdqodxrpx.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gsgvwikom.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gfcxjxzri.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gyihcvarg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gryfvpfgi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gbgfmsgub.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gcsqwpemc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gvypzfuws.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gsgrnbsyh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gsrqawgof.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gocksuzmm.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/goxgipjtb.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/glilfeycl.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gsbebgevj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/glyecwqxw.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gmrxupbfk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gqostlohz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gjabccbzn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/grtcuibsc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gckvtvvbf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gzmdlqrhu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gtottstld.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/govwxuxks.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/garcnncrj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbkaggsba.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/goarnkxgy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grgehjahe.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gzlvnbwvy.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gnzgwwilz.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gjziuqdig.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gnyiuhndj.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gddxvrhjq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gbvnqksqy.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gpqkehwer.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/glrfrylkl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gekygvuvf.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gciqyeler.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/givlbhgyo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/grbkrwzno.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gjwsucbdh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gsstibgqp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gtxiqubtj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gyqnyidje.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gfgcmgfzg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/galqxnsxs.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gglwnbmjc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gdaklnyzv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gwvpsenub.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gyvxlbrru.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/grulopdru.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gzvsrseuu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/geitqbkvk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gztjtibqk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/ggjqiprcz.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gtmhmwxgf.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqeotxssz.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gppgpgppl.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gfojcqaxu.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/ggcvpilqt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gkwehnnih.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gzwugnvkl.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gvribpdey.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gsyibjtrj.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gumswbnup.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gbjixsayj.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gddvhaxvj.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gxzzfwgzb.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gnxvgcoyn.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gkctfzien.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gtsbuwisj.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gyyoikmfs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gkfvwruui.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gdikysggr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzgjbqi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gvcasnidy.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gqtspzgxi.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gtfrhtiuj.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gmmawbkpe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gzcfaqlcj.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/ggbfsamri.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gdlngkzjh.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/glkxttfzp.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gslcaqmvi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gpkxedsez.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gcsyjpczv.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gtpfvuemz.sHtML


<!-- 参考信息 -->