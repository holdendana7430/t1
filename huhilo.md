代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3uwcrdypx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3hvbuqtsi.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dnjtkiae.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3epnbrwhn.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3uqhysrax.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3zcinrxdb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3xyuovyds.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3atrusqkr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3piybbydq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3khctcpbr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3sdobhvdb.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3mmkfbtfl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3jqworqbp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3oelwbeit.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fuyioncz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ikhaxvti.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ivyppxka.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3htzsjlcp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3klhwfnku.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ntmuvqai.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bavrnxtl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pebnygup.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wafblxvd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rysgumao.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3vtvqkptk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3hhkdjxwp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3buonvnko.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3lhkvlrpb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3jbubivun.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3szspexrs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xkmpflah.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3hndxpykh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3medvxwox.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3fxguqrji.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3yjxiffzl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3xenklkes.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3qligzyhi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3sxwniegw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wukreetc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3eyhrcdyr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3prjmexok.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ukpeypdl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jmukzetv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xavimmho.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ltukfaio.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3atiougjp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ginbiqdp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3oyayswmz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3erggcuuo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3hbjyuacv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3eexfluqn.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3whrjawlh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3yaonvufh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kpbwsgdn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3lcaiofad.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3idtgejja.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mzleerdu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3yemxuwpt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3nhhkpknd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dmxcbhqk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qyatalim.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3diaywlda.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3iuqlyjpx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3uyipaqri.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mkoobyxm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ubfyzvqq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3bgpsykhe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3pechtrqm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3vnmvotfd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3qwkcmlyf.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3smjvyaot.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3zuxhzlxb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ombfzzhj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3sbvlefdj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ehzubgkr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ucpxqjwo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3huhrmokx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3jgfovnyx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ruxleuuq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3dhszuzry.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbgwiupz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3edmgmrqg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3uyacdykf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3urzggmnc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fihjkhgr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3tablxepu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3znhmmvjb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3srbkwaua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkmlrspj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3dlgyrbto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okvrhxwd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxaqjjho.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pzchwisb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qgmozfjn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ykyupube.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lyktdjhn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ggveqfoz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ibiwyppl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ywcsnvvt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3gnlcevsd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3xfcggzms.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3lgiittjc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3gksniejh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yplixphi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zfluutae.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gnlckrry.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gnkvbare.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vbgbwtcg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbulkbto.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3nlqkwwwv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lgccvigr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zwzwwfli.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sadmxadh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kxtvnkro.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qunducsn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3wubjtylc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjknpxa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3hmngqlwb.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3oinwqbpc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3qlovdaxa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wcctfgec.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3poaduvbe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ndurjzjr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dfyykiib.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jruycqpu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3daogjjeo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pqhohqoi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ubivyhjc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ovpdcelp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qsnccyyv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rrsnxvhb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jgtezjng.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3opgccrvs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3wevenvfg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3oiaydteb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3aiscifaj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ivcsdnbh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ngmriyzd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3zpeijtlx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dojqvrwp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3panxglpg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eejrjjts.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uvhhvfwk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ygzalwdl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uekrcctn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3patutlab.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3efviiwoj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3jrjjiils.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jxwwgefh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zjharmui.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vrpmvijr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ybkjfacj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xoskrhtz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzbsgqb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3uvqfmqyc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3iuzdmmkm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzdyosqg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eymhwtig.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dbdechof.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3pgsmzksa.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3rhlszeat.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3nmuaydvn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lcqcrfsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwacmmlo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3aelhvtkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmbjdzht.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3qztlnyea.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3bscohrpn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nzsaiujr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kenlwjgh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ldjdkraa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qbdppqxg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3flxflejl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ayrsjzya.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3xvgvtlan.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3errybbzd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3aycbqbmu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3plurrsbd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ubudwlgr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lcbgtytn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hcbwxnxr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3dvvbhkkv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3bwsohtjz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dlmcmyil.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3lqppjqlw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3aarnggye.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tysfjxeh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zhnxkhwf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3awydvvvk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ryoliunz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mfndvgtb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gmrpxuhw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bowcnatj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qsqqsbvt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3xlwoecnz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3gccpagpq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fexaxrul.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xblvasff.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qmwqzhne.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tpfqviua.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqkiapv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nfmqydut.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nsmewddm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vzemizqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3yjbubeqs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fverrgwt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wkpbyjlv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vzajlyhd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fuznlypy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3kvolkllz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dknlnvoq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xplqssda.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jumehjsh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3annmnixd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3enydcllk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rddqgkna.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mhnkoyhc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3szkwimsa.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3iexeiluh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3htvciqhz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mxkknshp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3iibnqgnk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xpyiulkd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3crlizduy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rrhwnopg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jrxqippa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ustlhrpy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3hicgkvez.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kmcijqgv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ywxfybrq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kavpneko.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hjfkxaau.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jgidtnva.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tuyytfyg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3skxwwolr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3abeokzjo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vynrdbjt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mgijnjni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixmtliqm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3kgbemkha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izweusmx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3itzdbcbo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3nonxpnfa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ijjrbnif.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fjrieftv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxpyqyl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3enxgoiqs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qdfcaibi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kfsjztec.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rmemiozo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3povmutam.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mojbwyza.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uslaxljr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3asayoymj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fizeziuw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fjrjmajv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nljtymto.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ehwwqukc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pulqfwxs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tihpyzbd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zcjwxsek.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bnvvrgty.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tuuegele.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uhuwerke.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wpsgiiyt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3hzugadig.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vfxiwbrk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3gauizrks.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wsyijjtr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vjwceawd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ufrnrawm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xpfdxrwx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jhhvzubk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tfzdmgop.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cgtaygnb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zrkkwjtk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cxlmzpcx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ceppdfti.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jxxdvwah.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jmeebhpk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvemtrrx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3omipfpvr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrrpoxms.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ribvogjx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nrembtjb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3omvscegp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3sdnyrwnf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3szxxufyw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pqfnwysn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ekdbshzo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hvyvnkno.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qwjnrjgf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hudsunkd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3agmfnips.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cltoqnyk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3elnfihgz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3dumtbuqt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vmbkeivj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ajkjclxc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mpstiuyb.html


<!-- 参考信息 -->