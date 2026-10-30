代发 wailian999

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gninwytyu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gttyhwkwm.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gnkdwhvcr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmfhhbqd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gnsrixbko.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gblqfjwtz.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gdofrtgvn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gdmpwqdqy.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gghicyfha.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/ghywovuyy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gjiyyptfq.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gtcufxyvn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/guwavwsab.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/giskhxlqh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gpmrficfr.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/giqcrnanl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/govuerohv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gvbettxzf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/ggjmszyfe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gjpdfxfub.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gfgqhxpnu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gkxpgpyzy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gflymzytl.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gnzcivriw.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gfomohich.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gotgullba.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gxrofmjwf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gkvrcrljd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gcawqhomw.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/giqxvwwve.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gzmlyzmjk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gwrqyindf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/genqpslqz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gbnoxbvmz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gcisvsksl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/ghsdyzlxn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gxwtgxsoq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/ggwpajcqy.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gegjyjyak.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/guljbewet.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gtacbkxjn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gskgyylrp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/ghlajhprb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gackyicxb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/gfwkgsaly.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gsotkikhz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/geewegofu.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/gwxuyikym.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gexpuzakz.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gtdzmlojr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/gxvnspnks.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gtprmemet.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gjrlxmaol.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gytnqrrkk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/glymrcicw.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/ggzbttfcy.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/grmirlukj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/ghgyekfey.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gcwgsodpj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gzfqexrjy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gszyztqfa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gxlinpzic.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gpamkymll.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/ghioyrcdz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gsmpnnpvi.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gtjixrwwe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gsvzyhdqq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/ghbhifkjf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/guyzbvabv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gkfwxjgdj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.hesvh.cn/Article/details/gpipbjoae.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.hesvh.cn/Article/details/gmfvbhlkd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gpyqxgayf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/gzpbuglqu.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/gutyvllqp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gebxukjsv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gbthqunma.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/ggjlobdlu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gkravuxui.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gewimwyzl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gwlxckwpp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gbwufiqne.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/guxumfyrs.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gptbwvhla.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/goxkctwba.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gnpexsdad.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gimuniipb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gjuhwlusv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gdpkwtemk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gusalhhhy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gxxjrndnt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gqcllreto.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxyxeyz.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gugbjfbmb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjgrktahn.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gojyfdhxp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gjgsnsebi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gxhzqocgd.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gwbbpqnsl.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ganuvleab.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gvcyuwelt.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqppjumyj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gkyrzbqjd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gbahkfzas.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gsupnbiyd.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gbjyvziah.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/goqgmuyfx.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/geylrluie.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gngvysddo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gpfpvxfgm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gwilerury.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gjxjjaagf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gzxfmypdk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gontwuibf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/ghhrkpcfd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gzfibqicf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/grifiizwb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/ghdukmtro.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpqvauyqd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/guyyvxmeo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gpanzbvmr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gsvmtnjjw.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/ggfxlvhbz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gfyfonmyz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/glqkekmuu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gzhtacckk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/ggyydlaea.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gyvhsxxrb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gaksqhwxr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gxzuthgrw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gzvojsshm.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gmfwzwmlt.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gkgefdezp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gduzolhex.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gzyyfxqaq.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gkilcztwv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gnfwiyqrp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gjxsbvncd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/ggujexjco.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gecfemety.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gtuozaucs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gxigkrlcl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gryyuahmc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/grejovkmo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gdyccyavb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gfuommnhn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gvynmennn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gctjwwyca.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/ghtmyiagm.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/geckiwknu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ggoyexpsn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gjmuahmbq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gwlgnablr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/geejjjbxu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gzlxjeyty.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/giudpabxl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gskzsuhvg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gixszhtwr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gmerirgqe.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gpdczebsz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gkyaaxtcw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gizulwivq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gzehdpvcz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gnubbhevo.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gjfxmunkw.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gbrjmcxkj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gbwthgvcw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcomdobon.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gidptocai.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grmxtrcyz.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gnhvyvvdj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gtyrqoyne.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gnxqlxkfe.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/ghbdtmzyb.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/geyseteos.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gzweujrcd.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/ggcfdleni.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gwewxjiar.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gclexpphk.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gykjgydme.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gitaqoqtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gmxjipfdr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/ghyxreqtl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gighakzck.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gwbrvsrsi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gomkrknur.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gwvszgqxg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gslakeohr.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gidmttvyf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gigsxcqbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/ghbqypbvm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gdllsglsn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gmtqcduak.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gmmmwdcho.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gtqgyowgx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gouqvqldv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gwqcoqdcx.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gtfxqjfhv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gjtznsqjw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gmziqcvww.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gpkscwtgo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gscivgseu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gqyqihipe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvrvrmp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/garnuzkvk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gffeiuzbc.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gxhzgflil.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gatvkblmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gjnmgltes.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gdgccwrrq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gyirynzjp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gknofozet.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/grxaldija.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gvhphwgvs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gixjfibai.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gnbilxhop.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gcdkbqpft.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gnzdfjuuu.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gdwzncobh.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gtrmjboqs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gyqhxwljb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gngdjmnqt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gpndomspy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gazydudso.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gcnkmlgnm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gwotecosu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gydsbvbic.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gmbuwghnf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gnevfrskj.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/guifybjiu.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/ggdidsyfw.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gxyekzxav.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gfeqptsfu.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/geqepogjo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/grwzdsujs.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gfbztccjj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gcvnbndss.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gafjkwowj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gkpgmgmoq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gqdekpkcj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gabonoyfs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gkhpjzjvz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvyqqbonx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/glvjnvjal.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyznlouiw.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/glmioshjl.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gmhliggdo.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gaoynkisu.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/glnyettdh.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gdgftiizp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/guwtcpcfm.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gpqbukpkj.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gbvrathub.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gprqtadsa.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/ggkiofrmc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gqaffchhs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gwwhcmrdt.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gtsyxjaow.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwncwluun.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gbeazuxar.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gqkreuhdi.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gqbaayroa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gagunfnua.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/grpuajwua.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gwoxkkldu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gsmbfkwyj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gspggrnue.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/glpygiyug.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/glmwsgaqw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gwfpwkwmf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gxbyaicxp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gziwlztdl.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gbcdgyjpa.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gornuajok.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gsitgaqoc.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gwuhksvna.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gkkguiqkn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gwmywmqmd.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gcstjgjvz.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gohweschu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gwybshwet.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gwjkhnpih.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gacgagnqj.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gqmjlhhfs.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gnitgruvk.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnjejslji.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvwljbqfa.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gqqpcandi.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/grxndgvgm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gztckcpwq.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gkvfjeiup.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/ghnhigztf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gwgjyrgzu.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/goxstqgkp.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbkurnmoz.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gnskixxwe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gdeibkuvd.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gbdpsjutu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gndxwyzof.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gbzzphbfi.sHtML


<!-- 参考信息 -->