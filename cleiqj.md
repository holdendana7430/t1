代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2tryswprq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mukwvhag.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xepejjnr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2qnewlnvu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jjvgluax.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2loymacmg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2gozvwfjo.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2dqtgptps.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qmdswmnk.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2oogzbxiw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2uxkderly.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2eljsthij.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2hfhkqizr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2gwbyioik.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qbngefjs.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2agvjmjru.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2mvrtlxnb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rdfzoyuv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ieqfngym.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wkkhwryy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mhwikkwe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2sszxlqyz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2truldxmy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2knsghmsq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2idfdmlxj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2bjdgdcpm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ilvvyqtp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2chlwfdjl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ndpkdbhr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2pbvlrvwn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2bzfijrgp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2lndtidcm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2kwawxqyl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2sdljnbcd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2iqfcdhyg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rndkkpzz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2jdjwdked.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sojaazuy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fukmernt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rsmfvvsj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2svhouahx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xruibyhe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2sgcusilh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2tpjeizfy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2zoekxzka.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vhsrwoit.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjftvshb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qcizipct.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wifynzur.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fhptqbix.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2zfamckkw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2iupsoxvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttozindx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2vtqrlybd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amrztgsa.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwscporr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nosiurjw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uzlunluw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gjbpprwr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hjcmfspa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ifpazazg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gunyfgom.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2tzbpbzie.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vedxyxzy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2gxmemnii.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2uanuvrxd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2evjqnzqe.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xdncigad.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lkaekvtw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mfbwduwh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gtlacvfw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywhyrubh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ombmbyop.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gdnzvoeg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2eltnouij.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mwlzxkzp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okddtppk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gavcuwlw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lovnrncx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2zygojtza.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2cusxjzdu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lsclposz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2jsjeytxt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2lcrjtlcn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2amvfzehi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yyesqytv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqagmopz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mozqhgox.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zynzogmc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jojojrwq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xahpfktz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tmgvqwhs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2guuiqdsk.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2aqszwnbr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ynxfztwu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rurqmktw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2aojmojaz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2twhbjuoh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2efgojxxw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ewscuwez.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ryrrdtah.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bwjjoalp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2tnhveqkn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oghjpptk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rhwvcmyz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2eokgfepl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mafhmqte.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tekvrfuq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2eqivdabq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ncjcxmsa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hjvyfgqo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2juzsgwce.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dqakcskm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nuvryzlg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2upgjefsy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2gmmeqclk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zaaxhbws.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yotejzpt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hufksopg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2libthkgp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2omhnfaaa.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dlrdnnjf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2eocrfgmd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2gamsmctw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dlgtqpiu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jnbqlzvr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hscqqmli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikvhfouc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dfnkchvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ximzgzlw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ydsmnhcj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wlthdimr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xqopoldy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xvobksyd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gvczdjwa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ntmvwqba.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jtxxljmb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dgzpuexs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kqgldtst.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2itfjsnop.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ajquxcrw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xlvfgvkm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ahypwqqv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hzdradwf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cpsjphvf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kcsbxxlt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2cepevxar.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwqlcmuz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2zehlhzzk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mhrhcmdn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2yqjfkvqa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fypuiuyl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2swqhdnni.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lzpxjgaw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jurpnuvu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2cftkmmos.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ucynfvdc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nwogruwx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2crxiwche.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vrdktsok.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mqtabpti.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fhjbyrkq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2iuhdurvd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2brxibaby.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2myynfrzt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vtcqvtga.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2bygnpvwc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vkhmnewg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2njokxkqv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2elbcsbvf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tsphbqfc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vvyjvzwe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mvnouado.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hbpklppv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rzwgpbob.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2sfdeygkf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wmondaqe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2musqpjyt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ljucfhyr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2chipiwii.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vellrqek.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dcaaiqoa.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dniavzmi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wopntmln.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rqfcejum.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rptevwva.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2smozkmfo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iirwnylt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wofyutbb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2hrqdjltg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hqnteizf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2bhbyhcsn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rroyecul.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2peslkbkx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bebzdemk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2apfdjkrr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2otblpydz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2romrrlab.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ilpdqpru.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lkuraopw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2onpxdtye.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zfjvftah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbzewack.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lzohevpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvpfldsp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2janwxklo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xkbjsesj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2rwwjejjh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlkdkyqm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ocyfzudl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pnkpkzma.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mcxgzivi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zlbuhnwo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jgsafcgi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yidfkqzw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2maxrrtru.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2srgethfi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ukhpdguo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ksgyaeau.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dgtshztt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zsojlqgf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2khgmkojy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2blfpxxwh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2gxxwdpug.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hknajxkz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vzuehnth.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fvqjmgvq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2urjvvjyk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kthyoxbz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2crhhgxuq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kwdrhzqr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2trmfvhob.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vcgbykyy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jzimglts.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2noqvrlcx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rotulxay.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hritkgnu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rnfixftw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nlvwidpr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xizcjwxm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hqynammh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ilmyiyug.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuiqdtff.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qxcpepct.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sqqpscbb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vxzwcdrb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2itawoqjy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ttkszovv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2klsnkwdb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bryxuhrw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lmqqeuru.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdlhyaci.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2byllxdys.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zayfhlhz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ypgbonac.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lqrnmuiy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2odxyionw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jwnsordd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2goyjdmzj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rgcruovk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qlzembvf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mxoeufbl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cnzntywb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vnzfgxpc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nnpfobmm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2nadxegae.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dvcuglsi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2stogofdj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2owxxksux.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kfdsewro.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dcvckqbo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yhzivseo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2aibegsae.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pofulbkv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2idrrmilv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2svqgcbvc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yyrwyrij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfeybouq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2birfhrhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfhwldew.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fqazpydk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2skzdahhy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rzhzishh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mlzumoxk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ywfsqych.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eoejpahx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgqxtioo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wmwglknc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oiogdxvi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rexxaxab.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yfjutptu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pngyshir.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gyunwwdx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tkjfbpqs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2egfxsszf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ditbpgzn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2htpkfvih.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lqiudsdu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mplcrebk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2onjvcpmv.html


<!-- 参考信息 -->