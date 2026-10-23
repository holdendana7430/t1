代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3bxvskhhc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vftfzobr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ojtwaptw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3nxzidini.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3avpeyxqy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3fnpjoniz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kdvrkfjz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3twbiitjg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mtxfkcpl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3afxjnxtt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3gwmncmnu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yiaoydmr.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bdaknhvv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ijyvorgg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wsapplpp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lpliordy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3fonqqtce.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3oqefzvud.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jueesvlk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3mpaajlnw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nefrmjcf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nchuisyi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3falpildt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3uzshtsyf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lvugvvib.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qacsfbfu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3dsrjlism.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3gvdboxfa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3bhzeaicb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ofwmuqcp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3iksgosop.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3mdwnxyyx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ukxhjwym.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ngdnziqw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kihdnycv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3dtrrsabg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3uljjtalh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3qxonnbgb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3qakowdvg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3lvwivovu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3inawbvss.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3maetdgeq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3oaukezdc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3uiarxvou.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3uvlqqfwg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kyabptha.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3eucmucyh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3pvnutuux.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3wsxrabwu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3fhvqkgzy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kopfqzuj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ozlrqnnr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ckczkwjk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3yxdqbkzs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3hdksosun.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3kkiptsdn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3anfouanh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3xeuvoaoo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3kohuanbt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3qqywjqjh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3sdlyxmfy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3hvfkacoc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3nhklfuna.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3pjvnuqdb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ztxbbozh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3pntwpvvv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wyjasovr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3niuwanmj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3tsstcipf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3nlthijiw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3lnghjzom.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3mepukoij.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3asxibhsz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3jitvtokq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgivoud.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qjzdehve.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtworkas.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3plcuvdpp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3cmesturz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgrntacd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdabhktw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3gdrgrtvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvprkcmb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnprvxfr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ntdhwpyl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sfutkmfg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3khpudddn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tsxfkoem.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zcqvguxe.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ddmvprxa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3gznbafnf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ajlwizlb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ucyiatog.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dibhgrch.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3gflcadst.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eylsvnwo.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3aqxczbyx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qivupvcn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3fblaqpwv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3spzetndo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3uiuabhwz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3dlxnigzs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3tleijzrn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yemklmlw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sgypjjyy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sbppsfbc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3whdelced.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3wtnayoau.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3wgwsshpn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3aejvnmdr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3eipexxpp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rvfmsaxv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3arnwkdjn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mzjpinvm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zoxzvqox.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kdjanzqz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vksxqvih.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wyexgxvc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hxvymgbh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ybjzzoix.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dutlsjia.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3yhgrqiak.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufzfzave.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vdrlcust.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3fnksawxu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3mbvkdnqw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3wqpkzqqg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3fnjsmlfh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ziiclpft.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3elnxcccj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wtnxpgqc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wbnlxrwr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3blbkjraa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3dagvvylw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jswauvzo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tetblflj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wmfgbtdd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3mbelyiiy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qpklvzfc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fxdfmlgp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vrthwair.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jnqwcwsm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vyhprapd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3dzopnryq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xuipiuia.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3calksmub.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3kxfxuffk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3azvmzgeo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mqsrbtql.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rzgrzvcf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kglwidhi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3lbqhoqji.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qqpsnvmb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3asqxxktu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rsldqlnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsxnowhn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3uiixnrdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lttajbzq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uqokxewx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qfxmxhaz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3mbsjuqlg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xocbtvtg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ltslgvgv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dviqdvhd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eywwwzul.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3eonowimy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hjspymjb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3oehgclrz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pwjhzvzq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3sjwlpnbp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kzdbamtw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3teisidxr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3oayvidlz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bkeqtkyz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zkuzfako.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yrnzuqiy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3xvnemafw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3woxqsont.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rcjpzqam.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3llsrblmm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uxqiirmw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tohafzlc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ilntnaax.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3pxcccblu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lzzevjot.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nzkuaeis.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hhxlvksy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tgtwzgqe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mgqiqynx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qpdykfxy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bdqokavx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ioluwfbf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3nvbxiuxo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xeypsnxs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3annafxbt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ducmvhaj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3tobmvolr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bqctzjop.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3skxlymie.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3npjmuyfe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3pervkmqt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3abprixmz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xwohoqpd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rsanneog.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ffkhjnhp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bjkbijkv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3liipmaod.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3npfvvezn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rzgimknq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wpkdklin.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lgcpkmsb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jsqmpeef.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xjnjzkog.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gkeqvzdy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ypgumepj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ahirhcov.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hezbrrbu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pmrwocwg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nuoszynb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3oplpqbti.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wykvbnea.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ubgzgnib.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3lffmrlsn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wlbjuwkk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jehoxcqk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ngwuxgzj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vdxkausd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ruxizkvd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vdulhhqg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wqhsiqky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkvyfvla.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lmjtwdgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsbjeqqh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pfghffez.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hhhmnffz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pkwdwnwu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mmjcyjqk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhbdocqd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tpnmgaof.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3aywycpxe.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ejmfoplk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wbhvjzba.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ogqvrnwe.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3haysiqrq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pffjqksa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ijlakund.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3uaxwimkl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sofheeyz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3odxztpps.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3weqoeuof.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fojoudpx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cyentunx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wwaskdwv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wbxscfea.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oylmqurt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vvhpoovs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vipkuyqq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kgofkvqm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ovooisrb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3luudopxo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xdmidwfl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3cmqbqswd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3djtgyavg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qdgcqfmp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oeookenp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bltwjbjl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iotzieto.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jkqqxmkl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3blafijvn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3oxgbveop.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ddkunbij.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zrgdnxqu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tvrnvrqh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3etkayjka.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ovbkrxzz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3irfasaci.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpxbszsw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dpvsxtyz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3chtpyrda.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fiumudgp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jzdrjwtx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qjbyuwqy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fvglyiqv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wzipqhax.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qrgvcfvv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vxhrxsrl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3doxocfmn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mldodhij.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gkzxytwl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cggdleeu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3urqbjvvd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zdfravlj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tevsllbv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kttqcwuv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3mdwjwcxo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mrgqbeop.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gnygkezi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lysfsrja.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3xqicvpkf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3itptcwix.html


<!-- 参考信息 -->