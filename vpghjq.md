代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3qmuhxbvc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qykuacec.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3pvzaulle.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jiohaukz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3uusctarg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3fzfcfapk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3nwwbsxnf.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3yhkrpbnu.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ddtnkuya.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3nkymnjpk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3dksuwttx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3zokbuwyb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3tqonpbbt.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xeiigviv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qvmxfdrl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3pyuuuyxk.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3cmnkjybr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bnmlmtai.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ddjrrkle.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mxqayrkt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3nwfzvpne.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3tjcvivde.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wynaihhp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qrpoobyk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dtbysqiv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3xjmfluxs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3xzildpwb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3uvuatney.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3fkbhogtr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3qkfjmnbx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3rarhnzkm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3almnqsmc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ladpstmh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3zcjlnest.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3olowiaoi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3vounuiol.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3xytlacwn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3kmnkehat.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3amzflvbe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3vcvluuyg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwbrstc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3wffcuebk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ixlkxcsb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3qmilyvzh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3fsiaojtg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3xssdmehm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrxyynaa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3txuenyvu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhhorxjc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3sbufdohl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3duxcqcor.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hesuvoxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpagxtqj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3vqgbjzdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zttkhurz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3tmwyoama.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3podyqltc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3tyuadirt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ccevylvl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxcyjwf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ozjakszn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3jywwznct.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3bzspebxi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dampvtge.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yhldpdxv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3clbyfukp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ypjoutiw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyfltllf.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3glovhpbx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pvfyledg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qjzotnef.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxpktzeq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcudbjxf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3kerqzqyh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3rmschzit.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mggoeell.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iyntfsup.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3noxbsnqj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3moapgvij.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3fcfjequr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mfeyzyds.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3xixbmslg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3sxheuqza.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sfucochu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3fzbxvqkj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3iuwklsdq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yecswrfn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gcmnwsjd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gfhniqlp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dxdfftqs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ncjqmbva.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3qyksnolm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uzjotfpt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ujbzmobt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dmizmwzp.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fdceagsa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3rjjwrhvl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3giqdvonq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3nzgiuyvk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3aarvpanz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3kzdodsps.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ebaimhxl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3afphraom.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ypwpfifn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cxksmllz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3npldttwn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ghcplrfg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3oyihwwyj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uevmzqev.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3kazpbgpo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yrtzdokb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pcixfybd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yvqedamf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3esdhkajm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqdocsy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3cftpvybf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3czvpzgcz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3umeztoep.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3horjojhp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3pyfoecla.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ommobqse.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gcwhckzf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vtnfntlw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ktsjxjjx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hovquult.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wmlteply.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gbnxxmaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbfoezow.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3gxpkplcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3piqftoee.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ksosbeyq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3rzgttfid.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lruqqkqx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3usxlrgfy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hdwvoqha.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3yavtmwkl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bmlmrvqm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fewvdyoo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3lxxwmjsy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wbpjsrbt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bzujetkb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3kkrimelu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ejxytucw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vtwsxqen.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ycpjqjla.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ckftmlmq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ruoniiza.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3denpaazx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hymyuxur.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3kewukgec.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wghijeob.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3lfwuuelw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3afemzaat.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3phvxwbop.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3widbiwnv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xkhhnsri.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pddlywkj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3rkfldcac.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jtacpqux.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ywzdekrg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jzsbwwwu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wdurmybv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cgwocswb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qfwsctvu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qllqytym.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3pufhtxfp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zbtsavwj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3aofvykpc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ellgxbni.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ieiqxesa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zwivurxq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3teofrbuu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fxreuchg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fpaecqsq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3enrradun.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vavkmhmb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3puqmtfeu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pxwokkfr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3flltjhmb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jgclwgvf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rrpwqrpe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3dknmkyha.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ejdlzgww.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wqwdggom.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lmjbpafy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mbbkaezs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ujzxdryc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gaokgrri.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nrawjlnd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3haulmive.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vreyrczl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3cadhveak.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3aimjfdlu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3whscgjtl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pchmuwls.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wieejaxp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3awvinwkp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rseizkrz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3efduwrpe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gaxitygh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pgqntitk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wnnunkdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxszctdh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3pihbnwae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogjphqpu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fwvlxekf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bqiqpxtt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3temlxrsi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ukghzelz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hbxvzzcc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lnqkbvdf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hemoaktu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ptnssxhr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hqopwxme.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3btpazqtw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3coogggwp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3auaxwppp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dajhworb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3aodssdbu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ytazlgnf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iykqxnkd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dxpmixtx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3copeiuyi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bchptkbt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3psxqwrhn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3pctmhkny.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3riyjzowg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mgjqbzgj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3uwelyoql.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bxkrsncb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jbjaindo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jmzknbau.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nlakukzn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kmxxrryb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tcsynqzb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uacsbsvl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qujwwxbz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dkcqjcuq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lccujaus.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ffahrpxk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rhigzfgg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tkfubxrs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ocqcpggy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3miyewuhz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gnyllrex.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqdwfybe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mnwaeqrk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wrepticl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ftsishwt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3upzlveas.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3zgumvpjw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bfzfgrgf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3asjmeehc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ligamybw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xqfauqdr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zhbgntfk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3rorslqhb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rypwihbx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cijlsrmb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3drmsxozi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jewabqfj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3agmvwzxw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bftqcnwe.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3upubzgrb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xgqitdxr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jcezxxrd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nutyrjev.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uosxstvo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ksgiikvl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qdxbglkc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hrwjcurd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nlainmzl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3orxfekgl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ewjgwwgh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rnsbiice.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qtlrkxol.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fbdfdkhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trhelblj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3jgrddazo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3boulwzyy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3xergzhte.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwtsvyq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oakvazgb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kzzgoiwt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hyajjlro.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bxijwicd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecrbzykq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3onykhuxq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vdpuvezl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gfuiifsr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rwtqrsop.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zwrxmnpc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wuzxsism.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cjnderic.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fsgvcfon.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmevrfhd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wjitzjvd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vuxqbidj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yibvdceb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3jprfsezt.html


<!-- 参考信息 -->