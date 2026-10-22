代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2udktyfoq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2odbivrue.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qsuncutp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qehlewcr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2pxvegovp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xtrgiktv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhzlwzb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2twypdkbu.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dckeamhv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ickaasjc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2bveywusd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2jpwzzqgt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rsayjunf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2lhablgxc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2kwhznzxh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2hytwfwmf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2nxqinzta.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gsognllm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2kgesasen.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zgewqpth.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cldjcoys.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqesgrvz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2vsbvggch.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zmjhxsnr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2awpululk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ndtzilln.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2vwijjcyb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kdlmaxml.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2zrlndkse.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xiqoudto.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2lvvwyowb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2xveorqjd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2yjlyukif.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2vcjtuowi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2jclivfea.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2cqnmgvfp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ojqouefv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2raizdeph.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qavuiigx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2mpoyzjvt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2btwtmofy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2mlmdiboi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2wfxqdmfa.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2cqtcdmde.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2npljbvvf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2hdxuekdn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsiwdbtm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vllykvno.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkzuqinr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2vlhvegio.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ttgvqgwa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfazpgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohuhuvfu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2xayamyly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kibqvoxn.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ddfoswkx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2iipuuaux.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2egyszgak.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2szndsvtu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2twahiayd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2zwknlslj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2svbbklvi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2pilkfnfc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2lknlrfoy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2bcdyrsxl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2djhfvums.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ypeyfgdx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lvpcwbdk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wlsxequl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cfleazjw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nyutgbzt.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwmipszz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2rlohpgkg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2jzsqnliq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vmulzmwb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xvvxhhdc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jzjcniih.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yuuqyauj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2prkfgxqz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2crydfpex.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lvhrcykr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2tevhnyjh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipmqrgpi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2byibgcru.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ygbwriig.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nbkhbzmq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rxbjfnhb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rgodgtfh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2umnedqzj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2sjwbnecp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2aahtwlzz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2fgwprfoz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2njhknxzu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2myxsyahn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vlyxipez.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xzredxyp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ycybzuxu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2rwzvaaik.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ytsyzfpy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2myzrksrq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cpcmwpsi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jkssoykk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2odswjqgt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ywsnvwni.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zlvlgwaf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mbtrbhys.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ickgkffw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xuvtqoka.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rydttjuj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2iphdpzhm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yofyorvi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2pslmzpxh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ujfhggwv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gdwugzhr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vfpubpyy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ckaxepkx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vqaxrnyx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jiancxhp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2urdgynqp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yxecsmga.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ypbosmrr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dsfjyfpt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2angichgo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2eskykrtz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2cmpogcem.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2teaorkvg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zmyrvphr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dewnvaao.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2sbwijecm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txxkermn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2moxovuaj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2owxntmbc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2udajersz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ovsvwchz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cnhvdlol.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wysxiqde.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2gmddsudi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qtyqydtn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2itwfvuyc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ohnaoite.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2csscrsra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2zdsabbis.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tdrbrowy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jzjodsog.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tktbmvbr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2zzhjrylt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2orrhmiwp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dtbkmdeq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2easmrezu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2yxisrark.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bmigqjpm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pqwcgeoo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xfvsgvyb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zhhstsop.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pnhgvlgv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xjskppfy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hfxgvcec.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2fxdxsilt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2sbybrdco.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vntrfouq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pyzmxcoh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qnayktpf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2eyhxlzga.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gcmuwtpc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfezrji.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fpzmrxqo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vhwmddqf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2sdueyzgx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qwduswpg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pmnaurxi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zdnfcdlu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pvrgxmbf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vfogzlhe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bezfffkc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kzijelpn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xetbskid.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sxzthitn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xjdfrjwz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ersshkil.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tjukeauv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dtedceol.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uxetnfza.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2wirrcfge.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cjalfxje.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fdjzeeas.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lwbegyhl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xnofgqkj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2crpuybmg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2reyvnsfl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ugxtolqu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iblrwmbj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2tnerswuj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2epplgdfm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2scesauzy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nfpxvgzh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zwwxdotu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tblhsudp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ewuoawgw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2noeorhck.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2hegqvxng.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2htgpvghs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eqzuwkmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2goohxpyk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ifupsnvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfpoinac.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bdkvgnry.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2loreiznq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fiqtvkjt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypxaoyai.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybkharvw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2aowwdzei.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ffsyzlom.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xexxbxyc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vlmzetae.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2veketdzk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ojzkuaml.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qemokhtf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vtubiqak.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fccacoar.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fsvfbkpr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rvxnxsvp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qgilsfzp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ehewiimq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rhalotvm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nrrdudww.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fttpajtj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jitfainb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bwdsqjdq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2koljtxje.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ptqpdgfh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ngrvsfhp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2livjclnm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kyxfmhak.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gjyrgagd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2oyfbkvrz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tddjfrsu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xczxeckc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vkzkmpap.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qcwbyjpt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kbldncmd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ypndnozr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jxoanwwp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yawbrmhw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qlguodej.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hongepkb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tgqowama.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxdwmaml.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ijmcbgle.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dxafzvui.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2uixkmkzb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lqlmvznc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pifqsybw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xlpetril.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ryraojmi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2veodbmjf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2uflrrlyt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kkrklrbk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wlqwjaqg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wisvawfh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vfwfpvnp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kvtokkji.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2wjombvnl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2adtytkzx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gbcnfhrd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2osowxtmh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2sductdyc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hhnxjotc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ndzfdiyn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dgspsojj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qatesnga.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mznuhevp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ulqjrzku.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yhwbxgkt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2epqtoyeo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wiimkydn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dosderwh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ltwpiqgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eflcyxwy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2reioptvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjnxgvcn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yndrqubr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hdmppvdj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nvbgikdx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vfjgppps.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dtgefpuh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovwdqadl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zwoxcjfs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2exdnhqyw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdczrpjk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rxffqxfv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jvohgrjp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2qxtgqzcz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fuaoehvv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ncduiawv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ydlpscau.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pikbdtrh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vrimhhln.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2svquldps.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gfjglsog.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2edkrngtj.html


<!-- 参考信息 -->