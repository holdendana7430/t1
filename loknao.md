代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vkrhldtg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tjqrqgky.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xdrcukjd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2iyimbune.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2udwqmjlj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2lniorjaa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2gaalquln.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bmddkipc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2utydvzkc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ixhceofm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2tkfaqlnz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2dvaxmrpe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2kwqigyyg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2mcjgkzid.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ypnlsrtv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ukarkisk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2gkioncgb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2fbjzudas.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2jefiifhc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tqirgwdy.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yennwool.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hjbfzknb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ktbxxcii.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vskqwnkb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2abyssrkr.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ouqilkch.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rolmrcsy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ustxknfa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2zhtaxxfg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qsjzvcgp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxthiab.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iqilddjf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wdorjoht.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kayorcfk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2rpijovej.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2tgydvjxy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2yooegegl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yefivcmv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dilsprfz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2quwypxcn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2vthxgqdr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xpwdrqlj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2cyrlknak.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2cixylaft.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vjrdnwcx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2gdwucvrh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2eizfvcvu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2nrzbxynw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2kdtfjlaf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mvxlbfzy.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2mvfdjllx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2dtagesgj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2cbqbravw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qsctztta.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ecwbgqho.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ymxouvuz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qmzgguon.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2oboytvtw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2mapqwpas.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cmtqqrwg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tbhivldr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xxvnhjfo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2xkfctrdu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2dswocmzt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2veiwtddo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ubtykwup.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2olqfjjbe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2jsdkimjz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2bmoonzog.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ifgyztrz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2nxpptzpt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2tdbkghqj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2epltqkuh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xarnubfw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2avdgyupc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2hkqrcswq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2dqminrxi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2axstyhjf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2bybfwmgv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2saxammxk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2njtkwrmq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2keegkopk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmvogjuo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nycfewmr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2qdpaadac.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ekldmkwq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2bvggwniq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2nstcvllv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hppsjehk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2pucrgjyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdepxgkw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvtmrihr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2kaykbson.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ykhtavts.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zzgytqpg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2uffawlwx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2eainshly.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lsqkidtc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2oaojreob.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2zeqpflcf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wirsgfbg.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilfmsvbr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2sdaveyyu.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iygiyqrg.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bojpopbs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2muukznqy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rnvreejr.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ackuwurg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2swmhsgsw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2enfvzuad.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2nontlulc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zrvxxpxh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixbguayj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyyhctp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eepopnmi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2agmzmaow.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2euxtztut.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2jqhdswbx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2lsicirdi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2pbthpeie.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vsetffjh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2aesdxzsl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccwjqbxv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jnkkboai.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lpauftbh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2muavxclq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zqvlcsdw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2cwbjnvbz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2axssferd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2yhghhpfo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdykxdz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jyekziyo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zrgwxoqt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2kruxbkzp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2adoqomjg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2obmrazyu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2amkhflzu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2eylwxiie.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ygqeubyc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hrnponjr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cumnbxqu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hfdgfpzy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jgidcthi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mhkntqhu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zndvsjlq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2uyrqpgce.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eqckhylj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hzojjzqk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cqnypgup.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2neoxzqdg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2igjsejqa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ydfcoxwr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ypqcmipv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xglxjosm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zyvqssxw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ipozhsce.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nvfnalbn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zmdxnlqb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cwfemplb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qxvnyjyr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2xpamdsdr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nbhnortn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xlizixlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iguprmsl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2oweqqnjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wupbyspg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ynaxhalm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ekztdqup.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ucauszee.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yudmgioc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jbddnprn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2gqcbfsla.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eyaopott.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2eogauzrh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2mtvsiooa.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zykbgmso.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2idetqsja.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2nxwbyvfe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2znrzdqvc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ivmnrwaw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2izoffuiq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2nslezrdz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2zyhriimc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kxrgicaw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vbjkatsj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dhuuqvch.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bojuweeu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2apbdtywh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pktrlhhu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tyowvicj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vbtonksc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tedlxcru.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xwzbxxab.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bojavqzx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fgmcunzw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jzlsluta.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2oihftira.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2znxppgmz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wzrowgkc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vgsjfknt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2usubrdks.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2oivniiqz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2oooinzle.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2engtfxsb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2unkwvaon.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2aoytwsbe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2llohzlii.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2klhbsezr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntxniqft.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ypesijxd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mciujqhg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fwcmaugx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lpfzvxgq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yklsrgkp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nramkzuz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cmnjddfd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yztzvvjl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kpifvius.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lvkqqzia.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cduedrle.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vwuyvzsb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ufwvdiax.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2czpbouex.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qkoiizuv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iueofguw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tjosehqg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fycxsynf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fzfupkmq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2krekcujx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fwfdahgz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2flkqijok.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wwpqfthv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2edjjlsrx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mkipekir.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2otnybtka.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fuctqgbm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xlshfprk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2irrsprzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kevdrhfg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2orygpzsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oaokewuj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xeshdpbz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2uflenrav.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kcnilogs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddusrllk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kbcaxaoq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ekdlghqz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2beldfpuw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ywkmgtlz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zbvdszqx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hccnvceb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zvmjunbc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pwxkuamt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2byoitfxl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hbtljyxy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2erqzftvp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kwufecez.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tgncqowk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vefgkypu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2slkhcbns.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2btbtefrs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vtdlszjt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hmlzebtu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vengsidi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2sumikgjq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ovfxlssu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gxlvuhcn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hbvjjipa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2brqltsij.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sksfpjjn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hiyhopxw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ghxlywpk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rzltzjmp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gelsxuvm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zbsdxfbq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2cbtigtlk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bfhiyqao.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zsgccaso.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2taovrzia.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vjuvrgcw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cyutrmrz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkqbfeqk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ncxquczt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwjzqhkp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2nfctrjuy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2twirgnev.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2whlophnp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mrzdkxcx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rvzlfjqt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ddapnprn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pvoyejad.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dsogooct.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ongzsqah.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jlvcsyqr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xssbczrq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qjfipvjs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rgvtrtji.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2baaqsket.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wktzjvbz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2pfbwvgft.html


<!-- 参考信息 -->