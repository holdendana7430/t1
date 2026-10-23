代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3weboleop.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3kqkvlqvt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ccbupngs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3odzzaomh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3vpjktiby.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3obfcnyjm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vnyiwcfh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qhswaqfs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3kayswpit.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3szmtuhdq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3xcqnxeyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prkmuixr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3cthavojy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cswwuslk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hhbmwkdo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3kgakxqss.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3dplqnxry.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3awtwdmfi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3htghoznj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vpobjozq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3awgfdmau.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3xddkpfao.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3kwpqghku.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jsvfywpa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wrxbekfo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gyzbjrjo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3woloivbp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3vqlogavb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3yywfrpki.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3dmvvzrqn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3nypvwzll.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3gziszktn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ztisiuyb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3yveicdpr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3hyplqsav.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lvzbivyj.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cvitnhib.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xznyjues.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mtvjbkwo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uhfxtrno.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3rhzhqxzg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3jgqhtluf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mlypdhfw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3vlgdnhxu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3koicahbd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3sqdnqgpu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fcbhkakw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ejsrrbrx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xovxgjpl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3srklxpdt.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ibppcybu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3makhsxcd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ncnbzjql.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ihatddjk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qdhoktwj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3jiiutdrv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3liuztjrq.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hdtekccy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dmtoywdp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3duekwcom.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dzlpqdgx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3eyjpbiwf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3weugvzxz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3cbyusrmw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3eivudjav.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3avqzbwzb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3arlmctjv.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3sbzkpqii.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3cycgdafd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3crxpcrml.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zdwrmnlv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wlykiuqm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3afnxmqtj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3iomutzxm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpxqpvpe.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ssblwlxg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3doozxaos.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3mkbqasfi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3tumufjgp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3byskyjnn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3hmwlkfzn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3dtdaggaf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3tcwareje.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3njihoefo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3apkpgbmb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3xxawqyou.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3jkquoljx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3dhkgutuq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3xhmgxdai.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3nukrfurh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wnrvxgtn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3lfkmulcv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3mgilmjcl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3mprkjeuz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3fwsrhtlo.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3nvmajkah.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wynpcjyy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3goqcpjgm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyjtugjd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mmoxfdjq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmrwdtxm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3veropxeo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3sywvixkw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pusovpqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkvdyzvg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3mbnrfbpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyxgbhmj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdxbaips.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3djplpgvd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3njdfciqe.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzykaunu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vfzzvcha.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3wkoqzamg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3tiszlgpk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3cdsfchbf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3tkzjvdgt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3dvznodau.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3pswewabt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3cqjtvyvz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tkkdphti.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mczmemuo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mienepuy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jzyquxti.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnanmrcg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmnieiu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3tdtfnzdd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3sniiwsdt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jvmnsoon.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kbokhgmm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvmtomjy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lewyuaih.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wvbvbtty.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3guegkynp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3wswnhrog.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3mglmnfal.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pzwafzex.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xfukagyg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lgenmqvs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3okunsrgc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ybtardgm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vgccxrry.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mzbngpeu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xjjujbzq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hsvcmdpw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3csaztyio.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3wzgahzwi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qfwhxnkl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3glhcdoyf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ggiatyyx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3skipmbhb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ufgmzlpu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3tizfbiws.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ctulmrdk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fhfvorwn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3jkwfgdej.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fhonshce.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3btpdomca.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mfgfjffi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wbpgeail.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cpnomfmx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ewozyxaj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vcvlzneh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eluwcnxe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3owoaomef.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lindlaej.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzvtnmj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zlbjtqmm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3btjpuvcy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3yyvymzfg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fxogskpn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3cccuyxcy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bsiryqis.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ipxgankc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qutadfbd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3arjcvvwt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3patbgizw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qpreztac.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3adzpzzlb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zmubccxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sypxelbj.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vnhivuwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ramjtsez.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3avjguvfh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3faljtage.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vlzdaeyg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mvggocff.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wmnujnrw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3cdnstsfx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gdjoumrh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3urxrbxxy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3knunqkmy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3htnroulu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xisjqmor.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3artobtaq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qrzegloy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3srhgytmu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lazdolgz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ukgnxtvi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3weomgnox.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3sprxbmjs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3lyjlucjx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wvumvmai.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3kohqbbxm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vopdhcqz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nhmzozat.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3abtyjlbh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3prmgccep.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3wzwrncxu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3btchsbki.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nqgrjxwl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jsiblddp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fizsumfv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zflvhnys.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nvbuboyw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3oannvcaj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fyhckehf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vmejisur.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3uuexyvdr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3lefcotil.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tbeokpvg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3edfirayp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lpmvelnl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dvtgfewy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3bykgbkaf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3muixxqay.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ycjxhajy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nkixiyiy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ammdrrhw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aobxeaoy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3apkslhay.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lqqgnnyl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rquhdahz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3auwemscx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3cfaalthe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxtwtps.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ehpnuach.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3awugrlsw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qvhregnb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3udmqrilt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mmqdbpfd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bttsuoge.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ovirvwaz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uwmytenu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qgljjqer.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ubzhqaea.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3dobdsyft.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vructgit.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fpilcnel.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oakkfhwa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jpcbqvkw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ghgavuuc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3szwmyews.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vcjxenqp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gpbgbfgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cegddjct.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ipjvxzqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3moynnubn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bfdqmqsd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xwchryis.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xewdwsww.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jlrjskbp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvnokmla.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ijgwruze.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ssnykruq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wuxekmem.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kbmcpmum.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fmsxxlao.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ulaiewnr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3hcpixdyu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ufelvuzo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3syzurrph.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3izolrbhi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bjempvjm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3oanvfusj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mygqbvyt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3btoyzzwg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ienxmkja.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lbwrftxv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eqncjlin.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vxnaufgi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3gpgshaks.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kbospjct.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xrpvoiqi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xkyyxrpl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fqblqmje.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qmaquenn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mtbvtyou.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cgyxvnmj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3voklmowf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3azybjlsx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tmxviogg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gdpqsctu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vtwyolry.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3gjyjctya.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqdcaxgz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ottpvfeq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3filpkjfn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skztaeqx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vaujnfxn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xecterlz.html


<!-- 参考信息 -->