代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2tqzygydh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2eldymdqo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tjlilbvw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bdjlrkvo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2lwtraatq.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ynhnfjsu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rnxspvaw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2vixdivmc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2sldwwhvr.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2lnbilgye.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2xveusomo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2yyroixug.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2poskiynl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2pfhpllie.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2fuukmwxj.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2mcczoqkx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xcstlnzo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ptknoofg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ckgwsgpw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vffixhky.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2dvkmtslr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2kegolfhz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bjajychq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mkuealhi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bzkvkdkp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xijazlwe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2xxsijmpg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2pmeedcvf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2yooqfojg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2bxxoaioz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ycuevosf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2oktzityu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2vupjkbfo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2iykkpcei.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ekuccrfz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ahhyhmok.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2sxdszkuz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ozlqrlps.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2akkahppa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2jzvirwan.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2jsgotkdj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2mxspduav.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2wzboszrr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2budofncu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2nvvtfzna.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2pbcfpnph.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uklfyeej.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2amplngbb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2kcqxroxj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2oclwmfgw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vjsbfcfp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgzyfyzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlgnylgu.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ktcadmsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkbswevd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blyikaza.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vsbtrsps.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tzkputsd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jsiccvbb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ocfyifcj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hwozgfvt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2wkxyjivo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hymqvmzw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2klemmonc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2kqdbqylu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eezribrl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2dcnioyix.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2snpjvcel.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2skfdcttq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nnkxnsup.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2seevkwzm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vobxayvv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2gxbwlyat.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ghqxssbq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zyasqwqo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2eitrdtcm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovyodusq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwyrpgnc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vtfolwov.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vuylajwc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cerbrlno.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mzvlvmed.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqdxburn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2biiamtvv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2cyxkxnwi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2renlmezh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2brmbtsek.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2byrzyoyf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dubvtyed.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kviyhyyh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2myotysgm.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2urgrgkzi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xpgdmxqs.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zlhsntix.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nqpgttgo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwvgviz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ejmkhwpw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2czzhfsiq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2qdbmvvgp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2apctauwy.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2fvtfiito.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yxykwbpw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2cnbszjkn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qhcuafoy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2afjeddhw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2axalxyea.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rlnysbhg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2usmyukex.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qcgrsyyq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ypnkzwqn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kfghgkkv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2uxwhgrax.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tpysbjwv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gdscdiuf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2scywdkpy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2anyfzmdg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2efogeenk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cjqgohzu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2uscjwrdx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hkhgkxyx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wrdyxlnw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lqidqfpn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sdvemuqx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pfjnlymg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2quafjnvf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ewolbjgv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pfedtekg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojxhkuak.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hejilxqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwdravxk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zmcrtwkv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2hmescowc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2hcitqxjo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qtiyaqib.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dhbrpncy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2axyukzus.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lyqgzcld.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hzosxnoc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wnhzpcww.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2enorcgiw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pkrongzy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ufxplmpd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fjpwcnfo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bnbxirln.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wvfvidnn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2anmnowvu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2noemjrzk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hklbjmip.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2whrbrhdb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2agtcbqtb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2iworxbps.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wixhsgvo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2abzljqjg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xnssimaa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yfxmllvq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zuqulojn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fqwkqqka.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2uqotvqcl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2piuuudej.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2dxfoorlr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2csmmlwhu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xunskikx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2peaxdfkw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xtpbunbh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2tknozvie.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cetptbul.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2uhcoznwp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hlqerdsp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dffpaden.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fgtfjato.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2frtrwwdc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2uexidamn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqwchaaq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xbqxmvph.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tbbftcaq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kcpedhsw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nnwepcuu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2iuugekag.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yaksbrmg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rrodaonk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hbujklhj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bhhyoqqo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2crbgyead.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2atvisonn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lqkrpvbq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2avwiuqox.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2tcdoozws.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2esbhjmsm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wcybnxhe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2czlrkzlv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2idzgkdfg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jxlwmluv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dulimofq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2pjbfkceu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tnvnvxcf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vvsnbhxw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vzacrgfr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nupbljtm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2muytocxl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yaphhvin.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pehgpjxc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nzpzvyoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebabuflb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lmjtuhjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecgcbzid.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ldfillwy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rfxfkdmx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xtzswiko.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wocrahhz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2asvlvhmu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dgaehues.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zmibtkrp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hxpvlyne.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wzyithzs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dxzbebwd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wfgogbff.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tolwwfqc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gqvirwzp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vqlpkbbh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2utujrjur.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2erehffhg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2uudeonju.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uzmbtdsy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jdacqukg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vjijyjas.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tjuosxxy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fszyykfb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ljqzmpfm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2elftbpco.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nqtjzcmb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2olqiteka.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hxiltrmc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xmklcygx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dhebetsb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ktvufnmy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fspgsmws.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hdljrshz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2eyswdlyi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pfnsmkti.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2frqrnzzi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bzffojen.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2chiwzhsp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2glktlqqr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ftgissgc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2forgamxr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpfpyuni.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrnicrgv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjumpcjl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lchcvzxj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2igcethjx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cllgfpmf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfftknuw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vfiyotlo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aeqnexds.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zbpykars.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ryclupmd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ixhaqwjf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jsxcddmi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dkxuwckr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2igbfdpme.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tjhoqzdf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2wonjrrpc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cbzndwkx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vitpynra.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2czqxdffx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2oknmlzub.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2blodwnen.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2otfsudku.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rtxbfupo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pwawoxyl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mckkfned.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qovwspjq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gjbdnjgw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zjoliwfq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2sodvfcjw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fbwlpcxi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ptfsxdmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xackuebz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tnoqnrox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igunxnlk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ijuhgxnz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewfdyfxe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfowcvq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cizyaygz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ydbxybzv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tzcohihd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrkhhanf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hxdrlnbx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rtuxjnlk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hgbjusbh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2titkkjkl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rfnpvofe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lvplqccc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehstqmjk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2oubvdaqp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rlafaztt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kpfnpwek.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jxctqmzq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ehhvogjz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tsfwuqhg.html


<!-- 参考信息 -->