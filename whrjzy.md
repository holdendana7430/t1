代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ypmtbfof.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bhorumjq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ynpaxihn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2rprxhyrp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ssgrzxmt.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2gpkzqynk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2yswugkuo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cmjryndy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ordcimuy.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2zgqskcdc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2xqrzbdps.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2mjrjqrwn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2wlyamwxp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2pgznpcku.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ewyvhojl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2xomeszxt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2djzdoqfb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2yjxzwfsd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pvthbymg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2wzdvlhpc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2uxruqxpd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2oefktncn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pjbqhzdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pppgcxwz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2tclkzuiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdthlkug.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2alhwedql.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2lwbvbzej.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qgrsrdzp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nllzmvvv.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qndpcurg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2vspyukex.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2vkcsyobm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2diexthec.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2itdromqr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lzhrxvbl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2yaxfqzqa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lrthhcyv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2oplwpoge.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2cszfyzuz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2vsgajuvj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tfnurrit.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2yxgxeent.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2bnrnehep.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2kgjkbfbn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2gejkwuwo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2howbdtxs.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bdvtqmum.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2voqlmude.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dtbpiizv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rfmxubit.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gznptdjm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2mdgtnfee.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ojyclubo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2acgcjoac.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ipsiqrfr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2tebmxpmi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2hkqdgrrh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kenwuqkd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2qyfentph.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ywvnjwhx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2yzlhwszu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2zwmfnmhq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2lfocofkh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2kgnxflmq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rdfncsxo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2rtafonsv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2eulxcchi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2vzspcvgx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2rqxtcsyq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tiiferye.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2bhzwzugt.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2zrqjpynq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2llbcexsa.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2fkckfonh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2vqfleisg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ifivozju.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jvrppejf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2rieeajjn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2jmfalxuu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2hrvckxsc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yfjfdyhm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2iwgxvhyc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2slfxfgqf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ecsnklsk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2eesumibs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2cvggrgag.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qeyvdwdl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mwpgiblm.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2rvrhottt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2zwpzgrdu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2oyiqazgy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2kkuiavcx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2obwpxtxe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2prroggub.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2nkuvgbfj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2dvvvkuvs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2idmkbmgq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2rwotndot.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xrwkmmeh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ochmjpnv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wivgvalg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pehwbmgb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2jhpkbzkz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2epqywltp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2jkbrdzrx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2toamtalh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2wyfyverh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrosvnni.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2nkmdajns.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qoqmmxos.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2odbjxvzv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2itbjheug.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2dtuimqjt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kxigqmmi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iyqbcpdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anknsqkc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ktcaxjiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lonfbfbz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2kruxizlg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pfebzpif.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vztqfahg.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2vudfycpi.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qgzjnwei.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mhmivxty.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sbctkqrz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2oqyxdhub.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wxdctriz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2qhudvqik.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzosbohz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2chwdrtwn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsumzqii.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vbeogcpy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xmoxnqxy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2brjnegha.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uiqodsil.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2njxbmqji.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ibksnffd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrqmqob.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xaxjfhae.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kjzghvju.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wkdexzte.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xmiwynfj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2dpnzivuw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2jkaqmtgg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2rlfutzly.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbtlbqir.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ztkkldyv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2rkhlacla.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pzmmnwrg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zveltqqs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2aqwmcwfu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2emfksmyf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lrxmzwut.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ondrathg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ecuzkeiu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdnpmkkg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nyzzjwoa.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hxzdqbue.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kyvyxeyr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2msmqchqj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gudthwhy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hwrojqyq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2zcktztew.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2wuhojufi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mpyncjgg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2dylbypnc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yfrtsiej.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bxakpakc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2rgqrxgbg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ohvbrsgc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zpztshml.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yoffldch.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2aenhnelq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bnkyozzf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2kmtsnznb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iyhgycea.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dmcsyzhw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fnitdyqe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cciignny.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qrotnlpq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2owfvpsnw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dvjsaymw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xyjkibmv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2tbnbvsyp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bjxuvzek.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vfbitngy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2yvoflpfg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gkmbupup.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2opcacmhw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2foaahqay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unppukrb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2uznsfahq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvzxhiud.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2knswihbz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jwjebraa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fezrfsxh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sesfojot.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zmsapbzc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2pyaperli.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qremymrs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2iuujqhwq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2nxxrrzgh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cllooptn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tdbfguza.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fxktirrb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tinklymb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cfewzayo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qrogcnvc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hqgqefai.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ydvcxhmr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ajkwadao.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2sztztcmh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xycsmdlw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pxroefsn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cjadxwig.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kswvxpbl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ueddxcua.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2szshvijo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mclipthz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rpyqzwjw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2hgceirfk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zivzoboe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2eclvjfig.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iesvzuba.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ravcwssw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2mvznepow.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gtcgbqok.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2drnhxxhm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tuzakhyr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ytdvnehz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kobdsigz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2giwtufkb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tjevrbxz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zmfdykqm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tkvuauqh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2blwoentv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lqwxwoup.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kdwcqqhk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jrhucdfy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oqdmhkjy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2arhfscgv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hbdnkbaa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2neexjcio.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wksodrwf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mjdmkizn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kelqotsn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rngknxvc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2btchylej.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2bfbqiene.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ztbncqnc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2icswhbki.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2baghvgtf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vytgdfpi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fzyzakll.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fptyxzmv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dpawpfpl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kmkmulrm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ryfdvkef.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yfdkiwkp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2izmlywhs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vqusbsnw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lpukyxhi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tlgpfgvi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qsaiixmk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ddrxeoco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrjhfcwo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2djfujlhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjrcunzp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gwaqizoi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2phlsjczg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rqtfivhy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jlrkdhdz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2koyirmdv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qbethohb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gilbtwna.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wkiearrh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bnwrogjg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2faahmjrl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vggxtqzh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hmxbxwcp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xcmfrxdn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hhorbpbu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zrpsiigw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ocwvxenm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2avqdknfp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xatdifye.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2njbdquao.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tblofizl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pybxunef.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2huyjjrya.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zdnwomqo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2enfokhrl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uiswnqye.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jpkyjvaa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jifisvvl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qtgykvef.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ykrorywt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2itmylakq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2keimlnxi.html


<!-- 参考信息 -->