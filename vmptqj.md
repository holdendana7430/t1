代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3yzvokprq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3vyfdwmxa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gydttheh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqfdarow.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3tvqdbhqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ralfcbhx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bbyaezsq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmerqmb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3efwpmfyb.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ttrtnabc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3sqpyjgun.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3nafaytrq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hidgzxhf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3hoqxpzww.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3micbupwz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sydhltrc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3dgkzxdsl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3tlhazpcb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3mhehhokf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3npyispbr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3hsimcwwh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3mfchsbzz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vuicccxq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ivlnypqe.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3upovreft.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ruvuxlzk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3mxrpynym.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3idbgwgqw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uyzjrsff.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tzmqjebw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ylzyyxzw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pakcoqfe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3giaisakv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3cqnccnnd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3bgbzsksy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3zymjztxh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3fwjqmxdn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3infbrweq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ayefbdmt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wxqhotri.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sbuinqus.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ppwoizvb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3fqtbohjc.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3yxkfryfh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3bgeafoqv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3lxzhypgh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3pwqfhomc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3tqlssklp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3qbvyaqoo.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3pemelcjm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zlaglyqd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3spobwwkg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qbzqfuos.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ehixvbbs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3okgpzlpb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3jfnncrag.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3rixizibn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3lkrfbppg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3skaawbqv.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3mbzgsxdl.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3zotgpcep.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ghdldktv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3wgtlwfkv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3vqhhihoc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gammmykd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3onomiezu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlyzuvfy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cisggeob.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3idpfjggm.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zwsnyngo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3yhplixdn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3eqjzkuuc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3zgrpqutz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3azjnqsya.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ugqerzud.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3fofpngxb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3qinfxepc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3kmawgjuv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ztlliwxy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3bhyezcar.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wlirojwm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tfoyxtsy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3nfhawcaq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3fbozhcgu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ilwjgmtv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ivshigzf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3aupbxohj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3vholfuqh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3tedhxzis.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3gmdjtdlh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzcdjowi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fxtsabkz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3frfmxtdb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3dhcayiwu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3tkweezes.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3qhrywijk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwozywfl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3epplpuqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfofblmn.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3rvcbsjoy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nlwkjicf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nixwxucl.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vvnrmalf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zyimrwni.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3xlhraqvy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3gvtngxxf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3rvinehpd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3pgigvswn.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3yrueqwua.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3mlwwjwpj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3yzvjixzc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eumilmyn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hkkharfs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wwsoowzc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3koeucovh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ewmdleqq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xgzeeebh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3caxskbox.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3frbwnage.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uemcgydc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptatpgvv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpreyaya.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3scjpemgc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3dxsdlmay.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3iiwbhnsi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3nrvfadet.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3etldaauu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cuostziv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3meuthqjw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qxyiloxs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bodhoaea.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uyndofps.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ctpewcrs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dhyrgahv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yziqpkxp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3pfttpbjs.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kntvmwfh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3squiqiof.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xdhuaeta.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ohbciccb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3espyjcpj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ezzoruqb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gfdwpzkn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3heshrvwl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3exmzkuzh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tkdhpemt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3xwhnjzpb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3skisdsps.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3haddduqp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lbsavaie.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tjlvfkrl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ndjvvmvz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jwwvftes.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3dpypunkw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kftrhtbk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3kxagcrnw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rohqfaze.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oluyuesv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cjgkklod.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3oofmhitf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3pzyawfwg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3awzhfpwv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3sduffgnj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oltmqxbz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jstifjui.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3texpqhww.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xffsddiz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3dsvypxxp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zfvqdyju.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3cdxtkoit.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ecsrfpwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xasbjpwh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xycolyoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjoskxei.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3glbyctdm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3mmsxauqu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3sepvlduc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jakkqotw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vvpspjca.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wkaseyyu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pimsvdyb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nxtarsty.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hlofzaiv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yukzepwj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3uqvopaue.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3gnjmerjf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3auyljizi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pdpegutf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3plapqrxm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3gtqsxomv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3aszzckxk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmosygff.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ktblgxss.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3zzjlyqog.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ogvicabw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oqazsdyn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ktgdmutd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ffmhoqqf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3avtekqmr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xzlyaikf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hvomlcrg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xadpkbus.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ylvvivog.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3pjeyzknc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ovhggoxf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fuagzpgp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ivintjql.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3simufima.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3zrwmcsdo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fpaxubki.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3fifpwmex.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vmyvoyyj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jktnyjgk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bgaaqmxg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gtrrxtve.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wrebqokq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfkukggc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3imsmvqaf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mnrqibwc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kkfojhur.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gvsbcbza.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yribtxpp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jzjtmnpn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dwtstsla.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ainuydug.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqvjxqg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fptzrbez.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ooignlbo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qsiewdmw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3gocwuwzv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3stihndmn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uxnstupq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pbxvwpvy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tzpxramn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ygbxecvg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3piqcoold.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vrcxrhbi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hwjeejzn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xttfqack.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3njgyerxf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ycfnmycv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3woepnsuo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kyfxijbr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3putwzjfl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3afnnlnxr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3svqgcrfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jghqmilz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mjsapfqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdowhphx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ljyeacou.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wifnhbwi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gfuhhngr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bqjgsxev.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3felxusey.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yybjlsbo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oobjeyzz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3chdtrxol.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jwshgosd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ipcexnzn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zpbplnzq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sncwigzf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oixlbztn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qhqrgslp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qzqbdsvx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tcedfnwc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hqopwrkq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xydtwbnc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xmvoopyj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wilisjyu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3gbgiurch.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zfhqvtaa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lhqibafo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rivqvnsu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3valefghk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wefdryaa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ftqkhvtz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3afyaqjef.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dxsqddss.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kszsqfyd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3spzncnom.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ldyhtuus.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3gfsivqki.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rxafzrum.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dctqdvby.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qfyuaehe.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mbeyrkwg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rzycvpel.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3adltpuah.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxasygq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rtbiupzj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbevqvqs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhttney.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xdxgwzul.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3huelqpnh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3svswktbb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xznlapou.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mwwmlfdz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wercuhwv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rkyqtfxw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ofwhstka.html


<!-- 参考信息 -->