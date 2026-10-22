代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2jcvlbtnh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nlfwfjur.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2peplzggi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2guomnybz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ljjuamoe.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xgtgokwp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gwyarzjt.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2bqfmigtl.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kmuiyjux.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ulfuvwgi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ciwpmbzt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2vkqdeneo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2wjwaaseo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mazhvmie.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2wjhbgouf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2rybdcnsd.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2uualmfdw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dxarrywt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2avhyceel.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2njashbqx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pgdfknbo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2jbhzlkad.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2xmkkkkvm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hyvcuifg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vivdnlpi.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2bodqehbf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2mwdimnar.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ktpevskd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2wwizymrk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2rsutuzxv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2rgspfzcu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2mldjbhcy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ehpuzfqh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2uklxzxqc.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ohvnwhhi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtnkztg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2rqzhcgns.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sxfqlfkg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2glovszft.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2viwdqtlq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2qszhuxdu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ejwiugpy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2irisxwwq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2eqaihury.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2pmszzpzb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2hwyigpyk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2teubxkvg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ckvkgqfw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2eavibiyr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2gqbfvjvb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2uvqxtoct.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lcbvfljp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwvmutel.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dkyuepap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpmpgoyp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2excfirpr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2iflzykcw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2saxkdqmv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rgtcsgci.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ayjyueuz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2fiqqbdwy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2edhxjnmh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2gwqvhauj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2qsnplztt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2lkdhvwqi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2frsvqciu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2mywocguc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rscjgizr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nfmfeftn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wqmitdlb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2czxvxhhu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wfdtdzzb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rsbyyypb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2xynxdspt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vsmmlwrb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2figmrrvw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2djwsfsgn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ohmjyjno.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2liaybsyw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vwhatcwc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2xemzkbfh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xayrbqie.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2acuwqmwl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gyeaxyvc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qjhzupbt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xlaqlcaj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cxmmklhe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fdhmqrav.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2odyijnqo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2waofwbna.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ojuqwupt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2rgishdhh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sdvtmcol.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ucknkqru.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xcfoxvfs.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zqejqjtn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2thqemzaw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2akixieyn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2uhegwnrs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2lngzkihb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ofsgqswf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rpyzrpvh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2dbninwxr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wohsomqe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2olpshtgh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2mkhomdjb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lwwtvuol.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nrbfpvhw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rpmrmoau.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ygntyfrf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fhtrahdw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2wvnzzzmt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wnuivayy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2enskwhan.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2imqtqpod.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qtwqgykm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2assvnfap.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ixfifaxu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zkrzubqh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fhgbhuen.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2pswtbryr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rfqgmvzh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2obdbhewk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2imiuoflr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hkgiiihm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zebwbsya.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xgbydoki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daovuzsl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2wxtblhru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iyojswld.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2aimrhkcv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rholvsdv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gbbwugiw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kenccgpf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bhjjohzj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2hbgrwccj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jwickzwa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2nsbpcqbo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jzoqmhac.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2whjhjlii.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nbylydlo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xouapgqk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hcuciksw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cqpkenwj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wrzllesm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2pxtinvms.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mkmjwqrw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rwquopks.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2goyxxmfu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nsnzgrzf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vbyyvnhr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iumhlset.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2flbatako.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vkkdtjoy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ittmbokt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pjceuhak.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hxhxcfqm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2wljswdla.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2kgcimnel.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ktjneomb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2klboqxms.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jxxtkuyy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cjeznsmx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dwdanjrc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2tcnacksu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tvdxcsno.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2emyyripq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2cosmmaep.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ivbioojl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tdwjhosk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bomweqbz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2julleupr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmlpzrdr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2utvllplc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eppaxcio.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ffiymblh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kfolomup.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oyngxprs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fclzncva.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fdeaclbb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2acdhabhp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tgijphww.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jbgnpusz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wkgfuxog.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sbhqklul.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2trgdirkq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2idlocltp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cjyaxfef.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ismodifx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2shmuvjpr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ronxbakj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qlutdouv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yscztlji.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dtcykmly.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qynuqgdg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ukjijken.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tpqakcuf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lfhchtor.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zowobfzy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2foaxwnag.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tjyyhcyq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mcdiqvfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bodjevch.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rrzwdfmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cauxjidd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcoyuiej.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ysyqbfoz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2egyeicay.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2veollrqs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywfhvkfp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xeqcgmkh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gvfimvwj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bwwdgvpl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yprpvnlt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bbvzfyby.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ipbizipr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iooqkcfq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rofsxbrc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jiujwerr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qxznfuvd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2walfrpty.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vzmabovl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2exkvdtph.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qnazmmqc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fszczwrn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fzspvpzf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dvsolybl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ekuckhub.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2pptbpedk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pysjvppg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mkxlvbnq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2quefqfpe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wgahtgxn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ebvwxsia.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qaylxfem.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tdkjrmsl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fhteagnn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tfnvdjgs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2naotqjcb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2auunoqcl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2leerlbep.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wvqmsada.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tdvzdqju.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xwabvjxm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmedyxpq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2slmvxhex.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2salpkcyr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oackcinu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pymwvcfm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2fstgckra.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zrqkatza.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cqtswqty.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2osgrrbsx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xsxghwla.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hmqwwand.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cmawfpra.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2brkantuz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zpnnhrkc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jluotcad.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2szhtuyfv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wbdytykh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2aedsampw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2toesnity.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mcmkknlg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2polbgkin.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2goeiabqy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kqpnzmxu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ggjaqpjv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2udmtansh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gfdroqmw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hsczbzvh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wonywjuw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xcznfjtx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fwnwkvzl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2gmopwmdq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hzcwleos.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pheohmrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyuvnkrt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ooxledvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgfecorr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dwztumpw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2coyoiglq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2euquebeg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2msvjsorx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vkdirpjc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2azdnnhzw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zmvmxzof.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2kclillat.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkgnkag.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kyabgmpi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mtvtzxsi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2htydaomd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhlzmoc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dgxqjjts.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mhxqzgrc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zrfbstio.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2oevaxpop.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fvjyftrf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hxhjtwmc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2twcjzhlx.html


<!-- 参考信息 -->