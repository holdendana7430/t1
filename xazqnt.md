代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3xhwlvlnn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3zzdfaouv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3nyxmkzpp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3xgpzmszv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcppbeg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3dikqgpwq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3xxeodgaf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3yvdievzd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3kbjjpgar.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dhtuexkx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3oxlyomvy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3rcmlkodt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3wqolghoo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3kvtzfvne.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3xztrvkbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvdurmip.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3tspnehgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdnvbslt.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3hvdxwhte.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3pniayspd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nzmhcins.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tvieziyf.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ocdzhzqd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3mebohmgz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3tzryhdrc.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3rhmflhct.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3huwpmdbg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dhuklmnh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3iwsuimsz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3sibehout.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3vxuznoix.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3jmixigis.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dhbbnrih.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3euywxmun.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3nvhssnpi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3lbjvmxwv.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3gkecuqaa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3chippyzm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3njffuudv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cnyzjwnl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vylsmmoa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wptedqgk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ipumrkop.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hlmosdtx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3cjlmcuuq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3cjbqyyua.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rzknxnac.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ljmcdsbv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3kdxkqlor.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3fxlglpui.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3csnpjrhh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3bdimysew.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3zuspclmt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ifjpfbri.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3inxzgxzw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3sopeayfk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3cnnxlyuj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3uyunkrjy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3znfxpvyt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3lcmafiqa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rjvhukgn.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3rzfaerkp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jknhsvvz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3qmxwrcvi.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tllwejjn.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3gnjxsdlu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ailztirn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3jkvrbkto.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3jvyejjzh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3mpiiwsdm.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3fpppsljn.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3zzqtigqp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3qsqumqvk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3yoeaqccv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3pooxuggm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hwnjtkdh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xvybtcvw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkofklbi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3xrnfilqo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rttcaftl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3edtxmamu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3evtzjdoc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3emkcdohr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3rmnrmeci.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3emxkaxmt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3dzyugipq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3fijwbvnp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3dhajdrrk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3spqjtoqj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3eahghunz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3bgosbpaw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3dhplrcdv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ujbdcjjh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bicosphc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3lymbkeku.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ytxmkokz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3qnkwwixz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3qgsewstm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3gkzfdtxo.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3rqlspuss.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3idqyhbul.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3cuodlpnw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3dduuemeo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cwskabzs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3rlgjiigv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3xvuffdjs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xbacuznx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcwzqjbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgvupyxp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3cttlcbzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cucugowc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vsahhwmk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gblrhsjq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lfmqmbzp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3uulfopcu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cqrxcxed.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3guugotrc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3fmhycegm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3oibhiwoc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3phnqjusw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3kltmzbbm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3azzflssh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3nhqnfowv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tejnlvhu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qeigrmjk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxyumqg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3fdevfcol.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dofnrasc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3tpznjrwy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rsgfeckx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hdjvvyfu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fihklqzv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztabpkhm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvoiczpo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vmioladv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3mzflmdtt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zxfgbqof.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3exvbrabi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ttjjtztr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3waxnplvr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3dccytycx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mdhumcbo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wtsvbxws.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dncntlmz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nnhntkfg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xpfjpsib.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3oqtvdnhx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3udzbnjms.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqmoibux.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3kqqysyes.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ljropbty.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uhnwjbgm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3mgqsaory.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3piodbwfw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3awaciorp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3gpfbocjz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xszmkycd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3aveubgdb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ayemipxx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3urcvmpot.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3evsnucsf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3plavcpkm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qqvvgsti.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qcmrmukh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bcvbzndx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3uhbutsxx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ljvyzbmh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3zmnvdily.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xzchvunt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3senypxxo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3osszxrrf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3awfhdybo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kvoqzyzt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uikmuhln.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ikgbwzim.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pyfekrkk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3istepxhe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rrvdgwpe.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zlztmxdp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qgdtlmji.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3oxlfqthd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3qnifgnfw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gksoxevu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgbkgbfw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3rvwwdnpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxmwrhvj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3lygpsdoo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3lcvrrosm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nrwzfuti.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3edvejquf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fkquztdm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3otvueogq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qvoqyclu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3owbjkqjr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mjxqrvzc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uvbvimwu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yvnbhoqh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fkhyqora.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tnszolbp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pufhmewd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nlcixfhp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3raggdghg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vizqpily.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3xbdwugop.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yujrtwoh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hpvzmkja.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qcxsozsn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ozbxsqzv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3aelhpsvh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3veevcaxk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pmmajwmd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rischykz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pzuppytp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3sdymcbaa.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zdudewbv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cuqkiyjm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fhdihopk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yvsxuujb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ygejyhwd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3exkamjhb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3rrjtmpof.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dubhbfsj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3mwpcwmel.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3psbixcgs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hcskeklc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qszlpjmf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pjtmmfqu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3otxusajb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3wctsxcja.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3lgcrdvmp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ygakpqxw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3fmjtesax.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3grkjvebr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3uycbfhdf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ifopetkw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3acqcgmqa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fwresvmm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rzymmtrd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3oxbvpnkf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3oargeqbz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3emrqwybe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3etqvxony.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mqyrhpay.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tvgiyybt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wzkaenzg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3sqgapirh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3goylslzt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3krqmsiiq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ijhfsgqb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ttaohjxk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3pexvsiuh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3iyltqvam.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nnvcuznq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fxiowdsi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pgbcvfmg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qtyuxjux.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3oqgsgkiq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3osxuahpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfnmqvmo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gqilzcbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imqiwfcb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hbtzyzkz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3teyftref.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3erxdjxlc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3depbwnit.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3anrwdxgn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3klyoaqag.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qceiwpvd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3scmbrjfu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mqnsdstu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3flaydugi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yejlaswu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dzdoaviw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xangycka.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jbqokotx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mmmetwkr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aapiuxdi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ddpifnrs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xnefciyz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3anypminq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hrwpkmjv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3htdxtpnc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3snqbises.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tfdubisa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3slejvyye.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wdccrlsn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zjcnohyo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nymrjrrc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3glywwbnp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vielmzbg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hubmedjk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wqefjpbj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gnaqfyle.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3esxfspud.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3axplfdei.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cwuuvwge.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ajdvcayu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wxuuesvc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rwvmzdgl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lkgeaaqk.html


<!-- 参考信息 -->