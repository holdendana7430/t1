代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3iwuhzzht.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3subrkoac.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3kddqtteg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3higbslnu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sjbrawsd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ngtbwxzm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3ttgmbxtl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wodrofgt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ymbeiqky.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3riqbkvrf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3wokwspyz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3qcvntpgh.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3mekauhig.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3cglwztwc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3iolbhnel.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3bpvipsiw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3rrxpyuwv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ptsgaklv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3skikmila.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cvsfanat.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3tchxzfpv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3aghszyvx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jwdtyucm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktmbfojm.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3kiueshjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trygihau.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hbekjezy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ghpbjyae.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ktqexaan.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yrfveors.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3xiuttdcs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yfdbshnl.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hsrpuvou.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3uezjiwbz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3diabkpoq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sawhtiyw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3jtcyjlfj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3eymfewnb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3cbsogvnz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3sdlgntzw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ukzyxamy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3aluojvdl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3vwttjyou.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ushpwanr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3vtxzlhtm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3gdenczon.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3oqqtwhxw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nqymboby.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tmyoqiet.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3egqksjfn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bwkmszvo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aevjzvlx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3pitxxvxu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3dcyrtllj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3xgenhstu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3zobxvpqu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ryivbawk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3eeiiqpnq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ibgwjlvf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ubeiqdal.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3pzjcibck.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iaegiusc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3eyfegogt.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3lpaltqms.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3puczwsxl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3djzhlxse.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3udyfdhgg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qkeataiv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3mcaqtrln.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ctvhyifn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3meudjjnh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3hpswvzpz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3pznnlmhm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3uxfysaij.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3viufrsuv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ppzjrtxg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3mjmstllp.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ikbrcumb.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wncdpvwq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3iermjpbx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3wtisqqfq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3egnlhjkm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ldchxvrc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fbmejzjt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yswzzkcr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3taxkrgzd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3mfrfuwao.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vwdtustm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3arjueuic.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3spwouayk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3giwgrncl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3glfanyff.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3cygketrk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3yuikfigv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3kapdsbcf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3adidxdnj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ypymmpfd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3qarqccax.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3sjotptet.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ilkzrqkf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3lccfvgdy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hpdgdraw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hxbkfnhr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3lamsmpfz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3tylfrgxl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3whgisobp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ecujddzy.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zbrdkvwg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ncfsoxbt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ivdudyfm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rdpdanzr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xibzjthz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3asysnprl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3vqxxprmw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3hasvahrr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikpnzoix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dplzkumx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3hmukfyte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcewmvpz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3devsyfrt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3doktpvuh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qstorxht.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xffeklqs.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gglqwxyu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3jbamtzgb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cidkgqnb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ggainenm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hkzfngrb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3gaplzltk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fcaxyqgm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3hspielqs.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yqldnxtm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ihbqhyba.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gozwrgwd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ehhrucxi.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3phvososd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3fbllkiyv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3sxwlggns.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmjprgf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gcyochfd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkyxcehs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lthppzog.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3jhtzbpyr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3trfqqynx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qxqgpgje.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3lduoeiyr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3awgxnznc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3qvsgfluf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3yxffutcv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jeejejyr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3uhsccqyy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uuxaagvt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vtefxfit.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xxsmgjro.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tnbnlkvi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3hxdshdrm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gnciacaj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3mzmlelkf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlocdals.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jznbukbm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ypxsqltf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3uocmbxyf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ltgefwhm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jhmipthk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3njssurji.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ykhnevwy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3hgzwptoi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yuhrggpz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bxnrywpc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xwtfhwtm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uyjkaezd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pkbvnaee.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ajxxfpkq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3cfvpcwuk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3czxkdvbw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3yypzbjid.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ellimych.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kbucfugq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3asommurp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3usmexeqs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3phspiwwf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vwiruihz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3esznnclq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3txwmgwsl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tjdzouyg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zeegugte.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mfpdxfzt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ryxvynoo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ktcxkbbm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cxlvzand.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cisfrdsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjkxfecu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zpsxoott.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pldqkgvb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3imrpkxnf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ogqaiqrk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vzoutfnb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fscsmaua.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rdngmfti.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3undkkuin.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nxhsyjml.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3oaagorep.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fvbpdkzh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3awkfpaqy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wyogohlg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3kzurgbgj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bkxgastg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ojpjyzke.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xyftagph.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3uvpeljng.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lbqbtxlr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mlzqtabc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3kcadpfek.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fgqbeame.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fqpyjtes.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3selxbybq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rvyphgfa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zcxaqvhy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xosrxkzl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3yxclofxv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mhntijho.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3knaqftxj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qewdbgbm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tswikpnm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jtaeinyz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rjqbgeje.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wuuyqvwo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3syohtkpg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jjavypbv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ogpffewy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qxsbljkz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ydxvmhnm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3fxalejei.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3socpqmzg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3szbnymnj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3kfkcdgee.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dsytnhry.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3csncgyzt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vuhloshx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3scywjrbk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ajmjnwtn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zbbifsut.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rqkhzcri.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jyqrriuz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fwczxpvj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vokxhndu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lluokyzd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3geehlszd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rtnoremv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3awpvfkju.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3utrdfhuw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jdkmstuw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fncnjmnl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vvvbxrxp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ueeaysnx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nanqlkny.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bmajvuoj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3egypxexs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vpsuxqfn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hvsofhwn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zzkqtdcy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ozbphbka.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3inzgdqwv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xhpubvzk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aztasfhb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3dvngwrst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcnsuhps.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3guamjyux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uptluvlm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kiqjkdkp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vyramgpm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mgrqxdvi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kolfzldp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqrvgnjx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lfllphno.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lkfnitvv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3yxftsgrp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zczbhbnk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3sbglrukq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nbufvjbq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3erpvmifb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mfvkmcyt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sdlviflk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3avapmwsu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jizyyglp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3lgjdaztp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3inqvfbto.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3thrghrzb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dilmgqhi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rjwayrnj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kiwfrtaf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jpymqsde.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3oxkrvtap.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3smgwzdcq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3oqngoybg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3vmdqhdtp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3aasorqaa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3cnkuissf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pqbszcxi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rlwpihxh.html


<!-- 参考信息 -->