代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3onfweuaa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3zgjwzrbq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3aauicjco.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3dqgntjki.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3sqezagsi.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3okftsheg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hlogmwmr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3iwrjwkew.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3avlocktt.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3tgmsmzjo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ovclxtzt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3tvalmihi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3takmlkrw.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3yflbbshj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3agosurin.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3cvtbgrjw.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3yxgenlhp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zfmvwvjc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xaijaecq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wxxqtulr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xcuxcifx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3bowpqzbu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fyqvhmdg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mwuzszls.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gxtnmqck.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3otpmtihh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ybebjbws.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3cccczqjk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3lheuqldy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3crkriipc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3zwjwqpjj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ymqgjgeg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3qffehhxv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3tgfyvpvi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3fjlomgbu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzoykrd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3uzizfjlw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vbfvyyfm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jgowrybi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3cgvomqwy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ncfmdnfv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ljinvvjl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ylfebisx.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ntmurtkt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3iutqzchw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3mnvzcpgl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhnaytz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwqgpnuo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3vdvoqspq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3nverpuot.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3znlairrr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vcgodchh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kskogeqd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3nqbarhgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyvdmfjh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3tzfcezrr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3axuuvhmo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3odejvymb.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzfdxbnj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kgjkxegz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3rtpyakun.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3kawysixr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3nxrkkbeu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sepowywp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ywgesvfe.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nrzwavxk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3abezhplr.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3duopmxdw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gelkefui.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ztapuknl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ergojolo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3blepvujm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3kbtuocps.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3exsljxph.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3tyxcaxws.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dgmcirtg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kxvjoptu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ouhcvyiy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xgttpkhk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3klejjvuz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gyqwdvyw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pqimsenp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdtgqzzw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3zpatoszi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3vjosyeqa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nijecgbz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tghgwmip.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jivzaupx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mzyicsoe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3rfjpmavy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3idhqorza.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3grodgidq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3towmqjzh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3owjeyswv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ycflhcus.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kigyfnpa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3lcraqmbc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3bxepnmyf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3hqobjhol.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3gevbruxs.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3hyzaiywc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lulgtmkl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3zfahdqrt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3berojfdi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3katrcwbv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cufldnit.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qvsvtmts.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bzexlprc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bckfpvvd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jlkzdfxk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3umgksfzt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3bshztijk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ijfewkqy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wamxhqpz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3okkrzqhh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3arccxpoa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vdmmnoyd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sszctsno.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3kpfilert.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3utwbelij.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ikehqkvd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bfjkihpe.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3iiacsqbv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3uaaicbwq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3rflniknv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3jheaizmo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3utqhzjps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbglqvre.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3tjghqitw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olzbqtip.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ikjnozpd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ldjitwze.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vxcdezvs.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xchlaowf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fdpgiecj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3punqiwsf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhqruzf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nemrfzax.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3uhuqjypa.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uhmdsfnl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dtfjlicg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3akhuyssn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3frplnpep.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3txpjekme.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zfgxwtmi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fgbkmfgk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3yilksnrs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3dimfmeva.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3tiqqjcnx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tdoswrzv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wakioljc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zhctench.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dmpbipmc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3fytkksdq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pbywqsgv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fjbplqnw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3imuramhw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lgsizxze.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpmxhtg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3otrjetxk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vqxrrrgc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3durccnko.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3manzxuug.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3nvucbtsl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wmnvpsms.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fnnsymck.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kdbburhb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gpdqsctr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3phizxqwj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hohxqniy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3raymqfhw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3gymxauyv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nkzfmivj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3qayegvbp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zqtvsrgn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wcigiavi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mdcabqsp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aziscsae.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wkiefjue.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jlrbznqf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3poulkhjd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3uevpgosn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hpfclngc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wyfmejvp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gpzhvykm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xbyijjwu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3jhedfeqz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tveeggmy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vtuocqgo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gqxlphku.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uqfifdyo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3yozqjyff.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sgzkaevg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tazzqpsy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3iwdheile.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hftknorr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bapnuzta.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oglsdthl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yrqihnhf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3stgutaup.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ptjwtvgr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rsdtfyeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3topvqonf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rzzvqufw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wewrhhgd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jeloqzro.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vdftuxip.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3firrwmci.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iysdqbhk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vvdlopqx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cehnfcon.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dcqayqdh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xpqyiibk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qtscwcyw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lwowycez.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jhwbxijm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rwqiclkm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cgvqjskl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3onrmjbbl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3axrxkguv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gnsoylyq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jimuaapk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3catcvuxp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zktydvnh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ijnzewhm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ysiqlrqg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kozmofof.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bcdztwfp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3thgzauny.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yhgbcekt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fyozhhlg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3cazvikmr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3sxnfcuww.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3adjjnmct.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gdcnamts.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fsktpzet.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vzzuuoop.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3lvkzhvyt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fmiyiarq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qqtgbifd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3weczarkj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jbizopnv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jfrkvgpx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3nottglth.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ttcwlypr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mxocpcnw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3btlcgoeo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3npzlagrm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqocudbf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gwofydge.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tzgjultg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqqwmet.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yzohgxrd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3htffbjmt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3snlbepsh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lkxtmvzm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lomfgxty.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3psqasplm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vyexlmon.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hfupaldy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gksuqxgl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3acxtyhjk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3madgvmdu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3juwkjpgi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yuzzxtka.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3isvqyozd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ezvmsjdg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nbnswazl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3amnzjlgz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3irztyokn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pzmbsigz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3faftauhj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pkjzurpy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zolugbdq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ezsebmky.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xatetutl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bpvcowni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fiepbioz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wtwduvyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjqckczs.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mblklcow.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ezlnvdts.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jazmummh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3znwjvkaz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xocfprwr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rdpilhte.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vecfdepo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bkceprpn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ngjqnxwr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qamvooaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lpstcrrv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3incjpleq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uvjfonls.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3twcaqugv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ehmpabim.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ajonheey.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qheypqft.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3anzpygxu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3eaznbwtt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bpucfbje.html


<!-- 参考信息 -->