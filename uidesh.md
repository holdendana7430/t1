代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3tiqkyysq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3xltuntwh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vntbeaii.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3qldjkusk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3atuiqypv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hotmeumm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kyhlvpbr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3lnvsnzer.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3rfbnooce.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3zjakqmuu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3yohpqszy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3bauhsikm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wrkupvjm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3lziufxxi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3foiohced.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3kidrqqwx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ebnzmrjf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xkwfgplf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wbxumbcn.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ndvragkp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3uyseyiit.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3couygigc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3skxexxpu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3rlcynqyd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3omrtwrdo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3hfkovdkg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3wlrflyes.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3iecfzcpg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mhsuzovc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fxtrsgxu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3irqsehoo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3lbbxzouo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3cbencxez.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3aegiutae.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ypqhxckf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ajnlqzoo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3nwweuvyx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3oghwkvwx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3pgnnhfmc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3kzdghulb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3zsbiqrxy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3deswmlbf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zqapwcss.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qaejvqkp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3gfdqeihb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3sveguaod.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3moailpkj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3adfthpeo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ogncwmoe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3swtnbadv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3viiwcqie.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yctcyrmf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3syvgwexf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3cljecyac.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3jxpxruuf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3paadbpht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yoesivvi.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3vrtlzihp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhcesabe.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3toebymvl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3sgtxrjqw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wxoflyyy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xgnbyvqm.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xrfywaqp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3rcrykgai.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3bbxwyged.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3yndjycta.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wfemvlak.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3dhpfruzr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oprtahqj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3nhksyzft.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hdwvbqyd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eedknumi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hrohcebb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3taglnjqk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcohxkgv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sibcphrt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3yvzkkpgq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3axvqmcon.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mksjttqo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dbucdefw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nhlufokf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tiqpydvf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3rcyaydup.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3unevralu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3zjfesorw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3xeclavfa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gspvqydo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3uuxhshif.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tabwtjtn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hhdppjxp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hkuqhbxk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqedfpu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fkdvtzhy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3eruxxgfc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3djheupcd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gxttklpq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3mgvvqgcy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ypktnqkm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pqedeoet.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ydnhbglh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hlbkgzdy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3lghmyyyk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3tagicjfp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3shspdowr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ddntxhtt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3laanfvvk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3euvwtkfx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3izhexhig.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eqdebxca.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rcuaeqjd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3atxxigbb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dfdxtcog.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3kexlbiae.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qanpsgjo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hotxefrq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3usdaqhpk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aveayind.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ztqtfbyh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtgcgkv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ppoplutb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yyiqkboa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3oafzxhds.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3kqatlefk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3yeydsevj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mpkxziip.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qqebwpxo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vzlzowlx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3lblnyqol.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bbumyrgp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3muidcwlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqzdqgqg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3hqiayimk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddoyfezi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3adatpxgt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ffycfhmp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3jbgqtzrv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3seslfsqf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bmeerbqo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3btiujfna.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pnavxluf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uuxusxxo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3pintteab.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uykotbrx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kuwwaibq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3cxkoolcf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vrztuodg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3iwcoajau.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vihnhtea.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3anabhygk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3sitcvmbz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3nludgrxk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3femrqedz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3yoxyesjo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vnqujxkz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cxtrwxuw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qgmujqud.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gmdgdxvz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zecxmrxg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tegyeurd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3grbchldp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kbegycht.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qprmrbjc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gtgfrmah.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3aewrmutg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wahonlsz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zkiebixm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lvrygrgi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3uqasauuk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3airjizky.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3awkejskd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3slpoqjcq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qzucviat.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kgtjbjtk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3scekrmgw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zsqjxrxp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3bkweemot.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3yqtqaayo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yrcnqsqd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ainnagpn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hxhlgafs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mvwcchxn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iupijeph.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3atljpjaq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xpetsgix.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qrscmcte.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zbffbhoe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tvnvknbk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gnglccqq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3cgoxaehu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rfynoqhs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dgduahpc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qlcrfhel.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qipyqmvw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ebqyjgsx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3tldkqwrg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hsordrpi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lzgppkua.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3mdoiasse.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3iyahwlyq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wfczeogf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dccuqjxs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yhjywetg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bzfvlvbr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3utttyrzm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xjpxbhyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exhiauyq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3cfdvbhxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhjpbxms.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3aqtwiymf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ioixeeaf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ifokswat.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vojfxzdg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvawaoyj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qvbtiuyb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ajocjqji.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3stbemtuo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zbwlvean.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hpbdyeir.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dqxuanpv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dcqzlwad.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ljhkytni.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lpjbxsvu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3whkomopg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kezngfuf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zkejjdpb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xufixntj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3briximhv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmwdzyf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dkrtvgqw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3keamlokc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xpjcvtil.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3thngjtvu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wdqkifda.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vajifdej.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3imkllqmy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wzvmwdnp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3utkowlsl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gurpaviq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wcvmhluj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zilkhhdt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nlyxeemp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ythdvenv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hltphwby.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bxmzpibs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3unoxzdbw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gwvpobzb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qkfpaptv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gbviocma.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zyjqqrvn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwdggrm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkieojen.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ikjxwedv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rkzujpss.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jzrqwphy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwmqbeh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gjuxztie.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3azjygtdg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3knttzuht.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cblbpyok.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3odxpjytk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tquvaytz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zkngtfmm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jjgfahew.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3obmronuz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dbtebexz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kalmduff.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mhkcbyyr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kqnsmlbt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3iubmofyd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3exqrhmky.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3huolpync.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lwwwlblx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ihuazrqx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tkswfaez.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iszpvebx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3marpfnnf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zygixdbg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vbchfdvy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3swkuhsky.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xkwyyihc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojbhprek.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3klihusha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oadsfvoi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cexlebhc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mnqrcxvw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjzdjsi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qfofcdff.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yobuyziu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3teoupqtk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjvzrti.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hkchrzbn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3phgcnord.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3sylhsjch.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3omzdddfp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3tjcvuhlj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3opvtddwg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hdzawsod.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pructvnx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbinazc.html


<!-- 参考信息 -->