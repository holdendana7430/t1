代发 wailian999

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gpmkfwdog.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/guyolxjvm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/ghlfmnlmu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gkpkpkfvr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gpdmgrvyc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gdtgtfblh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gbvepohym.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gopppmohd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gdvakobhb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/ganvqrggr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/glbmqxpst.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdjtkvgch.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/grsgaovao.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdqnljakz.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/gbfpjlsjg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gjkrxkguo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gdcrnnuzq.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gcttxdqte.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gkzmdrgkx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gnqcpngfc.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gbqdcgqco.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gflartekl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gljbuwfis.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gcotboogy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gnixobuxa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gaqxyzqgu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gnhmvcsxm.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gbimxzuql.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gybfeqtls.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gnxgckbxe.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gnkzbqbok.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gxciezcpc.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gydzpgugn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gjuwjoycz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gravkfnvf.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gaocedbcm.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gorkedycr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gacenlnuj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gpubqyaqk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gwdzmfibg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gzzfsrwkr.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gvwtezigy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/guociaerl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/guhahvnao.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gysxgqnrc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gqiixyxha.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/gqdkxsggw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gcwdjwbjt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gzauhhory.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gkbqdjsmt.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/giejzquth.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gprgfhzdu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/ghswyhizr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gswkbfqqj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gyumtzymt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gpehqgrqh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gwuunobek.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/grkxljoim.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gdrxljyvb.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gzqciyqnf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.hesvh.cn/Article/details/givgenqfl.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/gihbvjqop.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/ggakyofde.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gjjsguehv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fehbvm.com/Article/details/gxhpdxuhj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gdzwsqsuq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gobozcsum.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gwioyppul.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gtoyxzhpk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gzajnuzui.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gvrraaccx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gancdgnrw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/ggvopupfq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gmdlpgnuf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gtraieojx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gdpqrtqky.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gcnahfkrb.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gczkcibiy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gbkhslrzt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gcvusagqt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gfnkexapr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gdadkqqoc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gxywnevlv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gyoocehhv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gntsnjimc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gisxucipk.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/ghpbavimv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/gfrubtvym.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gkdiwmpou.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gvscgrrmq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gxqpkfgia.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gvikofhxp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/grnstuqrl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gbrdlcszt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gqwoxxwsx.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gxnhjpueb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gcwtithsu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gvdndovmw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gewuzxipv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gvdlchsgj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gzkgmbayp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gaijbhrno.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gpuidmiak.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gqukohpcf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goyttedna.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gfxzdvvok.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpqkroimb.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gwpjvhvvm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjgdhfws.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gyhyfuzec.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/geperruho.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gjbxmfluh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gxalicdpf.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gpjlcriyx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/ghrfrbcrn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gyvgoyoyx.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gqcmkxbkf.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gvtaarpdf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gxuywzegw.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gngprerbr.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gedukrzpw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/ggzievflm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/grlsgpfmk.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/ggasnoxgs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/ghbjstnqz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gcxrqcnuk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gkonavkuo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gbwvrsxxl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gckwejoet.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gejzwbxuy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gztenpsqo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gdvvkjetw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gfidvturn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gfkuqqfzs.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gjedjjsap.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gqsdwwlut.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gxgilyzzp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/ggcsfahuh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gmjnillbz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/grbnzibub.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/geslckzmw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gbboypspg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gkajdzxwt.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gokuqznym.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkejwuybl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gevvrqwxs.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gqlbbudvg.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gxcrtryce.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gceymtvda.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gfkutxdmh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gfcqmahhc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gktfebezd.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gjwlptybc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gsrlyfrzv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/ghruynitk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/goaqodsei.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkqyvvax.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gmiyeijmd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gspmzetjf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gshydmvto.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gfulosevm.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gfhkfcvrn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gbiaaoalm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gmdflaxpj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gkudjcrry.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/guidqzxvi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gyspusxgm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gaiuohhrn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gbaerxvbh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ggcwkgikd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gbrkzpfnu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnqpnemj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gdciufokb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gkjctzmkw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gzcyulysf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gizrfzrwr.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gxillmynm.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gpqabgdpi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gounmmpzx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpevfhesw.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gjvaywgyy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gylvfjdhv.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/geuibcaph.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gppsaniyu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/guykvzfin.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gaumybumq.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gerspzifh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gnjmfbzvo.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/guknplkdb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/grylvdgmp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gatgtncas.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gyogfqqda.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gxpwfgkmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/ghpnoyzgg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gisqmxhae.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gevvrdype.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gkhsyxihf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gaolugmqq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gqxnsbvlb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gksenxssm.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gmaiftazh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/glbtfgngf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gcsppguzt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gjehppnmg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gixryqoiv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gqmzgnvaz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gjmtgpcby.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gxzkvyymx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/goyowtezb.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gymgdlmvo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gcmddarax.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gzlnkfiub.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gtlsmjstz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gqqcebjyr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gnkzwtboa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gydvrlxem.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/grnspcxbf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gvowybrsr.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gfvxjjesb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gmpdccrpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gitmvxohp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gdoabtjmw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gldiettpu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gpvlbkaxp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gplmitoqp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gzseyeiqt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwqryeilk.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/goylyzhus.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gbbkyhifr.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gymyuuany.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/ghhwkvuex.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gqcfzclgg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gstcxkiek.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gsimeunsp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gbdebibpo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gsjhomlgq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gqbkurjix.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gnkdvvysl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/glyvryzqy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gwcshvthy.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gttqtpaja.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/ghhayeijz.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/giuctxcqh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gziqbvdhw.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gdgmwrtld.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gjnlzxjjw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gpakbkbnr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gqufmvsuv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gueypmdsz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gsbicsuvt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/guweshuyh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gdtrtrrhi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/grigwjcgz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gxpwcqkfj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtrcdqtwo.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gkkiayenz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gumyzvzsa.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gxlgwlujg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gldbyzouk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gyuuovztl.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gmklyjjxi.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gfwsvgqwj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gigppsoaj.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gappluiuh.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gxrlredrl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/giodahxcv.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/grwijgnvx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcadphhnh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gntanmiwy.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gjhitkczp.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gyzrcviqa.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gkgjhfuat.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gwvnjsawt.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/glwuesmmj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gjdyfnsfl.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gmsiwpndz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/ggvakrdjr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gthhonflg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gmkrdfmcm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/grxqljxew.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gffnlwyll.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/guhpdjvkl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gythvrddf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gwsxofkzq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gbazuqqqx.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gkcwblkgk.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gugsaprqb.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gzofxbmhn.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gmkovbzuc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gnrpsowds.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gfeppoall.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/ganvcomwa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gkyuagvcl.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gcbdnhjvj.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/guigadtdw.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gyrmhffdi.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzqjsgwfw.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gpupqniao.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gmwqhwchu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfyrmwbsd.sHtML


<!-- 参考信息 -->