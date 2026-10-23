代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ahunbkxv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kwjqshce.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wjmtocvb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3rcsrspdu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ajnuuuyc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3zittrbcn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3aylggpuf.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3dmorboaz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3miqzjnlh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3eyemqdxs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3refaasrk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3imykmmqh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3bwkeqxzm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3sdapnfov.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ubjqnmvc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3apsaunxw.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3nehpetih.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xjfcagxi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ibuuizaa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bjueiwdw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qspqiqfe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3pisogkuf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3hajlhyre.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qcairkrd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nkhqznfi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zvggrfqg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3dbnchlzd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3gdytxlow.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ngerdasj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3cjimvfkd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3nouespss.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3aotjzlwg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3mygemnxm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3hqyofevy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ebblbtks.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3yfsicgfe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3xsofpmsx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3frtnwrto.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cqnfzlaw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3wrkejvum.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3zqzzvqwf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3fgcljlsv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3dctuixsh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3zmaetgfw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcljfbm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3xshlfwxh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3afrzzqds.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3khotyhdv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3nauqgcst.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3yoowdjfo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3bsqkaxul.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3dyqartcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xesguzin.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3wzxuvwsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyldhfxw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3xvcafhrc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uaexdwks.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uchozrng.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hsrbanwn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btylynxr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ktgxpexw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbpsjgs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3mlwkdmkl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ynueinjh.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3fmlpemvk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3orsfcysa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qbdycsxr.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zuuyttdz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hvspsbve.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sgrkbzgv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zfseibmb.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rbrmhhwi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3qkesjwtk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3qhyojkfj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3kkzgwtco.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cwairpca.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjallkro.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnvzadl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pyvdtgqk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qyttjiek.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kclnptvg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3khurutfh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3rsvcvlhe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ntlbfqza.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3afmvdaoi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kscvrknh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bsldpfvj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3liwsoaaq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kgcvgivi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vrrqufqq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yfnafoof.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3sfbxxiqm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qwfudbqa.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3iwabdoby.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btyoydlk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3subpwfng.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3cevdloam.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rtbhxemt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ttydmyry.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3iquhnllf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3aimmlozz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hhtmvuhb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3oibzxvrm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xmrrvmjg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cqgjukko.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lbdfzqfs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fywmvnvi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mhsvjkrc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wjneuadc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hpxmqrhz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ybacxkqd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3lwmnjjij.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rhnytbnv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yrvftgei.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3doifxwzo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kzklvcua.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3zslhwlme.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eaezhwet.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xfxgzsfm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zedeqejy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3inbjxeuk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gjnakqqg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3htbipyuv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ogiswasl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3crayyocw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nflkvikj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nkwcjkye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpxcgypp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3dqjrfasa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmzvhzxs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3wxsqavdr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hbvgatrw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3aktmzyae.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vvletjwc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3npbvhvtb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mivyytui.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hecxfebr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3sbpcnobi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uusctrih.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3doaxipkf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xlmjkqam.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vfhhtrbv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ybkgutmf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3enlefdgo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hbwhhjiv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3cvtkaddt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3hqgvgirn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rwtgjsit.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3crsqjuzm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bygdubti.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fljiszya.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3svhauemw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rqhwzotl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3lwigtmro.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xpikvwbt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3inciltpf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rpkgdepk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3oiwzlrac.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ttmcameq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fthnqrio.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tuioupff.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jkpozuzv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cabqkqsx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3dctohwlo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3atecsjys.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zaxeftse.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jvuzqdhs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3gankjyzs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lzhhdzar.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ekzpaxmz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mfswomdp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3zftukger.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kyxaunzl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jaudzpzy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nxmfwmav.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wxnkerbw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qojnxrgs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kkiwozcy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mroocbsh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bqkoleqf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zcvdfjqu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wqmbrhju.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3plvdekff.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3umkvvdxk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zrfmozlo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3qkpowost.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wltrxeny.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eaaavxnl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3naznuedz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3aaiwpoad.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vkvkxkcp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gvxueebn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ggloqdle.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3avejrldf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zsddyabn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wqyzleix.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tnpvwubz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ccjwswzp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ckdxwdup.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3zxyijqcu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cbuanczk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hdpkdvne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggfgolcq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rmkjpifq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsguebst.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fknwuuwg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wlurumys.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3lrxuqlmb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3foaizhqw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3guxbgihx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ghonvldk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3idqidbfd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ugsmmwty.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gfijetkd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvzmsark.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kkjbxcjb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tnoifods.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3apbgijmb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hetedvzq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zzrrqfxs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cgjuerti.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rqdjxrzv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dkjbgnyq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3exbjcqcq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ovfhqybx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3joppjnjb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ttnvcpii.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nnxkcwnp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bqrznehl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3iswultny.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3lfmptdvu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3axbihfbq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nzsryaom.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wvexrjcy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pbcjeqcr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pxusgtry.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mevphfpw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jgethdav.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3biluokza.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3utklnqge.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kcihtqiv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3majmmsrz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sfxtoaji.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zldiyfgu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iujcbsjp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3povlwzij.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvncdfmn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tgljgqjc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xxsdfled.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zmbtboyk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ufhmkcmr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wdgkeckp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ccvvsuep.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zsuvjfrh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ukugsvrn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yoaqjsvj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3sxaymtaz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pdguqsxr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rcrdvoum.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3vxwkdlfn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3uojmpzzn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uepktkhm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mkycbejd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rtbdcxhd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxzzrje.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rmwfghfe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jsqxbbnt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vjsfwzmz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3eaqetrli.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jbdomyjk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bjwwjcac.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iijzrgvt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tjplwmib.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pncbbdpr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bdajwjus.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ohqgtyxg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vhsrljxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csauqopi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pagyzirn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nafnbvgp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3whqiiryn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dydsfhjc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3isxtvacw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3luivtnue.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zbsdkrfa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dfjsedet.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uwdjmwbq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3oxsovyyu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vlsfymmp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rkhualkl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ghnmlelw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rhadfiwq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lzchtzcn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fcqibgdy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jklijqsk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ucrbnssw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zzvwhhhw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vnezlfvo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lbqhsnfe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wzwrgdlt.html


<!-- 参考信息 -->