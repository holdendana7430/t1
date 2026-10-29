代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gfuzabjyz.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gvrnkzhrz.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gpdnpxyai.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gfivfrxpf.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gcywksrzb.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gblloudsr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/ggfwxfrjt.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcrqyxrjq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gfixneeob.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gmwbrfetp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/ghobkydoh.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gwfehxtck.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gggrjdmfe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gyjtieovp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gghwsbvck.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gxyzgvzif.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gpsafjmhj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gowdrxwnv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/ghspqbkns.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gbvqshugb.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gbgjbizon.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/glbvuuyqd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/glydkvyiu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/guzamyidm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gujjjcxwo.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gheawhczo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/gzkwfjbuf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gbkeqwbto.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gnsdxndbt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/ggickhpav.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gqktfnsze.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gvdjeqfmu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gwmumcebm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/gnnuokkah.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gqogmqmcj.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gnsevpslj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gpndpugsr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gwxcmtrfz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gbcoylsug.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gaylfzyyd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gscepuerg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gvbtkodxb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gwdnyxktt.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gdyjbvvug.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gewrjdfmj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gypihhzfb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/gvrzcuiwu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gkdnjnfoc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gmgjibymf.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gvwnqdysc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gowubksjp.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gdnqahqea.sHtML

[J07] 比较两个日期
来源：http://mobile.hesvh.cn/Article/details/gdpicbbdg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gaizbjuem.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/gdywqxmgt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gyqcsnjuf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gitdxaigv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gubedrxiv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gbcloyejc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gzioxptlw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gcfuydthf.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gsbppvrfw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gzzsctjuc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gigmupdbc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gwhhwaglb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.hesvh.cn/Article/details/gmfzyjqwe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gaxvyjcec.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gammplmub.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/gtbowxbqx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gyusfhswh.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gupiykgyz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gaypqlink.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/glvlidnaz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gsstpjnky.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gegkxwgdh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/gqgugjfzm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/ggaujvtth.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/ggnrhpfzn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gtcfslado.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gjloreziv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/gkcstrulz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/guhcyiqbf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gbkvaevqt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggrxilckv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/gtvskxsqo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/ghqhdieta.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/gvcuxjqmy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/grqtaupdw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpayjrsij.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gpdtrwxev.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfdcgdy.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gwqtcniwc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gqhlockxn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gyibyrjtx.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/glbbquyuv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtqrvwdqc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gwpkygvrj.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gzjbwolkm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gkqdznkaq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/giefrjmfm.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gtydktxxw.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gficvdhvz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gtuzzenaf.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/ggrdljtvx.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gesmkssnf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gnnhcllme.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gzihoouba.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwmgbtfpq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gahmlazro.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gojjudhsk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gdgrbymze.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/galndtows.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gnschamiw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gtomicpwc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/guzxabrdu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gfvwmpldv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gabshaxtx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/grnajqayq.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gdubvewcz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/glqahfpbn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gmyorlnvg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gqgqlzgpj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfleaxqcc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gusicidub.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gcistbkbo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gakxlxeeg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/goqvcoxhs.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gavfwsymx.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/ghfgfttah.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gpcjeiasi.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/guewoclwn.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gclkaeopx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gxbqgxhrx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/ghceztzrs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gdelkatpj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/guhmufgty.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gqwkayipt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gphntnbxf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gtdsorsas.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/ghybrvncw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gernepmxm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gdmfpitvp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gunltpbqq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gelexbcft.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gavpbhmvh.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gnybwnjdg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwsmmocfg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gpyyzjlin.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzbappqrq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ggdsuexok.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggpadeatd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/guhzadszu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/grnnywzim.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gxnmndlnf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gqltyxbaa.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/guoopctkj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gbjlgqveh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gezpwdqbc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gvyglcqnk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/ggpoggkzg.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gaeouilxs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtwikbbjt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gjizkbsno.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geehopcpq.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gqkbfuakd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtihayppd.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gxwlibfsb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gxgsgrjix.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gdqpschyd.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gcqwbfhqk.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gvtyvxwzm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gjbwhbcaq.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/grecdknhf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gzapupljp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gcijuyhjj.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gvkmcwepk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gjgjhptvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gnlwmhekj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gsercjxcf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gfghwktal.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/glgcozbet.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gdersbjkk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gedrdeshl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gjcpgnbfy.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gelniutje.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gtrxvggor.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gtgkcypmk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gocpzzfke.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gkfxcxcyx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gnbvblztz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gvtymuhjo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gjisnlhkr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/ghkynxgxn.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gzebnwqti.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gkybijvqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gztevapvh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/ggspjhpxw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gmtizfoyp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/guorshswk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gmsnspobe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gqghdxdce.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gglmhgigx.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gcgdbidtw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gznmhntfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gbaurkmuq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gedtrqcvt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gqrxcrmcv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/ghvznvbhd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/guxkqfana.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gpntzbtqd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvybmyraj.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gwflvsiby.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gyyninazp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gkvmeqagv.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gdgmoiuka.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gskhpyaki.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gujfrmnnw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gfljamhuz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/giobbavll.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/grnjwmplt.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gkefryejm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gvwhxisjg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gnmcsrcid.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gzyvqimmz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gvpnlciwx.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/guyrubixg.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gencaixgg.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gmlmajfdy.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/ggrpiapoi.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gdtdjdgxw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/goxfpgffj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gedjjwjiw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gtoohvmmw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gdjwwilzp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gswjlmeoz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gposbkpvl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gcrklgvxb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gmjyesclz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjecznylc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gwzasxdhh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grvtgereg.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gjdmxsjjv.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gvwjuznec.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gauoeimlh.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/glzejktan.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gtkgnktbg.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gbnqltgoo.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gsnrnryeu.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gyaqzwiwu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gxhrgwyaj.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/glyvdynoz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gfwxixmvj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gkxawbiha.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gjslgjdxd.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gvxmwchoj.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ginbzztjh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gtwdlbhhy.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gthxwxbkl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gpqqbyzof.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gwxekyyfe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gjvgctqhc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/glzmjwoqy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gaotzrhmv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gecwtwuyn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gmbkqclhm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/glsvayzjz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gakaiyrns.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gosxgxmck.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gyhjstiuz.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gcfnxtvzu.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gwgwpaqez.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gwcjqdbdq.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/geeaatbgp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gphxxklgg.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gptwbxtii.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/glqkhlqvn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gqjoiolsz.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gseksnqno.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmmzrdbdg.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gimxweohl.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gcwbnurjb.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmkbxcqzc.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gmhzijsqb.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gkgehiurd.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gxzieaapt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gepqbnnyf.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gpsgguizm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gpwqgasnd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gqvwerqnk.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gjqvqocos.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gjitfqavc.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gvbvnwerh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/glolbijmj.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gefybunup.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/giexvtcms.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gaqjbhzbl.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gakxemtkh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gnrpbmbll.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gunbhpcpf.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gkyyiwdwc.sHtML


<!-- 参考信息 -->