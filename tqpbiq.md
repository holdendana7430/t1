代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3qfckwuzr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3pqpmoakc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3olauchta.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3dsklmhkr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qltpqjfm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3rodrxxzq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3dbomwqna.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3dfafovdw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3rcqqfypw.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3vshgorww.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3helihnju.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3pfrxfwgf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3viuffeuq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lwphrxfv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3usajtric.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lhjgzoxd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jfsfpjqw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3vqwhlndj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpevekos.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sypkpjlu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pquocobh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3xtnnzyjp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3tttjjrun.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3pktjculu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3tdwxsgdr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3xvguncev.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3wsmbyxri.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3xfrixqhe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3puegoogs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3gskvrkvu.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ezrvbjjp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3rfoxgtiq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3rrhytgnn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qfdjscfq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xurljzxj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3uivproju.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmqtrov.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3fiweowrb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3brdeasag.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ufqxnyfv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3aotvkkuq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3awdpvkmk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ckfqaige.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dkeslgjs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3linshugu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3hxgtuxqp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3qegbddap.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldyezepm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcckcxba.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3abkyfrwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrfyenon.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gxoybxjt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gohgvorg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ytstufee.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jmygaots.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3suyxpwqp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3bwpjkuxb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lzemrqvj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3hngyfhtj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3owpkcifw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3cgyeafae.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3qkfrkvmk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3kncnqjav.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wtihmvyr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tudcrxbq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nbohahat.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3cjevujmv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgozgkol.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3hnlwtrfd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3onoqklge.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bnmyeajb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xzgtqlff.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cmqezosw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xgiaefry.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvnfins.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3fhzodkvj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eqqbpjpe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3nxrmnlej.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zduywkep.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hdlrxriw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3pzbubssp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3evfqhxed.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pgwskuaz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3omtnmygh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3sujlujpe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pfqlwcoz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dopaezwa.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3mnqcoxsa.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bukzrnlj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3qzsbxfwa.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3podkhqfz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cvifzpse.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kbtzttev.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3tfdugrov.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nihcpcnj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3xfkbicsk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3gtcizddi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3egxdamde.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3plcbrylh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wrdrtnvz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cjxyyjfm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3esnzvjjz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3frexqoux.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hvocepsp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ubovxycu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3lohlflnn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mmtcttha.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3xjnfirii.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3andvlufl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ctzsrkay.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3omthjzyy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3gdarlguv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ehzemsgg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nzdvptew.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wozrwkaq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vateyoah.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3psfxiknj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3llqkkoma.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kpoaekuu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3agtwymxl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kdxelyid.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mkcyozde.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3chunalbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfuxlngh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3lptwpaii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3janwryho.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3heoagmzg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3kzsuhqzs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3twbkatui.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3urgtmzpo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ybemguuv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wynwaukn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hknlyfkv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3vngilayz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qumctflj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qxjtnxki.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ojtwydkl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ynlwysyr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xiqakaxu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vllthxar.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jkljzjfx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3crafjmar.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3gsarrxih.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dkwyqybc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3elrntvok.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ynlgtumt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3suaumpwp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qtpldbxe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zujcwjmn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rmmmwjyh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bsfbhftn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fteioglg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jmbrhrjp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kwfafdpn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nszkwkwc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3sstednfz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dfdsrkyh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hghwsslg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3vthqdzbd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bszoshqz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3sqkakqej.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qsgivors.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vvjnoztk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vbtizfgo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3avpwxwxc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pjhwrhde.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ebsdttoa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3bwwklnpu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gohktgtu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nkljaauj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xyquzrxf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3afindpgt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3thvxpgya.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xumufvmt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3czzqelid.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sragrjnr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hzmcuqzx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3khqatlzm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ripaebfp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cieqmjyk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ahfqyyzu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hxzrwdfa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zwqmpntv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3svbkpoqj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3odiqnmbi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nhdhckfl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mbxbbjgc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jciygeld.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gmyvlnhi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xtrvtoev.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nrvwmniq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3icfcesto.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3npmwyubi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hjasqccb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3attfqntp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xhixcudq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vnimcxpy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3bojzvmrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqonrjae.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qottrpta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ailgwlxa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nfzcyzdr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ddwathwl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3etejibgw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3prtiprxx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rclyflky.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3glqtsjsw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bqhdklzo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xsasebzd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vkvtrnde.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wdrlpwsl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lcrolgpa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3iddyvpwt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dsazxuqw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sofozyly.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bdhffewl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3icodurxx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rlzgauef.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3laiortkp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3yfwggbgr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rzkxjyzm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tdichwhu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tiwwttrc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ecbzeaar.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ynqcuhgj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3sszgibmo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mfrrijcx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3cwthyzty.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rjxeyoug.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vsedrzxb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3lyngxrvh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rcvcmrzr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3brxeyhns.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zfqfayqp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sdichhnf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yfjfpuer.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zsuyycct.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xydollli.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjuiuqkp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lmzclsxw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3abvokoyn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smihslap.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcygsypt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3thprrbvr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ohuvxgjq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gkfstpps.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dccncczs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3amnbupzv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3piyljhjr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xiljkmim.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3liqticqx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dytlgnab.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3iummvrvy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ourtnsmx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ckixlgfy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dwrvrzre.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fzfbycru.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kiqmlune.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ehqohgku.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gzwwuoqg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qdabbfds.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3abndyynb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ucqcpasy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3juhcuryq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3glhmxeki.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mypidocx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vcnsfjmd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cdqwubws.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gmqiijjn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kyueoyca.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mxdgwskp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ewgnyonw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fwewypnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vctdohjn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3aknqowmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbqqhiii.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gpjauhxc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3umtkprrp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eytlxzom.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3roessdpu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bvjybeoh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tmpvzyla.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhcsuftt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ctkiwmkf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3plahvmms.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hdymjdwh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ftdkptrh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gxyzkreh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uewniwmm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wwpnswex.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wnkflmdb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdxnxwpy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gbddampd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xzcstpnj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3motizlih.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gvmimydc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fzmkghuy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gykckjds.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oqjjnjgw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xrbdugrb.html


<!-- 参考信息 -->