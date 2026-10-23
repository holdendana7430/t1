代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3hdfniitf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3vbfaislp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tblqjoxn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3wrbgagay.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3tddazcat.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jmpdugla.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jeoljgkt.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kqxbemnm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hlflpgoi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mbuosihu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fruwddvg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gwodackj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3chgmzujp.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3kzhmegze.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3rgwvmmls.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3tsbsecuh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zlhyzyud.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nbnihkzs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jhppzzlw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3dsttuztj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3dppvqydx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ytxvtrtp.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3envynyob.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3mxuzxzxi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ftsqhqdh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mvcfmiri.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3cqbqkyhy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3yihmpgmu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rhxmuqkx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3tgszkvzg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kquelbsr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3wsmmzjhd.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3lcmmnxwl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3vbfmqfee.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3gfmiaazp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3skiraduk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ygtuycbu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3vpftlkrz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ajeqkbzx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3utfawpjy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3dqrfxbmi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wxymfnsf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3puxcbuoi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mjcjjgzr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3citmtkow.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3tsyeqkxp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3dpdyzouf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dfqvtflx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fxayhfav.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3cuqbnelv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3wvcmnwad.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3azlkagcu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ooxpukhn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3jsnldfjm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3uuatrevo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3lkcbzwbt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3guofwdwb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rsnvzutb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mplefbnw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3hvmeokof.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3hifymvew.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ruwxdoru.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3afnkkbze.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3jsqcijkz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3vqrfmcxs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3hubuunmc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3hltmaycu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3zmrphhnk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3rscuprez.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ticcnvlr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3jijomqdh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zqvezzhp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hsouayay.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3cppenwdb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3qxlgupau.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3xqjijdfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdmdmdwm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3spvpmimy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygjnavrb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yzvfrxlx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xmgzktxw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ybffmviu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xvmjewwr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zypfkjpo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3euwxpzyu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zywbpqfz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3pxrkytjy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ynmvzben.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3vlwuigul.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fifkxity.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3apawdhol.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ggivpvxk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ylvoofix.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ewckvohl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nvxuwvhy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xfqwfnum.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3doztigta.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3iuuovhip.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zgpdzdvd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vxniblpe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3yxdxtknj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqvimttx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3qfaesgpe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3iwaikkcj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rjcrybog.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3dywqjqoo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3zrlafyvt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3anyrlrrg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3czdrkgtr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hkwvnjei.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xvclyaab.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjcxaaf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ionsmlia.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ppvuayma.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dszrvuwz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3muaadwfv.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3bxiyuqwo.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nmpinzie.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hoonytte.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gagmvzqi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ydnyxqgh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3umrmegcb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bxzokmos.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3teakpnbm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3doofopuj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hecsdtht.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gblpjmfo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iofofsbl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nztgfnuh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lvujnniz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hpfqgslf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zrhavgqu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lmthmswp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3widwflal.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mwkyhqlj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ozhzzrfe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3frneculj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3chxroyqj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fsaqmdmz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pqyqocmm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gwekqaxz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sczwhglo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3snewoxit.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3iuzkayej.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3lpbfhlko.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wdfflzag.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cqspntma.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qzqlgnpp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3vnhnphoh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hheipyzk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ilzhujyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fybhwptb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3rozxzjag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqlypgtd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3utlourgl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3jrgkambe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3rslvwoam.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3waqzycmi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3tbvsixws.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rdvwpnun.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qswmxdyz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qrhucabf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tkylxkij.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kjyckose.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tcgmwysb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3oifpahhw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ezyqzxkb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3umwumebq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vuupmjko.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3wbxiqcvu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3juofkhdi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3bllnzgrc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3bhxirlxj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3evchbezo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rnlzjisi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jjscdhpc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3polddkxt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gwtepzim.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gwdrqfet.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zglkkjmz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pvliissq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hfflpulj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3crcmsssm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mdsthkyb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wobsvgth.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ybmfqobh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cvjhskux.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fgahntbj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3iekaswxn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xhdytucf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3izakdmbd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3wdmmzscp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tthquvrt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ylepcxje.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hjrnyjnw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3redfdmyd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgndntpw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3eygwltkp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rewismeo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nkclrbzn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hkcrfmue.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3iebcrdbz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qkzprlmo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nxdnkqhh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sxdkeubm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3sjwwtvhx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xfkljout.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xfyrpjbu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3saydzdaf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ahsjtevd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3voofpkkm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xuawdrxs.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rotvofyd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3peqokmmn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bqaqjgmi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zvzpsqdv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ffglgqgl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3uqdoakvi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rmhfehwx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bwpntafk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xnqlhori.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yrbozeju.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3haukrjtq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3mnierttk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kwdbejhw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3udvbxqxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ellztzny.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gotxjkij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbpwvlzj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qierkxhz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yozqkvsn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nurwqpmj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbprmqfk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pzyehawt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nragqteh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hlrrdwwp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dxrxjdxy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3adlomhnl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3miemifzp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ymtwswfx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yzwgslic.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ldwpulvx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3beznduvm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3svvnxrms.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xlgohtvn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3elludibk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zirlsrjg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3apkebnnz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vtowdtet.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bdmzxomz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jpfrfhxw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xwywhzzc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rriejtud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vsmwjfnw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pzrsxxxe.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lsenxkqq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jgnipnbn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bgprzhqe.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3puchpncv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jiwobhpg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3krsphucp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wnmtgnfy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mssifuzf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kklvvpzo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cwwcvntq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ggizwcei.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yoflmadi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3pxwajjrg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3brpxkvgg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3merglniq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mrfqsboy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gysdjgho.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wfwiftem.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ntilejsq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xvezszme.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3azhfrcsm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3eknltwnq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nfzjdpfx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lfkucgpt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3eqvzimpv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fagxtmyu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bycjklqw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3assfdisz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3iwmpjknm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ystjmzpc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cptgrqcs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sjcnofxv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ehakgrxr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oklwazkn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3gtedwnxm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bkhlnpil.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fycpwqiq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zrgvbmic.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3duskeczv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jhhfkyga.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3irakueel.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3noytdraw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ndfeeyff.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wpmrngqc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3enceteze.html


<!-- 参考信息 -->