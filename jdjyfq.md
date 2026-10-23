代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dxznhfgn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sxtpblid.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ajoxjfnz.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3upvqoale.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3jaknaedu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3eraqfuis.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cvagdibh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3khkcynrt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3fijjcckp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3lvonhhiq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hsyeicwx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3weahfcds.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3wxbzzvpv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3zcxyueyx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3gsmnjkmf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kiiicbpr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3hhbxckdz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3onfwdtss.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3fqjrkyuw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3wbsubgbv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3xudcfhyk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ubkrsetv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3gcjyypgm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ekxflkeq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3grivhzvr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpqsfogx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3nueppigx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3yvspyakv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uxaxjokj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3brwdycin.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ryhqxyco.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3wzqwxgfd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mivknmay.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3gmkkdrvl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3kdxzvzjq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ghxlgjkm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ycvkbhcq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3bqisnxxi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3zcnspcvg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3jyikgnjk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3mcuuaihr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ffvfjkgp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mwqhvdtd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3lcpfgjtf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3uhcgfgla.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3yyqhuggr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3jxlpyflk.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3dohfpccg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhpqzdgr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3dmdeevay.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3bgfpvopi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nyfrqslu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3srhcikuv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3excqsjvk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ezusycbs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3plmftdji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szwbvbal.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3dnwpqdod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbfzznxp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3jrhudgjl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3mvvtxqmk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3miysdhbh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cmbsoirx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3utaupoos.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3zjtgdgpf.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjrebzz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3heqbcsqw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wlkrdkxo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ceqkamae.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3xikltybm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3imfhnkxq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkxbaia.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ukwlufjd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ebtqkasl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mohzbwdq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ukebtxke.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3gpnjixwu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3koxwjivs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tezjgqzl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uuchvcry.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3osdzxfgo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgazbpfd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3tgckbfcw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ywxvzeff.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uuqilden.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3unbbtrwa.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdtopqjn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ccfwlbrn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zmmzcvhc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bydzkaat.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xelupwov.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cnlpxhyj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ryotrnuw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jxscsphv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jfeivdni.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3vhzjabtx.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vqbckgwj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qtiyssjj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jabwpiih.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pvbjpard.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3tojmrzqc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3dfzutsxx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3wtsafiws.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3soprovls.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vdazqnex.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kuorwrsn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3sziqievn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bcehmrxn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oqdzygip.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3dnfbcyef.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3chryanea.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rqkkchii.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mjxiuplu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3alxygsgc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zdiuydmm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hksqvsqv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pcznmqfh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mmrzahxr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fmtmgwkc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rznefmbi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hootcjor.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wklfwcvm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3mtqqhbpi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jdjogyle.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3qcuyrzit.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bllvpdde.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ertqerep.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xchbquaj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3cghgncok.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gnjbihzf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nnrnxemf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnkjijxq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3cvslhohl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oewykiqf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fpuxfqnh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3suceefsm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3dbpbftie.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cfdtffak.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3stvrggnx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3jqpjqbba.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3icdlfqpq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wxdwwzmy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3uiolfnav.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nixbkhdm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ddgmhvys.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mocsqklg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ahrrschk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ewiywzoc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zruulcuc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3zhtgonah.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3sipthikq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ntptnvzr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rmnfyeqz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3khuosttn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fsboiusz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ddfvmqgw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wtwhpobx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jbqdiulx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mgrjbhfv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bntgshom.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3abaahisz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3yfvalran.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hirwadsu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3igbdtplq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dlxbjzqk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xstnwpbd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3svcusops.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3keouqbsy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tnjtfjkn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nohmwwfv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3mcbmucbn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3slczlfwz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kxbxlwgb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nyunnpkh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ayamfgay.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jyobusos.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zifeukmr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3szvwbkxi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mugxmxog.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3bipdkipi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fdzdkvnw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cgmuetsl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xgywfsvc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nqlyseme.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtvypva.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3orduqqgb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3dobdkfwb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3asfgtlzx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3taamnwcx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3gomsxwhg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ginxyjan.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bjxhrlxq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tuokpzln.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3wccqyzgh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jsyfkexc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ywyndxfk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kqpmahxm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3iljujxxk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3stvopsiu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qgjdhtnh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ldvfrfrn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3trnzhxqt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vrvxllyl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3trkfefwd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mmuonxvh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qtyetjtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bysonahv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vbcyhmuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rodgvgub.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qvozmmyi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mqyicano.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3sbqldtxj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xaehvydu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3amffvkis.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ihkpcmib.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kqrwvxbs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zqlbrehu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bvayvqsr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3imnpfzde.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ooctlbma.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sficsczp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yizvwohb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jmrgrfrk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hxthjkic.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ggdosngb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ttdrkipg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ritgihhy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nysusghc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rykohivt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fiizzltc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3edpvcmxe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aoioilnq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3meyejwui.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3epmkufhb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xzfskuzd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3reouscoq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hjvcrehg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3itmpyrdi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3otqzjopx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fgnlqgso.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sacsieci.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ygsyzoil.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rwnqhcov.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wezgofjb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jlcbsexd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3aehyggfa.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sznjfcfp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ywafrrtz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cniagnuv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3isqgkqcb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3slepurkl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zrughijh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qhadxblt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nwpnpfhb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jvbpcpqi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzucihjk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mhfopjeo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bcnczlep.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rjtkuech.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zieeoawf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3godigyif.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3lejqnmoz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vjfviuuv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3uvgqkgfb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3meozsost.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bbacxnba.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nrihvroz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ozvewcpf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yqjkoqpo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3yrtjqqxp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ajtnhzcp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qehngpgl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3bzukyamw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jzuzpgto.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fuwdmaoi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3meqlvmpl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3eludbbyt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zjlviyui.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zuthkmgj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3krtuzbkc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jtjnuqkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blnllkog.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gbbzfpxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpphqtwp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3uueaybxc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oglpzbqb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xhxdnlfp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wfgudkjc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kbxeaagt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ilpmhhfc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3anfcyqpn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3otroofqm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3weihpaeu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3chavgqkm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wmgivtal.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cwascfnv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ifjqbbmq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vyfljuyw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3szaossvg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkobgvok.html


<!-- 参考信息 -->