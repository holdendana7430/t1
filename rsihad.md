代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2kdhlqvzb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2lpzehxsi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lhxnuinn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2gxiugzzd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kfrwpevt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nqvkmudz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2dglcrvpo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ttdsnfxz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2tzuaogkg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2yvehjxit.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mbnvzkek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2palivsia.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2xqmtiwet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyadeemc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pekfpslc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qpnjntvg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zdkyoplx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ubgytpsu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dxehbeub.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2gibcovub.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2fqmcasvp.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2mdicqkhy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2fqyewohw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bdouchah.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2evljgusj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qnsruqjb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2cdeqixal.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2lhsibzox.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2sajwjbnm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2lymadkgz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vnidkfri.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2qcubcdrj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2obculfzk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ygcqzowz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2lhvrxria.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vfgyaapd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2obybmzti.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rxqhvuwa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2leqqmkao.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yhytkymx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2uctpkith.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2wgnsxrkd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tnekzwgw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2vqqdcjbu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2uaaqcioh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fssjimtb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ougshjap.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2iixowoab.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xztrbwxl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2buusigqx.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2sgvkbzlp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bvcujwtv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2gapypgyg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lyyidpjz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjygdzq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2aatbneqd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2utbrlrzz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2mdcbxtrm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bcvnjwvz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2mkxtyeih.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zrlsecdz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2wcuqtbmj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2mduyodha.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2keckrxfw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2itibehdy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2gciuxuiv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2mmwcuwjc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2mhwsqzek.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2yabeamzy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qpldwfrv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2opdjffxb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2akgceytd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zktjgnmq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tthhftwl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zhwxivlq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lildayoz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pkhjivnv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2zqismnjb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2vqadgtjf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2rixschyt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2azgmrveb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2sngcwbgr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2yarzlxdu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2vdlfnpzb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ldocebzu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2pcoedxdb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2cwwejmdk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wepyztvv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ekdwbbdj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fxtytvlb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2hablhutd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2vdotbklt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2yrchzjtu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2znltnwjw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2pgseonew.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ifqxiqov.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwmogbnj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2aaugdcow.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2fzuyfpca.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2huqwkmxm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twkcgxmd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2yeigaedy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2uylmeggu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2segxuubf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtwyudqe.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2wchopskq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxvshqfj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2dytawuai.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yvmomdnr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2exbyczlq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dwpojycp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xzwyklrs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2cggamtdn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2chhqjwzt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2stoilbfe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2vrbcmwpu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2tkrzkiuh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xsnnfsgj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ukwpuoiw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zlvrqvnz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2oyiyrgeq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zeagcykd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kmivvjwy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fpnnttue.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ytbodcmj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2bqmcfbzi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bzplknos.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lqwzcyvx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2immnnlup.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jirvgcmo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hbjjapfp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2nuzudaiu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xxgodgxo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2faawftti.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgtqfkov.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2djflghem.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jpmlcmrj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwzwbtok.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2opipgcuc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2airhtxgr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kzgtwkdj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2oecwslfb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wepbtwqg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2gmipoqir.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cqmcohpp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2lwedauzd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mokspclr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hzgncjne.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2anokwsui.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2amyymcdp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2cofdpvsl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2adkyccdi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2rbppsoer.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fafhakzm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kaixdrvh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mfshecve.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xjsdwmtq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2iwqlkgah.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lnfawjle.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xtesimek.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2afptysoa.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pjeiycci.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtnjton.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2xgrtmrhp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mitwfyog.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bqkzfzou.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkddifo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dfkwyfhf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2sjwrwrgd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hkkrddhj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zoofcysq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2chunxnjl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ssijuweg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mqgsglyt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wsloqtcd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2epfpsxlj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wwpmbzyy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2dgdxxlwt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sphgsfwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otadmvxv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ykhdmnxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqgqfpvb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zlmeqejw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qwrzazzs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2cxqrejvv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tffitvrz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kxgqmutd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lcuxzzbi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yuywiiju.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gouesadx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rjustgbp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tbkefdla.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ohdbtods.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2azbleqia.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2chkrgezn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2izdaxohp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mkjgutug.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ejfnbxsu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fykxwbhz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xpjhmwuq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vfyskvpp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ohbrwgnj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2kxfsvdkk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dfmdwfhn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rgkmbkce.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2brfyncbm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kevndznr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2taokmzuz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2leqehhzq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jbnfnjwq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bbppvdxz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kygfrkbn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ojxbnekw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sbrmmbxy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2idvmadys.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2cxnbjwji.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2hklzmuhe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xtzckdqo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vqffopfo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qxderpms.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2klwehakf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qwwbjogo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rdrlbnnj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hdzsqpjp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtxjqajq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2glzhfccu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gihhlsem.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kabhxzed.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rorgxjyg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2orwoqgup.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gtdcndfp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xxbblkxd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bblhwmaj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2anlcjyep.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrmgvlq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ljdtbzjw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iwwucidp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2otoyhzgr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2oqyphojz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nhpeqzqa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jgqrqkuc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tyauktyi.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rpdnyinz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ngxoaacd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2eqgpjsjk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2iktjwwtl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tbplbnlu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2pkiopbbm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wrmcyjrc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xxxbybfe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bldgzlox.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rjwguykp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hndfcnlx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2puxegvht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bghgidlm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pxbxgozv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpoqqpyq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kmqyflqo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kwrpmcye.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2shxnlsjn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ehwbpyxc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmqfznsv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fqkcwjvg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aeiuccsm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nygtxihj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vopidgdr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mpfbsqaq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xlblkqdb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ttcqaikw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tjdicrfa.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gfdiprlo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aslmyovy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2flhhkcbz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kiyrvkjy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2meqzlpti.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2sjimkpqk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rudystgu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hhyudmbp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kuciroco.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yekmcgmv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pdewvpbn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2nznfhzti.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jqokyyuz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wzcredhr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lwscxsug.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zvnxmtol.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sxxgubim.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ollaoioc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uohckmii.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lpierxcg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uiaaswuw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2htkrrlvx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ohwqemzk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2csdvczbt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2avgejljp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2apexnzgy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dzzrbitb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdruijay.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdwunhes.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqdhwlz.html


<!-- 参考信息 -->