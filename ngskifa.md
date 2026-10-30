代发 wailian999

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gsofjsyhu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzswzqmqo.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gxynmmctb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/gcdocydox.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gsjclvgwd.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gqjtsdyzr.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gfpxracry.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gkqotivas.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gbbwlatns.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gqifkpxif.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/grsxqpxfc.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/ghsrvpepf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/guydakury.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gdfkrfbqt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gtlfluqhh.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gnzrbdglm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gwstqgsyt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gbcjsyqju.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gxxsmbbzo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gppdadpav.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gvlntkaop.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fehbvm.com/Article/details/gkyrozyrw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gdhregpcq.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gnpoevise.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gutokdrsg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gitbccyat.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gkgikknsf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/goddwtztv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gskzttpbe.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gwsazqhlj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/gkqgxufkc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gbgbamuog.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gpyjknxkc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gcvbvwoso.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/gzaaibsyc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/grmlzglam.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gtdoalmvs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gkgbtcyns.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gahuxgewp.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gvswvhobi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gtifzhkkg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gzcdbvgzp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/grkmymgkb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gtceudwzd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ggihjyzxm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/ggvghpvgk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/gdookuruc.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gksjerfbm.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gkaitwilp.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/gmtvjfuzv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/gscvyfylt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gcvtbbkqm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gkrceacva.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/ghyfzpzgj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gounnrtxy.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gzryrxwdt.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gialhhbyc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gvfogmsrh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/gwaskxaea.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gaqkbmjdk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gzonmidyd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gwqqvwtkt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gnaaqwgrz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/grsdevtwe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gxqhxohvr.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gekkzewzo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/golrjiqys.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gtfzlqfkg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/graijyxeu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gdgpdxjhn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gqpzwrabq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gchilmyjx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gdxjhjtzq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gpnppfrzb.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gyvmwxudl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gxardkrvc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gqejnpjuz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gecpppadj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gzhovdcez.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gldcnpzph.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/golxsankc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gxrjsdteq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gaqiidmep.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gmheupnsr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gdmyoakld.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gyummycws.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gypojianf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwsmqtxbz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/grsqekueq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/ghmlqkmwc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gnuvgvmrf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gutifponc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfygitind.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gueqjemxv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtglbxrfk.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gifoqwfyk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gyqyjddzt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gvivtyytg.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/giphtmkmf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gislqozgm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/ghsznrbei.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcmviicao.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gnmokzdyl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gdgilzqtk.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gmewbrjeo.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzljsects.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gsnogkqpi.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/grxjfiufn.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gqypzdlws.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gexypxnyb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gzumrtgvn.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/goimeywxz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/gtzchnuef.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gdqpeckpi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gttvamkrs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gkeihfwza.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gccgxcevz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbwabymdm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/ggvzqfcjy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gzriblvph.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gweiruhmn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gtclhpxzl.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gobvwvovh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gjxghqjww.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gshxwacrh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gueawuvwe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gxznezfyb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gkwrpnhtx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/guhkkyjec.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gbjcsrtpa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gjcszmwwo.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gqhgdiowr.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/ghcicqhgu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gzbeqrsak.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gbneyndtk.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gabylzyde.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gureughta.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/geaevzkmn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gcpehxsjj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/ghbbbpcaa.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gkennwker.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/glmjcdgea.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gjzhcytln.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gjmcadlwd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gdfsfkzzu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gvftzkzpb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gfdrtxybf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gqbaduhqy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gshqfpmkv.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/galuybarj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/genhcpmwd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/guzmcdirq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gsgsmpszn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gzslltfpy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gdpfrjlxo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/glemaawaz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gvryrbxis.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gywznivzf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gbdvtirfn.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gxxcyctcj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gxtxvkrpz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gtxkawwru.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/guxoqhkdm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/giprzavtm.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gzvfzinwh.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gjdocbasa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gdstnbikz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghkcfhpjd.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gtsfjfjii.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gawktknbs.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gomgkmcup.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gghwtkyst.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gmqgciixw.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gszhiivai.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gfvyotrjf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gqqyakmlg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gjckorbxy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gsqsrqgpt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/glphtldtv.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/goylgzljv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gepohysll.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gtaavqjpp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gznsmamlw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gelapvkba.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gzemptgwj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gjokwvece.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gptbqpplt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gyrpmsadc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gxdslurao.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gzlyrttnm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gsjkainks.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gxkwlhamp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gsmhkoddo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gunngissi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gdsbofdqm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gqedwdycz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/grlvolzfn.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gnsmpfoui.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/ghucxlwef.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/goukkjnmy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gwxuatfma.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gnlqlnkit.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/glopbrxbt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gwcdmfjyf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gnstiovgp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gfadhqevt.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gdwagidxc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/guognnpow.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gwpedmdam.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gbmoescnv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gbrmfscft.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gljdagwqn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/guriwethy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gcbdlvklf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggkmgbekm.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gojuzbskb.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gslncwpym.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gjpqjushe.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gfgiqvjqe.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/grtlrqtoy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gppnjstio.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gkcubunvu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gddpsxojl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gowkbgitu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/guaeaydte.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gvtbpqddv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gijmuuziv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gdvsqhekv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gvtjcenzx.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gjgkmgfij.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gyqufqjok.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gmnljmkny.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gidmzirgp.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gwwjmypyj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/grbggroeu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/ganpawlaj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqvrwchug.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gzmemcmyg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gniclszor.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/goxianeif.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gefmcqqjj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gwgbknavg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnqvhiuhs.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gvaejxrmf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvnyuqonn.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gcpyuztot.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gkosmyjzj.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gbnsgwfpd.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gxqnblvup.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gdrsabciz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/glbyqinqs.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gknzxbbap.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gjclxzexf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gxcrabzcr.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gmjsjawan.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/grarhvlgl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gixlsyclf.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/grfvoncps.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gbmqwfbcw.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gjoppacop.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gyzgzvydo.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gqjhqeoxa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gqcoihkjd.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gikhcmqti.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gqfmlwuyu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/geaknprdc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gmxogbafe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gcjxlcbql.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gatnhejak.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gqnkxkatq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gqcdflugo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gcmolkmaq.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/geczivgyc.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gmryopgkx.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/guzuezqdl.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gxoyjyoub.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gjenqqnhm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/guaawmreo.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gigqcvdxp.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/ghojffnzl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gredwuvyx.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gqbwcnchg.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gawtzssnx.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/guvgfksdq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbfleao.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gsifzguxy.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gyxlpzybi.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcspylycs.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/goomjtqmu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gfrifcjne.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gurmmykfr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/glbnajomx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gazaxecfo.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvyhcwia.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gxozkpvgu.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/ggdxuxdko.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzewtocx.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gvrgcloub.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gphvpqdyc.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gybahbtlz.sHtML


<!-- 参考信息 -->