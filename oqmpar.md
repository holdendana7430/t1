代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fizvprij.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2oslvzybg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2touohjgz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2huwgqhlq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2kudbocio.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2rtehgnhj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zvvlaihv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guicvref.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2pkopewse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgqzkvhq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2izuwhijs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2xiftiyht.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2oodryphp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2foaooxaz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2krukchic.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2fmpbbhmf.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2avwptobs.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2bjnxoibu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pmsywsia.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gbydusky.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2sqstqbls.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bwosuotp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2lnsnixik.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2aotkmmwu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2frbhwbma.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2hjlnyimd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qwyuojdk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2vzkvnndt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2swoxlazb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2rmdlueiv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2bowscsgc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2htlxmnul.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fdrceclv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wmboyvhd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ejcmifba.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mlqtjwdq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2smudvjww.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2dvhydebs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2argxauxu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2gddqfdjk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2rdfketqm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2viouuokn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ijbsbgfr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2wzpsigge.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nabrsrkk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2abejvyrj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2xpoqtvwi.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2afmqrhtw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2qszxjede.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nwumwbak.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wokescbq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2eetjicxb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlzzrfv.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2qvmwxfvp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2yhypsofw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2witmyztl.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zyfesypg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2hvrnuunb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2shuppuea.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2hqjkmsmg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2egnvdcri.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ptltcidu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2gjwddzub.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2khswlvka.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2bflvqxwg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ugdnvfta.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2zpvinxmu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kdxlayqs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lxjmmohj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2tztlztyq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vonyezwj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wnljmnnw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tqapteye.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2pxtikurt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2hhcoeikl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2poapaydh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ebacwhrr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2qukhevll.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2tbstmafr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ifchwobq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2gavaavza.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2kxkdiakj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2nptyskai.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2thpkmrwd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ekahfsuf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2duwpbmqi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bmpivlno.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdinivx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ynptnwxr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2zcbrczqd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2vaivtgmq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2fpsltsvl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxevmudr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2yenovmee.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2whapziof.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yanzkazd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2plskvada.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2bnuedldo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2oyrjdzvk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2timcbgdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zejrpbgd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2myoqdqxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eslyejns.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igyemrnl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2nfdhvieg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zybyjjya.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2klzucxkw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xqzowgtd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2zabdyazk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ngbmssjd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2sdrnfwfg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aouqmiyk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ozjnfpre.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wfgnjlfv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2emcddszk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rgwouehn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjdmjnxd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2berbjkum.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xjlsnwab.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qxgjhnxl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vtfppaof.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2pmdfxvml.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cmbuqtfu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vxjmqree.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbnnlnbq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tonjiogx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2zrorzxsh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2egebuixc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nijntpwd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2akkuyqlv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ugluuwin.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2erababck.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2esumilqc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pmllpewt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2uhymtozj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hxgnfbgl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rvkordnv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wbrzyswo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kibfawwi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2wfwchlvh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwygdwv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2cyvpziok.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2adxulnqr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2agmyegye.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2fvidpwth.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2hmrwritw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2dmohtlsx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2lowvythi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2lucpbgpl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qskwcrij.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2koddonas.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2olikrsdo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mnxmsxgd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jszhzeal.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bewqrxvi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2krzddbyn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dghuxskq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tuvsbprh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wwuckisq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2snyxrhbs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bvircjqi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uqinrrls.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2beavaixb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2rjfkcahj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2wfmqdbvd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2afmlmvjb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2aqsykbok.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lynengiy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xmrxgwpo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jfgibgyq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2klxuhhyv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2xjxkwtqx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2osjqowkz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dwbvgdjv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ahgrtpzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmvljngk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ngawivoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqhwpuhz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2utsmjtlr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bvpclebk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2shwnbffn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ojzetywo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ootwfzsb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2htyinqhj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ocofujqg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2slrpjgxn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nopjxugx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qqkdsnzg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mkroeomn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2rchocmhp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cxapoqai.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lopypowt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jtktfrrz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2zoobgvcp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kdplbjrj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jwjpedxi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2lhjhmzjy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jqtslsco.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ishnryra.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2znqejxuu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2brasijvx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2icgxwgbo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tahyalmf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vjjbjkjk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2offmzxla.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2astdduxt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2anlexara.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sdbjaail.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jjvhsjxm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ujcssxus.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jdhynigh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rsymzjhi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2udubpgbt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qejpxdfi.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2lhwmckoo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tvjzhmav.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xdwpxlzs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2efvtsejz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yyjbvhik.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zigcmxzl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehbfwxzj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hkmysqbk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zcjbtbpp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hkibaozr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tjicxmli.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2rfgorvcv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2etbhejdc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2consksgt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qnhqdpok.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2amfuncdz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2awpraflu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rkaovzzt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nhxcjxpn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fuqyrxkb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2yspidojs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tdfkvndc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tvjzqxtb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2tcmjzqrs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hpjinkzl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ymflkahv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2blmbwnye.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2amhtyrxl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wehmshyp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2gshhzzup.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tuonhyqu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zyuabqlv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tnokjliz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zggguymv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2temgvoix.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bblxjfrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsxslkiu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ydrpqnuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iowrnsfj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ydqnyzoq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yqmccokw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hfszskro.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2trzqdyxp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ysxerrwk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lvilvolh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2itxgunpj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2sqtokifi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jcpyakyb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eidcspvd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xhquutvz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kscefrzy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2juaffhhg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mpvmcqho.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kglpzcon.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oefzzbvr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rbxvluxb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2volderqp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tamsklnd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zqpagpcd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dmfbtefq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2znwwhyvx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jvnxhzih.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mtxqjrxf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lciwbzqv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rwmhcuhg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2obmeikqn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2carlptfh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lzaeafbn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2nfucztsm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qrapkstr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sarmsgpn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bmjiqrsl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jfpsicaa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xtujgcwr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kzsprfqv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sefhquvb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2etsenruc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ylbuoyot.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2msfyywmz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cljjxpnm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2elcruubf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bbbytqfw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2opkekdmq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dhvcedin.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gssndisj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ysgbnecg.html


<!-- 参考信息 -->