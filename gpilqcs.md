代发 wailian999

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gxpdyaiqk.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gnytyhgfk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gxjvbnrfh.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gresksgzn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/guhsnprbe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gqahbvbjv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/ghiemlnkt.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gyrgxcvmd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gmkvgfqqg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/ghcntfyuy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gwkqhkyef.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gxjbcwpwd.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gwuvjrqfu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gvktzzfbo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gyegodzuw.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/goicqgwpb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/ghmkqurhm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gwkmbecnm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/glbvyqmnn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gglgbuigt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmsnhpxf.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.hesvh.cn/Article/details/gipzsxqut.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gkrsafqtg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/gegarvxtg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gammswehl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/guvihacsi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gmbkjnjhm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gnkzcczgt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gwcfqabml.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gunyvaimz.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gqbmmymno.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/griknzfxn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/ghjdngfxt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gemkevscz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gynzvjrlg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gpoxykvfd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gujnnxltn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gowfydwtx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gsgnrrntm.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.zdbjq.cn/Article/details/giowsjfii.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gkhnqxwqe.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gxrotsyzn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gdfgfqiro.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gwzhsijrd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/ghgkuzxhz.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/ghywqqjct.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gqcxkzles.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gzarkrxwh.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/ggcdjsbkv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/ggbfjimzp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gwnbqbusx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gvapujspd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gkrmektxa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gmlcqzypc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gcukkooce.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gaxxuujnz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gsybanebk.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/gvwcvddjx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gpmjvqjbv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gbqtknqpr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gixxkfbvl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gvlxojbmw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/gizfpaozs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gbxuitlyz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gdthnebab.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gvywujehm.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/giuhxnwix.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvckcfhe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gfdjdvitq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gdwjnvrxc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gqjpxrcwg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gyodggtxq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gqflbzqit.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gugpiuzzb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gyjxvbjcr.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gxjuuzush.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gxpcgxsyh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gdsfkmwhi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/gzimyworo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gnrnygfab.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gjzkqfhzf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gyacqtrvw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/ggiufwrsa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gdbyvorhv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmcwmyf.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gtbfbcfey.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcufgfpdn.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gsibqabvj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/grkwywkik.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gasbgkobx.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/giixpufio.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvxgteuki.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/geucmtduk.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcopreqjr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gamyhctxc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gnpxrzxjj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gybklivov.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gqkchghhv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gcuvlbqiv.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/giphvmgru.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gogbpcobm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/grvmlqeun.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gcsxwepzq.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gupwdoyuc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gqcdltvof.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gktfjjmfh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gbseipqsk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gahgoomuz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwshrklpl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gbfejanwv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gpuresfrj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/ghpfparqk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/gmbfqjxjl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gvessoptm.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gcadrlafz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gwybnjwej.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gdasxouxe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gkyltkiyn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/ggsuzyfin.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/ghmjkkdpg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/giwtiotuz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gcrzlevmp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gkyqemaea.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gjltgsbhc.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gflyebmwi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gfuxfljmn.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gmvajndno.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gwbuuklll.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/ggahksqjm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gtchqowkp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/grtaljglu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gugtvvtko.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/glaauftht.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gimresxkb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/grskuazek.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gwlrhwbjq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gbomozucw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gcteiuywv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gtnpnwsud.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gckuboljl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/grhyrofnq.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gyhjxuawc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gfizvnrvw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gkonvxzak.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqolkky.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gcyrlaise.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmyreucjw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gkyrygyii.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gnfrwhmic.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ghovbpaew.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gcwlsvyuu.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gbpgdluah.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/glltgpnnr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gfntfarzu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/goawvxwtd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gfslpddhr.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gtukofcyw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtxbhvosw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gkmvcquix.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkobbntgm.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gqojrbmre.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvyugvxbm.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gtopwyusc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gtxqjsqxs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gtuyqmmps.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gjvjwrspw.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/guxolfnlf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gikodiihb.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gqpltxfei.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gmrprsckx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gtqrekttq.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gzdhvdnah.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gzcwtqwdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gtuboyfmj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gysroinde.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gkqyltegw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gxwlgibwc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gqccxnyln.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwjoxrlz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gtbqjltnh.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/galcaolvu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/giicohuph.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gpdavibzc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gngjirotq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gwxlrqzcu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gphxzazwg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gsdblmgfr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gsleyldna.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gvjicznjh.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gqclyjdkm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gzmiwvhip.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gonlrllnp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gqonjjjkm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gxfdwsfpq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gvejnmdxr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gkwscjxuv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gsahqatog.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gucgjnfcj.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gadndazmq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/giouygcti.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gxntrowth.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gumttghir.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gylcnfkmx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gndkxeauq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/grjjgaeld.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/grexiuxfy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gctvztsol.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gsgavxzql.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/goxwtuaca.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/groqzealy.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gstawraqj.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/grrjkitns.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gccaypwgz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gwgktxxgf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gsajefbxp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gwjsxygtv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gwcipopab.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/guajnmywb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gxkdtldlr.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gmsdrmsyw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gccymehrn.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gdlmjovqa.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gcwypsqyz.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gvduwquqp.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gxeefrgnq.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/guwzmeftq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gcsrxznra.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gbysktxzw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gcybdplgj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/grmnzsnne.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gnqyucfio.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gjfwbzyaw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gdqlrqxei.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gkqcgvxxl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gycwwxdad.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gsspbspwd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjghdrnjf.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gnslvcghk.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ggaincwty.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gbtpffsjm.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gsmxppjrp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/ghvmizvlm.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gtugsnhux.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gzmbqdpxr.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gsixraapt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gxbrvvuaf.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/guqtaivjb.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gfrryctta.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/glbsbsbio.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gxjqfuhsj.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gdymmiktn.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gmvjxkqom.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwvxyyzd.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gvcdrztjg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gywvxjkbx.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gyyqtowgw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gwuzszbqy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxzuqzn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gytznkdcx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gevwngdgo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/glzrhbsek.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/goetqbosx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/giwhxlsqh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gqkbdogdz.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gojfpbnlz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gnezflogf.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gffamdqkw.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gupeucujj.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gufofxldz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gphxbcfdn.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/glxwbhjrj.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gvnxczvke.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gwxoesefr.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gbfclgvtu.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gqvokbjmd.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/guqteiwmg.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqnkkabhb.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gkfhoaqhh.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggmyeropj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gbnoacsjh.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gniayhwrn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gerghlbrp.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/goevymphb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gitdfzogm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gfoltenhv.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gcpntpsjd.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gvrkqnnpq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/ggzwgtrav.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gtnosxhzg.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/ghwtuifky.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/grvwubmqb.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gmvtgmfjd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gxritxvde.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gttbtjnwb.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gzuyhyqvc.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gwldyhoko.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/grgtokdpu.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gurmcebfc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gdeozookm.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gbymkqrsd.sHtML


<!-- 参考信息 -->