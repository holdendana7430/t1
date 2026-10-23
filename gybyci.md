代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3qkukwlvq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wwssxdww.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jzaemqwf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3utusryvj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3hfblccwi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zynhjjjp.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3elqwloex.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3aesovgdm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3jshjzhpp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xmtbitip.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lpdapyjs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hlqzppqd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3htoqhnmz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3buipnuru.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3lbdddsdo.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3vldfnlmr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3szbgrxcg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3odqiedvb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zybdawap.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3esgakcdk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3cznsetfh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3lmxlueke.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3gzcuobko.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3mveykgde.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3nswhxosr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rvybstix.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kmpzffdm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3khupycrw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3scgyasnd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvsdumxe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3czctaubl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fpgdxfxg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hgyolhlj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3omfnfptt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3mhbklojp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ktxosnyq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3libcfhjo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3kynvsovi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3qvdiscgt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3hcqubtqh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3cytgfuqf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3btlvfoap.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3usggnouu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3gzrdkqyg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3vlcszuio.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gidnhvmr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3dcbsucrx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gsxztyeo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhahimx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3mupqiajl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3zzmcbroz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3yqpddkmg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3afesypny.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3yoldufib.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3wgjqbbqg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eeboesfm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vexxmukr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3pddgoolo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3dpwmoxas.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwzzaca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szriaubc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3lcugkdgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bskzwsla.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qbtrfybw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3unanzbll.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bhizauyu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ysadrogh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hzjtdozh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3cpaypysn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3bbvugtxp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3vupztmcj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3xnjgqpij.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3wnkbwscs.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3avqolyye.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3wyvzcxho.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pkzinfrd.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wahcndav.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fbbnsesq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxispge.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ocpniitv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3namublfl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3sxoauckn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpttmgk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pfamildh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqeoiyot.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dystanbc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ujseyojy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3lzznyfzj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3adlbwdjs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3emucpzzf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3gfifiget.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yjurlkme.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3sgsbyzfy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pmwkvdfk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3evxwyqpb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bdhwmpft.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3feqrpfln.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pstyqlhr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rcvbovfc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3vrjkojwu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3virmexop.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3rpnvdcma.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fnxwppya.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ifdixkim.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3yiiqcvqi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kgwjbbfq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fvsheuyx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3dtkoqcjz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3jupgutps.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mgohlkun.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3gliocsky.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dplzopwg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hkuirsoc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cekkkjhq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gheaysnt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ddqisbho.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vbvpvaip.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bnqjjxyt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lyamqxqo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hojueuxi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jevhnywu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ozvwcqea.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nmeuwqpg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3vnneipsm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lmcuatma.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nvssiptk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3abhhfkou.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gaiqewyc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3stxmwuyd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xyqwjure.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kkomzaml.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vdsyfebd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fckgzyvv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wgnmmhla.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3iqwgtcrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zffxlkxl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zaynbehf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjazxmya.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3kruslkwy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3gnkmzkjd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3fchmgaer.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qzxprwse.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3czfacaan.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dvxefnqv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vatomaye.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ynozzmoo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oopukrbj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xmomwwxu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ibtygbgc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3hzggdexj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ffgoaply.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ximvtucx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3xyxymhmc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3gkvretzr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jyatqvvt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kdjvbbja.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3sjkxexsx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3rbahwfwj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3xvjiwlqi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hvyjrcym.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3yzmntgan.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qzjztozs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3prebmgrb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hjafzvdj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3niruxelp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3yhoxpddn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3iiylsexe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ejgnuqav.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xgnxbqst.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tmonykxl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3prosfpls.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bttssfgr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bqhmxrxp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bcazgnsz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3konbkjjm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lrunqmvn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vlxxirih.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ozzhilqe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kzighjlp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3bjkbccdg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3prviyqbn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3tqpewidt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gjiwcuqh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3phozvuau.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3onbauiik.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xygqlycy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3upfxeeqo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hjntgazh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hfsvtquq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rifupkxn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3llchjjlj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3genyivag.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hefgujkj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bqzqpnrl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ncezpklm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xbwtrnvv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vbpcxxhg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vsdatvey.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cskwfucf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3cbxbcmsi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sgnhogzk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ullbnlrv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ftzxsnso.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cbxbizad.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hdotqggt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vhqvlbru.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wdrrdzuc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3iwwalthy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pdumfdrs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lnfwsgqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byuyujsr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gwtihnjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igyylzeb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zcpwxnnr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ikifjatd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3deyrlkst.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tghiruno.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbwekdhn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kywprfau.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rdiugqnk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mrlndqcy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ivwksuvq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3waxjtmbp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fnmsmbnm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jihpwfnx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xnxpfjdo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qgvwgjzi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gdyqprqp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kfzvhwas.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3llpeuawh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iketfezw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xethplfk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sniftxee.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lxbrupeh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zbustiib.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3frmplzcn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mugiccre.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cogccwdk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lqkalbny.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3uclkvmuv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bpxqkrcq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bmeganjo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kmsylwss.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ufjgiuoz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pygsnwfo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pwpfzcsh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dxodfkgj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3komsdonv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cbwdbpgu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rqzbzaan.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rgnfbipz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fvwbxwcw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlrnacad.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wtkkwbom.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghblzfkb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqzqwbwc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3aeplmvbr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hvnayiyn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3omewhlnp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wcjgidmt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3oealvczc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zwtojqhb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fvqrsore.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cctfdxqx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pooebsru.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hjhnzvmo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vhpkazny.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jthhglut.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3juayrxbb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3bgbahdwt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vydduozv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wzcvgkqf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eringhkp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3iwbeobsc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ngjsoytl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xadknjzj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zpzzidrs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vhlgkskw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3bmwgwyoz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gcddlxnt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cehatyhj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ipktraha.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tdzzgjzg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hbjdfirh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xfbyuocf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzghakui.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mmhbbeqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vysbhggk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ulsugrzf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eocbluax.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rvhweqls.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ktoshokg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxkmvtx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ziwipdrv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xihkzbzy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jynhkhpk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nznfoqqr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mxyeoqnb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fnydksya.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3upsgkifa.html


<!-- 参考信息 -->