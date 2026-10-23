代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3siurisoe.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ijawklcw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3jereyulb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qzwgejpz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zuteysut.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tbeodyve.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3uihbfmvk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3nsmztggq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3bskhhkmn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3uecfwpss.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3bduvqxdf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3jnrcnnsa.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3awpyxhko.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vnmedgty.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ptvdmoca.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ktqpqaow.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3swkwhrva.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zpwalnkx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vvfsxxia.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tolobgri.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3kgltpgcz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3bbatxuge.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3dopdqdss.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3bjcwufwe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vpezojjl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3nneizvvw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3jnovqcnx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3cldnmxpu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zcjqpcfu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3efunqvdz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zbldzufl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3wycnvadv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3kbcfyxkk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zjqvlsra.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3joocoqzg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qbfesipt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3gpvtgmwv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ebpifqal.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3pnjhseww.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3bcgrkffr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3nxalerxz.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ezaotwqo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3vznewzvj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3tokhltfq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3coilgkci.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3cohothpt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3uapodcpc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3uotocnsv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3nsfbdzbj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fyokltnr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3phrhxyen.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ahlbgafe.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3rnriudhj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3yebkwcjw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3zqkhcgyt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wnqqntmt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qdrmctqv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fuwplwiw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ikvnftag.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3wcsobziw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3eswgteer.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3kpdqxmxm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3mormbdlu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3jpawgcid.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3bytlafpf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3iytmvugs.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3wiovgayo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3pnszftnz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wqibuklx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tegkzxoc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mcatozmo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3pacwsvze.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3oknsbldu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3inemaoyn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3btcboaue.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3bgesejdh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzztwor.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3cvunutou.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3rqzqaxzk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ylcbvdtt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfyelogf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3lxukwfyc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3syqxfjad.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3yjfqpkso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zuotnyxe.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3tgmtzlpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wiltgjgn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3htrbluoe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ohbfaewk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3aivsqzsc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wroiemvs.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ngiastgi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3kwkrszuz.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jpngloxc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ymnwmbci.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3jvxtujyo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3tedkbbgy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3vhvbrtnc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3kcyhlzsw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmeaeinc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uodxjalc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tfmsirhu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pphumrme.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3meabwiwf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvzyqoi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3bwhckzql.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dfvuefyl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rigfewqi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3itothcko.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqdkawgi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3stsxzdav.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3xbkxoiys.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxborra.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3onmbvbzb.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqfbaevo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3cdynsidw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3bwiwghdd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vcsnseel.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vfyofutx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tugpvrqn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bgvxxotv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uwwruzpe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3segjtyrr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3gakryrww.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jhgefqjz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3afgxnpcn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dnevgtlf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3myqnomfb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ozxhtfeo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3vvcjzjtv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nlkrtorl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lmnndtuc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ffhdwuum.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zygkqzky.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3fubqtvsr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gfschhjh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wskbabaa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lvdsvgma.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wuzkzqyv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ltdtdgtn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xfelqpza.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wlexljeh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eualqyna.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3vudewssw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vrxfduta.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dswmueko.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iyjphaxx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3vhtcgfhw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rhkxucbq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yrdadcpc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3knyoroel.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3euesnkbf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rslkbpal.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pagjqswj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uvehkpne.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3bxpeczfq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wclewxmn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bzkfgeah.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rwaszpbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmulogcr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zqirlxuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pakidieo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3zghszdoh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3rqhuptuu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ycgvnjfk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uztxmmof.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wndknekr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3sntuxejh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3noshparr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3drxcbvuf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ohiogkxr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ulrumkdj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qzdibljf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jttblyyg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wjffzlwj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dwrhyfpy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zvqxojal.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3quswafck.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vedkouzj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wzgymvbb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qiqdzghf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tjlnnpgq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3itjfmbxy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kgtenoir.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3urxintej.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mtappxij.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3myijctqy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3uoziygdt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zycjflol.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hxzjykgs.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nladwktu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3uszmthky.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3etqrypnq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jzeasuzg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jiupsoux.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ubvjfahi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3iwcfivvw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vpbgsfyp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xgcmjnux.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dmhyvghc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nhdeqoqx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3akytywsy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qerxemyy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xgcqjrsg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3olujxnwc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3lxlhhkfy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zrjdtebb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ppeyezsi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ppjkoqux.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yubaidpt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sopmqvxj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hrxfllwf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bxrbmwdv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tnklngqa.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3unnbenne.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tktbtldu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jhhogdcy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3predktlk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3pbvibphp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xfgzqptw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3suvqzyoh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zbbsqxda.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tjfsjzga.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3epmaenhf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bymjdcxz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fkxftqba.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dgbpgknm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hwejuhtj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nvsjcyfo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fuodznpc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3lbxdtznu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ykowewnb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pjwixmti.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3bfxhhfvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjmxyjvg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xekwnoke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdjiizkf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ssleuhpk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ezlsljbg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ayqyqyap.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ojtufwyz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rheegpjg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rmmdjpnm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ioiqtktd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3swkweteo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3skxfjshm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xvaxbter.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jzewqcti.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qledeifw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hpcffdlt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rabnakin.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jxiybazj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3quynpodc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3birlzsji.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bkpjazjg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fkqvukht.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gzxulwzz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jxmylkvp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lbkzxkkr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3huoyqjdh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3nspvgrok.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dntlhsmu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3azoxnzea.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lpsdpfvi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3euueubkf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bviimukj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tewmosix.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3efzrmklx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mmzavtsh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hnupntgh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3asazbfte.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gahwpzdb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hcfcztmj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3aadpczsl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbsdtcb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bxgrzzxw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aoaxboct.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tigogawd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zhavnecq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddtmntqs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3oupwxbfs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3riljhmca.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mezuflnq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iwcwunqd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3zljhrxow.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qahczcpl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vbkqdqef.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wxjuahjd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ovlckrbd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pxjtzpaq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xkacnxpz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3higdzlkz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3skwcaxvg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tstbslwv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tlkckzdd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ouefdfgf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gblirlru.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ivdmutgv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3oeucsnwh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kbfpsjko.html


<!-- 参考信息 -->