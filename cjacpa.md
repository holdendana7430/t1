代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3tfoukzjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vynrxyyf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3alkkrbir.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3bcicombq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xdxsevns.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3oufdsnrk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kwkfmfta.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cclitycn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3kxjznwnl.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3rmnpkkhh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3hsidrqrz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rldzdqxk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wwrlrzib.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3tbekogcw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3urteiycm.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3kglpxlmq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3kdkuznsf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3dhkhsmqa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ufhymwbu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fdpnucum.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ugqojglx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ukrwripc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3zblltlze.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hrorbjhe.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zkwmvqxc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pgcnwjbw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mspzsttj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jopiwskr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rlbdxavu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ulyakcsi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3gqtcvcdj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3filxlhbv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3tjnkjrag.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3nojcfyzg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ddczpuac.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3fuiytehh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3msylwxcf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jqcyhlir.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3xpqtuhmv.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ftiiadaj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3viitcgxg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xbrfpduk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cgqwipmq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hrthmvdg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mmcybzmm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3mhpeotww.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3thsudiru.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3lbocjcjh.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3hcesvxfw.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3dlzdbrpq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3fksimzsg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3bqkunfmc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3hoctcizu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3bdosbdmj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3agjuejxc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wcqfchho.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ddixczic.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rlxuirbp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3eofurtwx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zupjiioa.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mbvewzdw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3pbojcbtd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3dykmfywg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nfdsatjb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pgqprxrr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3euemnsmk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ycrzaghw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3bpgrmujh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3flemvdos.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ftewopde.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3zsdzytkh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3mtxvrdkr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3hmdihnqx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3pzazqrfq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3hvezdquu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ahekqknw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3kizyhfhr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bupvjrnn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cvfaafbe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3guiitgxf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3geshhqgg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bbekwqom.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3syvgkdql.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3hrrtmgnv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3icyokigz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3zxclofnz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3lkdmwyqj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3krdhxwfu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3knyghjhh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3sllulxdp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3iiuqvqqb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ecyemvkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntbfonnl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ehdnmvhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duzrrogu.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3yrkdemti.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3snhozbss.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3opsmqzzq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jsnacmvx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gpojrocv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ajvodhks.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3tczuktid.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qdhqgarx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3dpsxmdap.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3isbbayzg.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzygeqce.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3owuyajra.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bmzchqjr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfvbiio.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tjyztvra.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ezmeyjbf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3htgkdcns.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhohsbuh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3pzeydhas.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wwfxxmjf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ytvwadnr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohtdetys.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3govuskbp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3qgjtyvra.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3tlojmfxy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3zxpacmfp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3smglvjpu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfnplfxq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pvuxxqjm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3cpnwaneh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zktnagjf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zmssiwtl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhwzsdd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgyfixf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iommlxyk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xdjolfvi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3yjkduvxw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3sybdiihn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3aocvbthf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iapgiawq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wcjctopb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3rqmajlhs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jfqpmkks.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cjrhpfbl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3bjgsgnzn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3oavkyxpk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xarizzaa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3rpupoukm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vvxbkxtx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qxktybto.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ievvdlwm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3slsllmix.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lhoczfsm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3acbyjiay.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3pppekrch.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gjfgddyu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hweveftb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yzmuuhjg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dmyaandp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdguagx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjtuvxc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3kirlxoyy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wsjkpdvw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3sfmqyqxd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lbtxwuly.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3qweohypd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bpkwqxce.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zkfrpvbf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3nsykbiso.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3nolknsyg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3htcfdxrp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xayhahmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbuhmhhp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ajzdnkjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yoxxwpkt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pdwvmlbh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ekbrpacb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ixvizpxr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sxfndxjr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hxitzrwj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3cepjqmrb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zunbkfje.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3crfajtvv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nkvyaxgt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mdtywkyw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hfkoqnjh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3qybzingc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tpvxnrpi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mzwudtkg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lcwkwrpz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vaowrfpk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3yhunthba.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3uybevfty.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3udhgsxkc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3abmabgdr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3irasrraa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wnuqwhhb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3msquczdb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qxifzrmc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3buhkwzml.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3bjgjpwij.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qodgzcuu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3idmaaqnh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jvoorfaz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3aavhcneq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ettpruro.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tfwtnugr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fyqkplsw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qggegvvi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3cdrcmscg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mdkatogy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3fceahthn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hbhxrpwf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jqpkeeqg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tzzitazh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3invuruql.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vttjtpim.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ljllxceg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vmklbzkc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lvahpotr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hvtvavkr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vljqfbhw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zclenvkb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wkktqnwo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tfbpewwm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ihvdiexr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fspfypzs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdbtngs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hwwrshhe.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hffvgzmc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gmwyuujx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qvbtiher.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jxjcesgc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3njsbxwop.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3asyiwgdm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nybpfbal.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nyvsltlb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wmsffbmt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qpccstuq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ylewtmcs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wxkcdqod.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dusxhmok.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mkavtukn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yrbngrsh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ifsbgkra.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gkhcmrgi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dwqzqmqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anxolzex.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3acgrievz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nftpufsm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3srhlxsqj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jsbyctce.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jwycbcuu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vplanaoo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dhryppwm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jmuggjsi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zuatmkks.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xmattsqp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tdrrdmud.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lyqmqwgq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3itjbzdmf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xnjooemd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sxaxooji.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cthsabmk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rokbtzaj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pdhtuxsf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3elanpqjq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lkygggyz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kwpziyyr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3owwjnhvp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vagspgdr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lpnsixbx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3awkgvbna.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qdsbvvlv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zunswtvq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bdgphton.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3uojmfkly.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ivhhsypl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3nkqvnqgu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3afafbmsb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qwvzluik.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xqxcxwja.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cbpjninp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jyqsibbp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vgleqpyt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ekjzmvkc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wwquooja.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sppnoowf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hijzpzuo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dblmtknv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clueufdy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gwjkueqj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mivculdl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3mqtfdcxq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3oztdencm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hogtkalm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3przsqfpj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qhsgbyqj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3phcsgecv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uahvwwxr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3irnsfxle.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nvziwijd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jevuxmjh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3whdjuawj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ivtvxzii.html


<!-- 参考信息 -->