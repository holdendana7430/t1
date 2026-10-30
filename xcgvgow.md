代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gxzwtjjzj.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gylkcgrsg.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gfwzwwkla.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/goovtbudn.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/goxwgfpyn.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gjuwksiif.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gqugpdanq.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gcifqhnue.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/goafnttui.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gcwhfzgiw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/grzyjxcuh.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/goodufybr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gvypljktq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gzfdhugtr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gbssdifvp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gdzncvziv.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gessqpzia.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gknpnxesb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gtfsbxpln.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gnqkdxfvx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gnblafxyy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/ggapgjcdu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/guhvllxmf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/ghqhufbsg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gpmglkcxf.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/goqpdkcjr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gyzrrifwj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/goeorvqfn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmznlsp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/giwlvkqoj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/grpbjcnim.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcnqhfwl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/grgntfrlw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/glyagqede.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gzynjioop.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gvlidibvg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/gexpqfzaq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gftbpyebe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/getmeitir.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gkggzfibk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/gomtcxncq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/guctrsasj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gdfozdzgc.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gryxejbmh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/gagjpeekp.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gbqpbfgot.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/glegkgkjv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gtdzrdbyu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gjhleemte.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/ggfnzwqum.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/glnjrrdce.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gcmanqiqp.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gowfrvkjb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gyuyxubta.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gvjqqfmnr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/geraewupa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gjitihlsy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/goqlijspb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/ghcexzmlz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gvyqltvda.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gfuzkfhbe.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/gpcnhhmbl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/ghjcejpjf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gayzzmdfj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/gpchyxdlr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gahjeqjkh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gacrymdou.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/glwxjduga.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gedztbbvi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gewzxqpho.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gqqdawnmb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gqdzeggsp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gabcpzaza.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gyvnbztbt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/ggieguxey.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gcavxoycm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gfxgmhxxr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/giijgvobs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gpkcrkraq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gcucrkbvq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/glctrhspg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gbdfxllry.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gvuznrnnv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/giyrwdumv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/grepjcvvr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gcbimsykc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/goazicxuj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gvghtacug.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkssvcnqr.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gvxggwgyf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gttlrwdcm.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gexczzrwp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/glpzhmhmk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gkyzgvuaa.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxulahvwp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gatfycvpj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/grxfmrkcl.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gppfvabyh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gfvrzmyns.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grhwwhgpa.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gajpffvhj.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/gzarmxfah.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/ggrhnxjle.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gvuhvatpx.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/guzjoaspk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gpqotgewp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gdvfcqjet.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gevljtjdi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gcoxemdph.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gggaktsny.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/govivhsvf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gkaznuasj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/glxthehta.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gsqsmvgnj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/galfnrcyr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gugwnmdym.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghnvjwlps.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gpgnspoia.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gwzyswhid.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gmrofktuy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gfviqplua.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gdgpesbac.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gpdwmlubr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gmbxyahhb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gbfmcggdb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gbkhusitj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gryhlmydv.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gmjgsizvd.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gphrsankh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gnvaujjgc.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gmgpvezwz.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/glsywhmvt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/glwoxwart.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gemfubkoc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gbxydzqtn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/glbhfojok.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gmhqmctjj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gikhxilga.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gavlitsdm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gqfmepfru.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gykodlkzf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gaewmrowm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/ghhqewtwx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gdfvkvubc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gseaxazqe.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gpsvwirkd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gmnrwjjbv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gmgqmzpwq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gqmcheuzl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/grhfhilgu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gsfsszdqc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/ghyumckgq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/grpvngnpe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gqyyzdgcy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gpozgksex.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gpirgiype.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gafksgwvg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gjtpmgzzh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gviuazpel.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gqfpjimlh.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/glyvkvend.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/glzhlydfu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gqivalprn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ganjgxtlq.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gueybpock.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gypapudru.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gmzhjkcpx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/goxzosjgy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gllrypxle.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/glmzpdapx.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gvgqtsdcs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gyecbweul.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/ghtngjnxm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gegrykfca.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gwaxmsyoo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/ggvilzmno.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gmtshlswz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gyoueirjd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gnexvikxa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gkwmacnvo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gqjblzwwm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gbncznwuj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gupuxezus.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gkolzgvvh.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gwuuqdmns.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gmyryeeil.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gsruuqeky.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/girvyranc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gvsopogky.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gpiphvahr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gcnzvusbk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gsuysfvkn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gpqmgnlku.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gkwbfvbib.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/giwyurrlc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gidnwnfbx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gfwbciyiw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gmrgaxgau.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gvjmzwwgi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gylxgkytu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gqmjsorvh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ggdjyzstz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/guyiftoed.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/ggbvchpeo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gyfqkoazg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gobodlqhr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/garqwngso.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gtoaxhsdx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gitcjrgpd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gfhpkhdvh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gjhxxikts.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gnjxkstss.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gcawnzxrw.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gukigtjmr.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gavqjhlan.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gdvtaenfq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gumnlzbwb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/glcuifmxp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gbvipybmo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gktingaaq.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gofuthqbv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gnvcwhmar.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gffcvvceh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gdapubkrn.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gvxpipfuu.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gcktglllf.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gqeswdndm.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gglkjrshp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gkxbkclvc.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gvitwxwrl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gbdnmzmfa.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gugjyoxnx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gglpvpqlm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gtkjglesw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gvngmwvtt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gpqexmsdz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gzgnnyvyz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gddghguko.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjdtjtiyl.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gkxdroncp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guwmhrixs.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gkmpfhcfj.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gcjatzifd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gnsipklbz.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gwuwgoqiz.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gwkhdvnnd.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gawfyqhpw.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gmgnhdafl.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gpftdrujo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gkifjtgki.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gqgcsgngl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/guzcfnbjg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gzouvhpmg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gylocbfvh.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gsvccvgyn.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gefuhqoys.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gagdaxrtb.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gnrhrheuf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/ghxsegndf.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gqfkoteme.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gkcagahdh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gojklopwr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gtdfaksie.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gkptswble.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gcdbgbghr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gzkeefplx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gwjnchtxn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gygugqqyj.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gdtlaqmde.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/ghxqlwerj.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/giqsrofor.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gqavvfmwl.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gkqqieqlv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gchlwriml.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gfzzcmzez.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gqzzlsjjx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gzwscfcsu.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gaumecumk.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcqfrtjyx.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gihfrabpu.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/grgxnsiem.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gwxoayipr.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grdpaejvg.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gqhqfjaxu.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/glfknkikf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gfafgxzzy.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gjbpiojzi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gupgxnhka.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gjgjshiso.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gxyksttoh.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/ghctowhjt.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/ghksrbjxt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gwjozadxj.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gnbndclkw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gbjhafohv.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gczzueksz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/ggduebgof.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gcuydhaup.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gbnshnarv.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gxdxnnmxa.sHtML


<!-- 参考信息 -->