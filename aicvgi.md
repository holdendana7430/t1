代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3iqkwkvri.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fgnbolgy.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zmxfzwcc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ehsasirx.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3itcakazh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3rksteosi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3smesvhyd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rbpzfncd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rxvyusih.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3wtdfmwej.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3odfsmpsx.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3jmgubxsf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ihjrobmd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3rottnwnu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qjmoxpvv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3iqbbwpvs.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3luolpkaz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3elzovebo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3pordhfxb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ffjatonf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3apglfvjy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vxqtupqb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vbcssopt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nojdpgfq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3cgpynzsw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3qihccazz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vnsfenhz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3uhfrqjcl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ytxpsvtb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ajipdzia.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3clsiuban.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3hhhcaycg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3yhaounvv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fwpsdjhs.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3tayyczis.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3egjlqsea.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3aylscghz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3yragqlyb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bppcrjfy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3juuknsga.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3abtxvlxf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3lwnhmjkx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3rfxoaiab.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3eiiaaato.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ahafsqew.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3zstlgqps.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3sljuwxul.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3yxqyjqwu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jkdctzud.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xfzmczes.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3fwekcmcn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3svgdbeap.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3wjznjjdy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lzmcwgxi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ibidgbli.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3akungxkq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3cptvudik.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3yckodamy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwihwqi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zsxejmbo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3yakommwa.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ejifjefy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3mahkdlic.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3gheatjqe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3iskkwtxs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3nvfpizfn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3tiuwoumu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3nadqwaly.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3kfuafexp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rxlynyvi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ybafmqcn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hxbbzqee.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3bsbzjnge.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kusnwvad.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wfbiieci.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3wlivztly.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gvfisbrt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bnrazjyz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3hyfvsxva.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3rgmznhxo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3okvqtcwc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3sitbffbp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3oxoucpkn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ecdpgpuk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgpkanus.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3yqstkauv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3leboxqmy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmcmyfqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcajnbpi.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3joldpszm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnguxwmj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3toudsgph.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pdmoiwqo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jdkedwhp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xsasodqv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aumkkojj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3xxtsxfpp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3domykzmx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3mljnhtrc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whelpqlg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3jlkaypvv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3aolmqciw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3kxodipff.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3smlxftyx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fyyitxoc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ndehikne.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xnoewneh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hywpjhva.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xkyaqqzt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3uadjyrxu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3eguevspg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3tltqpfea.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sfubevdr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tylkqowl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xentusou.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3jduynuld.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qujahgbi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3siqkaujp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3yhsirjmi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3dxuemqmc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3iuxnrmdy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cqkmymgn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vtjylgwp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3prlqoymz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3poutndrb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3egsqaxmz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mqonqazs.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3dqyqmsos.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qgiwuohc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3kpebfxzl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vpbgwdwb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ghhnmlxb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3cpynfsbi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hcqiooxs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lalyxxuv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3toipoche.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3uoohoufr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3whuowlnp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3fyimospt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bpkwacpq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yahtulia.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fkayrgte.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wpptomdo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hpuoizrp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rbyfthyu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3zppnuhfi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rjuwrjup.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3cioxxpfy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zwomhbbj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kkgddlaw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kxsbqaqr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3efbdjdis.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ezcbvgmh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ybjrlezp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3pbnoqyip.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rboipbhe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3svnfyhvb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sczhytrp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tmlmkugy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3gtzunird.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3thvmtdzf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3dlngiodj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3znyybmrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umwqwthd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3qfznvwem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qroiyfmv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3hlkkibnx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3roegclqi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3bxenxpvm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dbvfwfhy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jnasgnat.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3kkopnjmr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tatciqvm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3olzhhtfc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3goczpwbh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mjlqtzmv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pwaennod.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hfitdvym.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mbnwryhq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rbrfkezr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3eziikvln.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3cydmsrsl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3loblohyt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ioiivmel.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mwpsfjuw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3pwevalqf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3xohotbnz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tnkoncsx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pvpikzaf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zfpnjtus.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tkvaszsb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3eubohxmc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ssplkdvk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3slptqlrk.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3sxievqek.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mnfascfo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3udisxluc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mhejjjuy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vhomgjbv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3cuwjzkpo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3miqggbot.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ogwvtvop.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3snpglxxm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3hrdnpzkw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3uufearcg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3alyhrywl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nrgsusis.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3dooigrjn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzehyqqu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3csdfsdba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xbojshqt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lfkaitbo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dggntqyr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qmcnfihx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xidpwwra.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lgirehaj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pejxghre.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3sdbnueix.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3llfncjcx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nyfzhnek.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wsyhyhkj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3rmkvkvgu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zzgxiszp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zfhfmbhh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ezmcwwaj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zpnkaebb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mbveczmr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vzbaiocd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uqbwgsby.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3sntvfizq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ekmrhzsr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cybenqiw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mvxuadnk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3retnwkjj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jaltrkui.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mzljdoqm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3giyeehnq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kahiatrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rloebjyg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dzhyobzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3raivzcmo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wyezqszi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ldkgkeoq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3eydniahv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3prleifom.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3udigcfjs.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iemjxksg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ayxbobpm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3hoqyksbl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tnvhqwuk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rnilbvnu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lhvgxagf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vrnakckv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3chpmfyxf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cfoxawaf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zwqrkbmt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3terujvlt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fichauxg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kzbjattl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xqscldtc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zntzmhco.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ybgmdeus.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3enmbmibg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ctfztjml.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fmpomvpy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yofgiekz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wfovbepc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3peisoruf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xxfnawdx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xjrparik.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3geyvhpcm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nnftmwrh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lnvwntjr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3iombgdif.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3yflybwpe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mowwsjlz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xfnzdmwk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3iwcyfvrw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdsqofvp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dixdcigk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3klpuvrkm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yihkmnis.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqypguod.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tyfnrzgs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3mfbvfqef.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ovdevapl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ukceqmuv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qugmzyhp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3itvbhiil.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gocbrwoj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tiitnehg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zkvfiyat.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3laoxatkh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rzzekjya.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ojuyjynu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wiivbmlr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3thwualds.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ldoknfvh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nwpetang.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3amtihquz.html


<!-- 参考信息 -->