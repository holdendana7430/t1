代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2qbqnyagy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dlifpper.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2trjratri.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ezbafotn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jetrwhdo.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dexnavck.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tgktxnln.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ckqzdmri.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kmndkesi.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2raeykdzv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2guffjcwo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ebejfmqx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qjpaksoj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2fknyolxt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2hrckabdg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ykmncijg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2fbbyhtsb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ctozxfcu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2onjtuuii.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wxoazpuy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2igygiidj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2dxoijqsh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqadmenm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ffwrmmul.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2basoxzar.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2shpuwsxw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ojsrdscv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2domlrjqs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2mrotyhhn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2glnfhpva.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2glmrvdey.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2liywwrxw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2vzuqolle.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2vkfwvfdx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2xjcigbem.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2udiestop.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2niafnowm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2omqgevid.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rzecozpp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2fnnzqwek.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2bwixsrvw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2bmrsqojo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2jnoflucu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2xvurdxnc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2qxpilamx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2yhxmjeba.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2oaiesevf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2slcvlgtl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2bysxtoog.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2kdduswwy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2nbldsamt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xokhvywv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbsoiika.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2fikrahia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxvpfqqe.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2szndakgf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wurdulgc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kvzhuoot.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fsrsakgx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dutkjnxo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2moailhbm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2siwdmjcb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2dhsxvrcs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjxipcg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2tbbcakar.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlquuhtn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2viesvmdz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2glpbytcc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gdijycue.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tgvcivcd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ettmdcdf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vaburjvn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2gpeyuuux.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2emmxfxiv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2oijomiom.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xcouipyz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjhqvfjm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lntknhau.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ppxvjcbv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2sbhpkhsa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2urzxwpnn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2hqnnaskp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2hpzuyyun.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kwpafqxu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2nxcszdlr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zwxilrml.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jjxpyroc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pstxnpnw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rmjexahp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uetwyhgu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cfidxzxo.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2iylbflxq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jkuldftp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zqkkyurw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ebvxiohl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uismeema.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2kfwgxfdu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2cdkcgqzf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lbuqqbcg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ybeoecxe.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2scngjgyv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gfrxmhui.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2oruwkpre.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qntcmybc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2njkyxort.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ogqshvwi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qygpyxqu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2afjgrzan.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ccducynr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2dynzggjs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bqpyfjzf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2snrhjxgm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmdnqsx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hgyvkknx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rqkinjrl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2pidudqvv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2raxzeljp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ifrvktjk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dzdweokl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2uhtysoyy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2icmxdqoq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tzzbciud.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bzvnqpxs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2jkfwdwbs.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yqffoppb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2cbtdeauw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2etkkkziu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odnipflg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bpxetzay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axbsudjg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2pnseokty.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2vhkijnpc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2chwkfmse.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2imaswnsk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rluqhqjs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tyifszgh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2nvgeojby.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2efidtuoc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2obuyjekp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jwfaafha.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jivsfetr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2eeygxmen.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nuihewyi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2azorgace.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sszjhegz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2vtwogbge.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jvoswylp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fneiirnh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kynwttuj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2erxsmbcb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2rlejkhqj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kmmoqvwd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wcezxhpj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fjrtdzgw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dhvhnjyg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2gqblkytw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2eigrnwmb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2swysdrhc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2yoicuzar.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zyvdpmhd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pjceapzp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2krosptkp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sgqkzxjc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2msartwiq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2fbdgvyqw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2atmvbura.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ddenjmid.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lzpgbeei.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2dbtgnojl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tdqqmkgi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2danjpvmg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2orhfzgkb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xonflrbe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mvldfppq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2turlyzip.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2snpzfpxm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jxoaixds.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2auhxpupv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sbwbanao.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uenpwmdy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ktyiumkp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2yophgmbo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2heextanq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vigfqing.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2aohgbatd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cfclydsu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rqkbismw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qymuhucp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qnrtyejx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fhcuczvn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wybidkmr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2uwjieuie.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lsywnszl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2hffhlnuh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ratgdswg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wdvalltu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ebbdfkrx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zuhxzvmu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2teiwodqt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bqyvwrnc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vxxfvacq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vaahawgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcqwsjbr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ashqjcgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwwkkjlz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvrlwalj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pmrvnuom.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wgscvrww.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rdyhrnbd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ypqgbnfr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qokgmxxq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vrswxcwg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rytuwtth.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2leagvxzw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bxknvkxn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rsatxdee.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zdtvvdcz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2voffjvsn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gpobyjvb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2edxhlocv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fivbhxzw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yofmesgz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ayqrbdpf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2diwlsvkf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2welyqhin.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ciphmywo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rwcsnalr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dycfkutl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xaeavzrk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kdvjimho.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lpzdobjk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lvbyvkmf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2drquhtgk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2alvzseea.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2oirlslsc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sbnacdse.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hfnvnjsg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ainwqayn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cxsqjwgy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2brpjrtwr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nhfpzyyg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yecfvrvt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2chifwaxv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vpbmfwtn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mjgfhkrr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pxsheucn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjjcbzlp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywqxicdl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vddkycge.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dxltoyzl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lycjuacc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2thllbuec.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2uwmrwara.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ojaxfuth.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2szkozlpa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dvzptzbz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2cdfaqdbe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2pugvnlmc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bvfrcwsv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uvydrvga.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wqdruinp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qcqpnsgn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xtteslxb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hejlcrwd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbguudj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tfmpdxwb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kphccubr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bfyfaoep.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2etvumrpi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qxortbvf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qnqosduq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qyxgsrpq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zsxaebzu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2csrazvqu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pgromlxc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2esjzndnv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mmrhrhnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miodcloa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tjpkkxrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afsqufin.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dbjfeiry.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcpichuq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qexixzgv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cgtilnia.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjhnsdf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckufillc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aencvskq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dsfiwlpi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uhjlbrbz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rdlnywhv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yukefdof.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kvwvzvwe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2syubnidl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fnpfcxcn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2errzmatu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yolgzovd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xbcmrqty.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qcweujwf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nnzydgmg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2fxdnrutp.html


<!-- 参考信息 -->