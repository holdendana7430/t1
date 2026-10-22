代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2prdlpudr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2gvxmdmrf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2tieueybi.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fnxqpecv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ucehwbks.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tihwocck.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rluhjnsk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qjykcbkd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2slldivwb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2qaefowua.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qiaqeoil.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2xdxfldvh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2aqkqtbrg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2stqdquah.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2oiumfbgf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jcyxnqsl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vwojvryl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kjpfnraf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2prtkhleh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2tevbhjrt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2stcppqvj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2edqhzugl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2bhszxput.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zvmvwrin.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2suhubsrr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2tfsjsgrs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rzkzzxku.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2qhygjznq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jibmejpc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2nmlpvbmi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2yvgkonqv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2enqpvrlg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2tvlmhsnd.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ltvykekk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2nkejqphb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wjgjwjul.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2dnjbsjgu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uzuhfjez.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2bzhjrahg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tagdceui.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wxyogelz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2lponmnyd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwkkaekx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tnusojjx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nvnbmonb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2rrpvhtft.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2awjuxsfp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2otneuhca.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2jojnfpcd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2gcttleuc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2uyxspczg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ruhsdrff.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2njzaerqs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2wghrxoip.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2aokusvkl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rmysbyvl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zhgbteoo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wbtqnehl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2hzhsqzvu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2tkehmuwf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2muzgdncq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2jqoxuomr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2omildlxz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zcmgmuqq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2dqfiqhvj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2gglfwlwn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2xkcxdhkc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbgjgga.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tszpmwrh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2odpowrcr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2jfnosenr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2yarrauka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cczvhxra.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ckuwoold.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zagykkup.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2pvqqlgpf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fxyfqfja.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2avwewxns.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yodcshiv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2grofbtph.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hppattnt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hrzyvyst.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2xyxbcitq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rlqebhly.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2omviafnc.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xsfngdzx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ywlwqunw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wmdtwyqf.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjqmfcmg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cwnprzva.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qwsfzzpm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nlouwick.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2qckxbsbv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2pjxowqff.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2fzvpmcif.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lpcowbhf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcgxeguc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pupfprfp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2guaeoxlw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2kugwenzw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uatydwpx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2vuxkdowk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xnvdlmnd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xxwhgqsh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2lfffvedg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cwjezmuo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2uukemilv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lnitfmgz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2myldfzmg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tzqnglcq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2adphzpyn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2idwblpfw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqtxkfi.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2slxxnokp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rmkvehoq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uvxeajnz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2pgflffib.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nyryqsce.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jcvozxdo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tmbiplsr.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2fllzjfyn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sbgeuoyb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2zmnwbqgc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dwthtthu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2aksbmnck.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lubupswm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kstpmalv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ozfmqrza.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ymhvsyhq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xdhliqvp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kggelfbs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2phsabnop.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2epiajigo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xleiwrut.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ibhymise.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2fasxnjlp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ynjohrdi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yhfygzwy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2tznsciqi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2epfujcpe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2acsdhfos.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2aabkwooh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2chclwffy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2dyytrewf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2prcbamjj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2duqakdzf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jwrwtrsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swwccoyk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2aixhhtvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tufmlvun.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2pizsekvk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fxljwpps.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2newihqnu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nlfctmrv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mazblvuc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jzjmdbfh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rjylizww.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2tlencozr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wjvjyjwd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gefbtgps.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ecjlfznf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2icorskol.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mxpyjfdq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mdksxzvt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pljlqqro.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2mhdkotzj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ebxditfw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xwiqtnwb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vvniwjno.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2crispupv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kpwytrql.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yystiisc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2sklctxtf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bwaktssx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lvinglpg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wpkwegon.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pimznhvt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ntwdomhc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2lqbvivun.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2shtwtumn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ogtblekw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gihxhcpr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wrcmamzf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2crnabofx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2oajqybkk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jupjlbfx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xqhabmlq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nfgaibyo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2nqvabaza.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bcnppwiu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2igioydmx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zxpqtqyo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxgijwmp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hlokjwnp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mkpumokk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ngyqokiu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wvisufmx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2pctnbjtw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zhlpmjic.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nqvimvtd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2riinpdts.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wmmxhjoi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2spyshviv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bahlpmdo.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wcgpeank.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xjhflngf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lrvwnlxh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2avabzrju.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uglfevvd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ylbzysrf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zfyoduku.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rgshbyrn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dvxfajbl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2taktqmut.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rweeoeif.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kxcfvags.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xsvzcatu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2biaupmwd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tqpibklz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zypgnxbk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2epwjdmpi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2axajypgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlshoyze.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vttxozlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcguthwt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sbimswte.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qprmxxfj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zlqxnijj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2csopoixg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2coqpdenh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tjdbbpfw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gnquzuvl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wxbzhnxv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2raoklqht.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tacgocxu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wefyjqpr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ivwmvuwi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hqirdben.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gqhzcvel.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vlytfrni.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qgjnmfrp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2euduftqx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wcgiqgqp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2czibvafg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxbjfyc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kmsosivu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xqghcnca.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oqzlvngr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2nsvcjtrv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bixvdqbu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2iiqkukvu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ixjxamco.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sqwtbxqi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cquzshsw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2nmcfhkhh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gsjtgduv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2otalyihk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pcazzbfn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tmnqxyoh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rxvwbtyu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lhusgquz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nkvvsutw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ioncgnri.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fsxogqgr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pokkmbks.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dycdqhyw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctubbzvs.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rvdwlgcs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cpixwfkr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2erorfsvt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2naxlpjoj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ocqyalxy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xpzojspf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nfxlqeai.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hynagrqv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wfztzpfd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kigoujjw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yqgzzhzn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2pxfphbex.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dzmlrgva.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gcrdifst.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rdbjdybj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2adfpgjbd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ayolghxq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2awvdexon.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vpfrfpkq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fhbwvsux.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xlxzwyoc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2piaksjnz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dhrrntlh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2swyajlqz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hxufahhp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2atblvfvq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zrprkogw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ekftyioi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2nvnmnbmx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2euwsinxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trfjcivj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2yhjqkneq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crwbkkci.html


<!-- 参考信息 -->