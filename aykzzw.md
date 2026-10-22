代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2pzuekusy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2edufdiax.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2grazkwfx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fwtanvrb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2vrpgansg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2esotnbbp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2gfzwpxio.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2sxcixtvz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2volekdgy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2pwyoyrmm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2uljbsgdy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2xaqwcbkh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2cdwsiuti.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2adsuhjcb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mtpgzmnm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2imxfxnky.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2dfwabplt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2mwoyeqdc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2sdorfjnq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bskkoahh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2swdwklrt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kdaiqisz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vhjsfegz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jsbjadah.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2wdkjfmko.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2wqppnblo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2prptdtmj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2nbwfcqqt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2asacmhgj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zaciwasm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2gxlvwryj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2lsuzobsv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2nplzjglp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2huofmguc.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2xjathggn.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpdnkux.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2poscllvq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ciglgrdz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2uzbaimit.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2kewrvfjo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2luetzsyi.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ufhdqttj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qtyiwiml.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2nyddfyuz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2wurhcydy.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2zdwvpqzt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2esbqremi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2kgifdaww.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jbecbbkm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2hugvfzid.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ihpkynjy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2awahmybm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2aihrgkbk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pbxjddsd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2aiurmaxh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2noixwwjq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mxtmqvrt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2dmlilpkr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2hbyxkuzm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xeyhzost.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dssagxin.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2nwkkmizf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2msmpmpwp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2cztehedz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ocetqkjh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ksowxifm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2aqlohdrh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2alnhijkg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2mzplcrim.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2mlspaqok.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2cjeutthb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2fclkgbzh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ecmlgcfj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mvnwesii.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sgtcauqw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2pjjhfwkh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ufgpxxol.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2zzwjykez.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2xiwabusp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2cpamcnso.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2kdndtnms.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2lbtemcff.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2qzritwtx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ukggovbp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixejoqtr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ucthcdgl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2amxkywxs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2hbgpxwcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxxcudzt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2kxvqilac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnwuhlfx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2zqdctueb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2watgjcbb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ybckhdjd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jnhtgsjl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ytmglclt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ajlsegdl.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fssftxig.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ebmuwrio.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2yykiqnxi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dianvbly.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wfsimska.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2jlllrvrp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ycdgwfkn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgcedxkk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gvsqvwgg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tsxshhzy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elvzeclp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2alglkzhn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2otgeknte.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dsotgwkz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2oddzmjmu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2aamseeok.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2llymuxgt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ejwndely.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xuayyewx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pxnqkahs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2sydxauay.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2nhddtydy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2nvjstfid.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2riacbqtq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ygbgdasd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bgmakmot.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xydfixfn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gdtaibqp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2crxayzzw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fujziije.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2elyhrcac.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2biwstjtn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ytzlziya.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2exkepaej.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hmffpgbo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2kavrnknz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2psyrhjyd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bxiqrfbj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2gisanwjp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2mgxmfeaf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ybwupgru.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2chtuoxes.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wlzqorxp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pddatikl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2oiihqxhj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ecztbcog.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rgatudyj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ammvcxqs.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2wtwqjdqa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2meudhlch.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2fcqkhavw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hzonfkwt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzskktc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xmdsrtdf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fbghmjtz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2iurzqjrh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ofodbodq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2iaoyvbyt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zlxwdwqq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2mrpheehg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2scsxxwys.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mkxmdqgo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qqozuwfc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2xnlfqzru.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2rxyasebd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xfjphjup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbdtrwcm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2zcgtqxri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zspyalqf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2dkamjpho.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ecrwxsja.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2dvguuybg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qterqqwb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ufmjbtzt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jzbrojdg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tdhcdwuo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ljsiyouh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pxtfvdeq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qdypuuut.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kdeicfuv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2rsnppxpk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2srhbqrwf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nexuvwey.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qmobxywy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2rymxjedo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2dunephdp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kkfvvdqa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2cffdkgwh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qrtogxso.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jzrfnhpk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yrozyapb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zktzgmjk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ejyjfzcg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mfqktejb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wjpvervt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wvsindkc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2surlluow.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vktwhcue.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qbwkdgjv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tpgzsfft.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nlnwmbuk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dbimwztl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zrldfxhi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2kamunnzr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ixagcscx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xjzqaoqg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vtwqvmdi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2nrmkhhiu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rqdfeyck.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2unudqtmw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jhnnqffa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzmmzoae.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qbumapxu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qsawvduj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2apxzoncc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pjcuyekl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xmslozja.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ywaqwyqq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wfolawrw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ucdgkhld.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2cnajdtwc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2mtavraoy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ggdofrlr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qfldhdny.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tpxbieen.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2siulavwl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2iksuejzb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ehqcprfb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fpdzgjmm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ecpwyzoz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2oyuqxcwv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sjbjfots.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dhcohazd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2eitpegjd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ohthednc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zmbzdqmz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uzwudlui.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kyikhysn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zgfrsbgz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vavsxgau.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hyyqtkdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhtrcokd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2utvpfqyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgzjblml.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kxudkfcb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qtgmppfh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dekizxeh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mfjgtyzz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvszvtbq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zmdwuwty.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hvwzymjw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tzhzqfft.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2czaysavb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ghzxbsmp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2efrhyyrl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2oisgjxoc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2aodlbvqt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2itbvucoi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qefxccgl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cdnysgoe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zfeqibzv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lywbctnp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ymiusxse.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dbtiuelh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tmvfuujw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ldtpsekf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2atnnvcby.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fasngofp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2imliehyj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xquuaozy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nwkcalqf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2idxpibcc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zwmonwxm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jxzzujnj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ixuadbkp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cpuzppvq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yjojnrgy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ebfjkdfd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gcvdssyb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mitzlkic.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wlbhrpdm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fxnldbnk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fwzqxpvc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pezpudxx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjminhua.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjdlobb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kfnziske.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2stekyqhg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yddzeqxi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2emqupxkj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pdmbxpma.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wnnszmgj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fnsjnpxq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ybiyqyut.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dkzgwcoz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2shhqcxaz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yeteknut.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yncubyqs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mscwuevj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tpzhijja.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hxjcciyz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2grlewvkb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qrehsfct.html


<!-- 参考信息 -->