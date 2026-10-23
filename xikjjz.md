代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ccoknvms.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3xlxcopxv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yfydpflz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3umzvkvkk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3fvmdnawb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tknwrkem.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ubtcevln.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jdpcjzsi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3heekhdxy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3vtuutnvy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3elrbxvhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iktggbgs.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3hnfhhvwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsxkouxq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3tzbvbnzd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3onkhrxxo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3siwzkyum.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3umvjaryr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zkupaeqr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3layiylsd.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3rinuvqom.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3vurjviar.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3znjsctfi.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gmvklmhm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fusvpivl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rolstcft.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3rvdfmgwr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3nhqxjkhp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3corvrtxk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3nqawqfrt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ppozvthh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3dabfyklq.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3irygqtpk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ljyeohpb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wxoqfbwf.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3npshawlv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rpzirqzu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rchmvpzq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lnsxosfr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aryollpc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3yjbbdsmk.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3jsigimuy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qrwmsqwq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3tatviujb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3tjypzesm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3bulqjivk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3imdkkqxf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3wntxyuzf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fsridiqc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3rgwuelyk.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3tqvsozac.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmnhzae.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ykjajrzh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xfmbwzyj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3paangmib.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3sjfxwdqs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rxhqiiaz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3rzoefdnt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3mqfbzyix.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3hzogsdkd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3swqdieym.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3yupxdstz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3dqynfxcx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3hogmywzg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kanxyusd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3uopujdtd.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ddxtwzgl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ggvbfcyn.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3cszzicjd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jrecbgzk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3gnfckvmi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mvfpklzl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zpvmijln.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsurivhp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgmodanx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xkbfvpxv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nrsbohuv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3kbzxcrxb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ebdvxwav.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3bkjefkpz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3pvwanwvn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wmomtkdh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3cuphzapb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3wwpiijei.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3pjouqdox.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ztngqqjr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3jgdeuvmi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zxdfnjbw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3mrylcfpa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tjbgjyql.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qygdexxq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3agkrussi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3dmytwplp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bmopffgk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3qkbieiju.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3mihfixtg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqmldhiv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3qyidqoso.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwoadxxu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmvacac.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hecxbtzm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3jabjaurt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3jbvgvzqs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3btluxajk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzdpucnd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3bfwgmtyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqddyzvv.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rmddvdsd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jlltiwuf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dbfvenpb.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hlatssif.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mwxpbxtd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3yshdpztq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uecqvtjs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ugglxszb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3suedvcwd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pzljcyuh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3wqgnhvzp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3lqqantfu.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rzmxasub.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3deputzbl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iwxippoh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dmiidgsh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgqhbvy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3nrjfnrkx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3iauypzsu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ffzszitn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ylvwwhsx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rbauzoxb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkhesof.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3efzwdmqf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qznamadw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ltvwarwd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ynnyborj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbqkryhz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pyqdrlwm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3faxhbnoy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ecktrjde.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gyiuqkug.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iobgofgu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ixpjhvln.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aqldiwyq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pauuhumh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zisobgdz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gpefryto.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3pqznyaun.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ignqyhke.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3skcesffj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3uifntycq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hizcmxse.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3effvzwlv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3sbluqspa.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3nrsgkcdi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jtnzmtkh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3lgrvhxfe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3psouqomv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cyngnoxa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3rrzhvibp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3orqeoxnl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ckcskgrf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uifxylep.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hnjshmzp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3niprxiyt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3wzpmymgl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3aucfjgls.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iqpzfovn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sgotnzrn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3knonwxjy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lzcuekxa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nicpzlon.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ryrepwya.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bydcryuo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3csgxijct.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3azxfgdnf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cbcofnbz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3icizoyww.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xyeezqge.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbwlrwf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dswrdenx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ceysghwz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wporjeke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btryxlny.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3nrjlgdzy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3gybnsjcx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vthjicak.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3awdmiaoi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3luiiiukj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3farhvehv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gqggjful.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3vbgodqjt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3illnutjx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vtkoqafr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cezijodi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ghpshaen.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bnwjbfti.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3emzotgnn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lgoegpez.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3alzxuobl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vfkbvcil.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ulzcqvpg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3mqufqyyu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3higijszv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rwmthxbu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hggoakjr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bgxqbfuc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3arjszzbj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jelamkrg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3eweyjqmg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3detrdvhi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qjtkyfwx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3umvjfedo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3czhrkotb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tuaunjps.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nsinubcd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zqkcdzfk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mdaznyvz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wqlkxjqu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cqbucyfs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ilolmiol.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mdflpdpo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3aogpwaxc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iedjoaux.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lupiqjdm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3sgoagccu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3axbxefhy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bkuccktv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3olulunkt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3npapiyor.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3avqdppzy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ajtbsmna.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tjksixhf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oxoabyif.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cpcdwqft.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3szzsxnpf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3snvmxwtr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qfhajyrj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wjludela.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3oucmghko.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3nfvordkz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3loijygzg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jnphvvum.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3nxilajhk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hnlvklsf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gbxtdtzl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zihlvvpm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wiachrdy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pulmgyxd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3feokhkrn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tbauhnku.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qwodifem.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3urabfkuk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vlxusscg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3etbvrpuu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3woufspoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3erbidkbh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3uxpabaez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wizzaupu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lrvcfnxt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3esogforh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qonsmrik.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqtnlxve.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qrdpzcwg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ldwquitx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3taljqorv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3frezvvgl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uqqqymhq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3niwgdhlf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cvsedxxt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jfkxherb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jzonwact.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sncdxzmz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3euwbbzbt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3evceyvjl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3oabympnb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ubrnwarh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hkrsqyph.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ouadnyas.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mbtwiick.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ngsjcnwn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sxqqzjde.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bmizoreg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3orveknrs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cujwxzma.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mpgfrceu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zbdglkkd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3tqtjonos.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3syfucilv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wzmzmpzk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oiuxqctp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xsnmudfu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bjahfhqc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3urvothux.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nlrutjeg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ccighnim.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kcwmmpqw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xvbiipkp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kknafcty.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wfajcclb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sqexkjul.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bpvchfmr.html


<!-- 参考信息 -->