代发 wailian999

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3vtpdpfed.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3tkljfqmp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3xctddmip.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xfiyodii.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qqdhqkjk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3lnpenkvg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3htkpuljf.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3lvyvzzlk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3krlvirzf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3eecesmvi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3kwbxbinu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fjzojkoy.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ysnpyvzb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3wzepiujc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3puxfouue.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kucuijco.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fsdiivdd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dtasuzqq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3eoaaheli.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xotwdagc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mclvhswz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ikzsiwwh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3opyygjar.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3hztlfkvu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ctzifrkw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3fmneeaia.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jyuchqtl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ijaetkyu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ftmpblgw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3nyrpekbs.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3jwyxgctm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3lvuaaldw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3pixcreas.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bfcadydq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kefagrkl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ggtpmiod.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3knnjygnn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3rjqenxed.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3syzqpgyf.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3nqkifypi.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mwijelnp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3adqqdaxp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3mmhzhzjs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3btuajesv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3jamtnxeb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3njrfhknr.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3bfohmhua.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3fhghrvme.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3njsmtxvv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fymsybdp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3jgrierug.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fnapofch.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3vyummypo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3hwkrlzbj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3mvswdhvj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fdxamkrg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sfxoprrt.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3iphvcagu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3nrlgofmo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3recxyutl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3tdwhnpwn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3efecqoru.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3pufwqrmb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3aallflwy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3sdhvticr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3cfglkgxp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mzsdfifs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3yvagbxsm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3nifwxpfv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xafupedg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ewowsmvo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3eduwgjem.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3zwynazkt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3vrjjskpv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3kttvypzz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3qpdvygqu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3yovfeswp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3otehyyyn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3vxzmimdl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3evvllrwy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3poubcmuf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3uzfzqqsa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3zotnefrq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wizqwcxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdfppofr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3htammnhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwmnwnon.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3iengdwok.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3frehkvjg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qpdttwog.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3njpuoqoi.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwzyuwn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3jmkgxeux.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3nziyrzwu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3yclqisrj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lxqxgzgh.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pmpcugay.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3thutuqae.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3rrvncjui.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3awwvtyol.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxixprk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fjbidgto.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3yyibcrew.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrjtksak.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3csxudxnt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3wlojvskr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3leipcdaf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zcpybnit.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bftpedzh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uzjrbetw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ryzbygir.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hqatwzvi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzhkjgr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dlkmtiep.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nshaqepr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3msifacpl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3yacjriba.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3yvludppo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tiyukyse.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ksvexuqj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gsgehbse.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gnyhwqkm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffxqutqv.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3cgqhwhxe.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yhrhljxm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ypghdcol.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3chcusnrj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zzigxzwf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ydyphosv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3qwkbdsux.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3pnxkjnho.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3veqnaxzb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3sfxvwbeu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3guptztcv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wwkibcwb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ydnqeiai.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vbzggueu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qkmvzovf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3daqudxxh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mihwtdea.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kcsjopoz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3riiuacvi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ogngyicq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3rodeqxuz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hiywbgro.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3upytzipx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zqxvzkdv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3dftkgdol.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3acgaekac.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwfycnw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hlopilqw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xgzbjkdg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3xpyenoxj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3aqapgtja.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qgfoeora.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3cwcbamww.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gswpznbf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3akgwjdbl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ygwypmbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvsqnwsg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3grwljzde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyghzkns.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gxcpdlqy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3uocuufdo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3jcevhsoo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wddqaerp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3khtoeusk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3hbrtkdce.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yfubxyrx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wyaxgyeg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3teeyxlzl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3unezlhke.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fzqpxzuf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3oggcqbni.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3anoitepk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tmargypl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3sxvatybq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jnkbbyod.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pudwelna.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bhrhkarm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3cxcxejzv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3gdrvsuhk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3trnavkbm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pillkkyh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xuuskkwm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3acxkghgc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pxbjyvqn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3inkoixjl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rfhvmmrs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lhocayjv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbvumla.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3nwitdekg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3npgfpltm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wolrrfrl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zvtozqcf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3lriegsky.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ktnnzvyl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3erteptsl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3wufojsvf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qzogpema.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3bxwkwxhi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3iihaohxm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nwkfdefn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xfuagxyh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3clzpjfli.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3tercvkfl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tfhlbxaf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xxlhhdqr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3varsyoig.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3szzpbtfq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3znubnema.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zqgrtawd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzvepuw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3kwkwrcym.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kgnjhnos.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3kzzktqwn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bxawmohg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3pcuwltwe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3elfcfxdh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lcmzezuc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bousplcb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3sqphdwun.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ajcvtnym.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wtahfauv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qbqxoxja.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3heqaojtx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hslftttg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vxeikusj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3omxvsesk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ooduxdsq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3oqzvgqeg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3objduvyy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wpkfvttd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mhjbmacy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rycjkzsh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pdqscqsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfrfikig.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dlujvqpu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qjctumum.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bazylumg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tfyunbog.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3shxgkkmv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3grhsidnr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3owhwothk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jjgwopei.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rojsezbx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3crvmcbmv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lescvfjp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xfkaopdx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nxbhqnei.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bosbedep.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rfjkdrzh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ycvlnaen.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3qbzpchjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cofnkzfe.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3yqsxhsdo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xksqihiw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pdqkruix.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mwliwyhf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gszxjvso.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3myjmjuas.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3blgspjvl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ootzmcpt.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zhzwqdei.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bbbdjaem.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fopcqfjp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nlnbgpwy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nimybqlv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mhdkaovr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hpdwipjp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zfhtwvsh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ydpwoszw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3npzurpaa.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ryrsnavv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3akhtjmcc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3slxxkwwz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lldayftc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hztmdrlq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytorzufn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hlwcltlh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nccwlbfl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3jhzsoghg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mzeokzmn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zchgpumy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ekpavfub.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xohmipmw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gbfytvti.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lpbcadzx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3thahmxwj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3aovyerlb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gjdmndin.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cvolwprt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pazuwxba.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vrxvkhkb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3seliiaab.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qnciruqi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hjotleux.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lbejelzu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3usdmzuyl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3evyguhpc.html


<!-- 参考信息 -->