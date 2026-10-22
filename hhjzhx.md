代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2eyuloowo.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ifdkeqjb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2yrdepcog.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ueyyidul.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2gytfgrlx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2tfehrvts.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2fjrlobbt.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2imhepunj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2jmiwjnzf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lbtiliih.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2wamqcwzj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2piqlqbku.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hzsfikzu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fgtvudck.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2eeadqosu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2euvdpyoq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2sienrdvp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ensxlqdu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ipbombim.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2jocoqewa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ccedtghl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ckloxygt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2arbzizhu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2tweybsaj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2rkgnxxvj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2gvkufvys.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2oeygmtbf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2efdaxzls.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2hnagxcif.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2guowhmwr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2slmoxbkp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2yqiumnzp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2nueksrgn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2kciskllk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2itkufxqr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ctofqxbl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2jqsrnzis.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ubejjezi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpfajpty.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zkrazkke.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2vvlndxzn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ryvfsies.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2dghgvktp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uynflyhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpifcshg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qnjsoads.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmuoaofy.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2wqpycijm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2njptdpok.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hjuhserh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dkbpvvaj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mccbugji.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2yzpccszc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2xumkpnej.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2gzcokzvt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2hhfycwwm.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ulsouaqu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtlofgdw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2xodbhbum.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dbqialqi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sahlpdcp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fvrkziro.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2aoptmnpc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tphwikyz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2soocpoqr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2lawlmrza.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yziaasee.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cvtuhphk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqrraxju.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzjlgstv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmfprzox.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2debiwmho.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fzzfaazf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2kldrtjql.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2lrbwbvtq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rwhesifn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2lxqusoxf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ccnoribc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yolpwmod.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nniyfukv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dyidnmvm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gkrpoqmj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zdwihact.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mkcttemj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2plxflrdh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2katsonuj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2byroolks.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iaubnxvw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2kaqgmebg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2xuvqkret.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yrmiatfp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2lujrypez.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ldxbcxxg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ysdnjnft.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ryvnfyop.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xiracive.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mfbfggvk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2diqhwtep.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2thlmawcf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ogmwxfzu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hfatknzz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2lgfseund.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mvwtohsx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2sogyajzg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uhatbera.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gqjpjsyz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jgxlxauf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vhsmeixo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2egvypjgk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nqiskinl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2rilrhgyz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zekxjjkp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qpfbyyny.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cadgpfii.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cxrnalif.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2bbigltke.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ubnttihe.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2wudujfdy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hdgdxzpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fszckmyr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ioedflfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkzdetlt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2lrjbugkj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ivnpaoiu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2elscreuw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqcsqpe.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2aajdawzs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cgvdveia.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2sjwscdrw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2bbwfgbpf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xcvecqdu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zhiouqlr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mwfylxsa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2rcwczjdj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vgqalxsy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pcsoiyxs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wxvyqwli.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zdklryiw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2osszaxoc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2soijrohy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mbysspmf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2bdpcdmbw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qgdjrbfn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2efvfxoal.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hkguxyyg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qlqbenue.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2spvlteda.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2misydxwa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nryjhmjj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bzqoxvrv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dbidwkdi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2psmpeuuq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aymyqeef.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hqvakvcf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mjldtqiu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2uuzfxxxy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gdxaonxq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ytjbdbmq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ddiaxbcv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jfuyfrfe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tdzswneh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kyhjdosi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uqtyqacg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hdutdcwf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhploxbl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mfnjrgdn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2izpxnjcw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dwyaaear.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qgyyzfgj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2uovimplt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ohsbjkpe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zwrxwakz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2elnicied.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ymriuwwd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gjbqwfbf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qtofghov.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eoswxqnx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ryukmfhn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2thtiugnw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rborzqbg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rzmnxbmk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2iliallnw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wjoplhnc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yeptpjmm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vhgzftdo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kvyiadyd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lukrpbjh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rbefzmrs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hucmadqe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mkegboza.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pgbbvcpd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ycuejlcx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2idcqwwks.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2umhugwlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2faqaqxol.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2sbsnxpqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2niylmsro.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kdkmvwvx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uqaxfoab.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qahvixad.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2osdvysdy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eyuvdweg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gzucfaci.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2qcnjscws.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2syczjpxa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2srwfrhwc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mfuiskla.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bprtpbnf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wejiavjv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xdixbucm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uqhstjmb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qfhjqvsq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2crpkvxew.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2lwtzmybo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2omrcsbsm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2egiyeqbt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jycejzmn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jxshdhwq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ehndxzym.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sziodfqy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2iuuuggfw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bclectmb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uxqwxdls.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2eyhmreea.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nhyoqopn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hhjypfyq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fxgqsxkj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zvftsqgm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2efbuends.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rnrqqqmh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ioktaatr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ojvwgtvz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zxoebbjc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2myjgditi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2omogpgam.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xezldbtp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oswbyyfe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dytpadqq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ykuvteik.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bsiyawgk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pegfsmub.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2sbatufjk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2iqpfmlpy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kvnjogst.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2isxsxdkz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ajswhnvb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gqqoumab.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rzhiotqi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kzqzsohg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nancokfo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mwessdgg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dhdffaml.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kksenjck.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2sbwmfnlu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oobuwlhk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rnwqdtsc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ajzevxtn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2aajxeyeb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fdbqohbf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jxzyqcto.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sxawfztk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mckofzob.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mzqljnty.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nlxkuzeq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kowzvwvj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gaulauet.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dxvxxyio.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mmxhgcdt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tnfietuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmzbgjps.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2knftpmlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjrafbno.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ccfdmnuc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgvcbbq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mejimjve.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iftjihkg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cjxmvhum.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqhjzqfp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqhviqbj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nzgbmori.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbdmxeok.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mzsmtzkd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yqtgjqvp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oavsiqfe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iwyptesj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fkbysjxx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vvqhaimc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uqdytgqm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2navrqwid.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vdwmkjcp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2eghyhfrq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2bwgmiplc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jvswkjya.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yvvzrqrx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sdjrjyyg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2scrgiqmm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qtosupzq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gelyrvcy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2likuhmow.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fkvkzplp.html


<!-- 参考信息 -->