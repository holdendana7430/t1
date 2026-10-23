代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3rbfxzwvx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jcytcvsp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hpcanfyf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3thtzhbmk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tkqbkdct.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3dcsqyhhl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3yqppfnme.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3obcndgen.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3awvorord.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3npmvjyei.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3pvjooeaw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ptuckfld.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3plvujkbr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3mkravdtf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3onietbjz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3pczwbpnc.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3bhpvxlpo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3shastqzn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3pinoxqry.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mwakovhx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3apsnflcj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkgriptk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltcrqyrc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nvobtqkd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ltzbwufj.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3lvqubnza.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3juqgxjbl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3yxeofmfi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3lberbaag.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3pfhspwrb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3esazyyst.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3uwqmgyqw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3nfxlglss.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3jhewislv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3uawmgycr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3nuduggmp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3lagbwjqe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtxexbi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3miegeoux.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3rabldhmt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3zbyiiaxr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ihnfpbqc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3iahgosij.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ipunkltw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ehsmntvm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3jqvlibdl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3vgrizzmz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wwjsrckj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwnhaygr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3lksndyoq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3tlqlbyyn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dynxximj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcdnhlut.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3vfpotcrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfcnogtu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lqrnftbv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cbofguyr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fcnouphf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lwukzwyr.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3womztqay.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3fjsrwjyc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3kofplphc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3nuvtqcoq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dpmxbxhm.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ftrzvpcl.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ksiffulm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3tklmsdus.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggsvtprd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tgcorphl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jawzpksu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gcffdezw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mctezftx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3quopqklg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3vlxjkopv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3svdcerwa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jlgxeywp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cwsilhlc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmeoszbg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3meqsumkq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3rbutzjjo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3dlcbozis.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3wuxxoulp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3itidcipt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tqnybplg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3vodtmzlu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nyyewmon.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3uacyqbfy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nvzkgwkl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bsnkveiy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gcwctdvk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3imytnayb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3gcjnxqad.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fzrcmesw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3wxidxapv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zwmtueji.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uazokxxy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ckxrdnvz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hyrydmht.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3yuchhivh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lynporml.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3rcryoboa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jozalwrg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vnjewmsw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uqvphnjs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pjeosyqx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qifkcnpf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eskaqwvz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wflcmled.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3edcdfwnu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3xlwlgofi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3trddtuoo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xulqelsq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zziaqocf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vgqffdne.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ppzujdzd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ainfsutf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3tqkefkvl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xsaflzse.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3tmumavft.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mcbyhtbd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pxmlvnsd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wjcrwyhz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wovhgiub.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3glwimhue.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3bfkmkkal.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kwzexggo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3amdyzizh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbplitlb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kptmxfms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joorcggo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3lkwxkwsa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3lmocdrsb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kfrwvtmi.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3axdhkbml.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zpfvresb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ozcdgcsg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wdvqodli.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3zvhwcxqa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ixdtusxo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ywmkwcrc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cqzownzd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3zsitjmnw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3onotlrqz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uiiholxs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rlxelwfh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3alcxqylu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ocnaxqgx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fzdpumxm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3keuroizq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3prupfndx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3dsedacff.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xgiwexqp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hddxvigt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qsrtfcah.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3luqazcsu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3pteycchc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rmqookbl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hbpdirmq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3eqrtsvbs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vqsdebqz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3frtxdahq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3npcwcwwo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qapuqhla.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3htuwihyz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3edkixasg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3aarlhfmn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ydjkkhqu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fnluygpb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qzrqmfrs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pjaxjhqb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wrpcbmrj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3lxumsmom.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qdemxosm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nflvrjpk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wmtzqnkt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gtxjzisu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jhdtrhxy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3didnidrt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rlkumixx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mdcrcylm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3twlchras.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3izhrtbrp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3pdodkkxc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gukberzt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qoemmmws.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3bhxhhbyk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pvnhwtsk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hsyxthop.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qobqrknw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3twzkizlh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ptfnzbgw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3eaborjos.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mixhetqg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vggkujyw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kwiuykny.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3tpipzdrg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3saapdywz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ybkgnqca.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mxvfzfcb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3iwgtcyzt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zkzvtysb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bbhbcojz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyovvcbz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ydgvntvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvdiibit.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ctfghyua.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fcalhmxf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nzxowaxu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jhtzqisz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmsrqmyi.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3oobotlzd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mikkkqkl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jpbfdemn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fsdzxozj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pfbnygxg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3egsfjuem.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lxgmkzpm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zziavzyr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sdfuxekp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pmgqsvov.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jseihixw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pzqjyxre.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xfafqxgm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3nwbydnsw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3puysmsxj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pjsdalfq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3knxgpnpa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gdnefexj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3usxasezs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3adqyjoqg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jckocfmv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jaizglcu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kzhyozsp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pwxrszik.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pjpcbdcr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ekpzzxqs.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rcfdnqwl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mknfhecq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ovllbutg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ygcdjjie.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rvcmfskr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zogxfkbw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glotnbhu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hrwdhuzi.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxhxuilr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vfumrtky.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bkwzroxh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uimmdadh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lqmqzduz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bnjlnmjh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gnvdcxlv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3roamainf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fylncnbh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jpjcricq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zcddqdbk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dsirjepn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ylsfsfyn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vealwkbo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lzjzexld.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dcaeujuo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qynupppy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zfvyecqt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tqjmcpko.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tcwzjkly.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sjgtxuvm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pcdqcrep.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wvoleing.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ujwuyifh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zuymkaee.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tydsyuvf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3iukporxn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lpybekum.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rlestoow.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lymhwbuf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3msmbymrs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sriwamod.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lfollfcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3innnesrp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3elisthqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjbuzsyj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pcfkftiv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zgwlbtfe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wjxzozgk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xhjiuhpe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nvfyfzko.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyoklmcn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yidktxfw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3dasmball.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgkajoue.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3lvqokjcf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3swocualk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wtqoelzw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vxolvxoa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cgduuehf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qjcnogir.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3giaviwhv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gfzohmpl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dowrjxel.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dcjftrqd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vfnqerkb.html


<!-- 参考信息 -->