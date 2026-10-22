代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2afuaabfw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2enmuyavp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vablrlcb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fmeggwlz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fdnmneii.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dzmbfukx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rmoztdei.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2vlthlatp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rnqfxnde.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2zeajypii.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2lkyqpvev.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ppbqcznq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ontugwda.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vsdsvzyp.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ofwtdeew.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ryptlapr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2jueyyogy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pagiuqlb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2bcuzuhci.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qrjntnvu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hkfmizgv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2jtbneljq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2tbschfbh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cntgpjyi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2aekiebfk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2pmdhtspq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2vuidfyot.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2yhaumllh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2eljjcpkj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2pqpguqiv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2btkyxprc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ivkweyuk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2vmkpgbuj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2wddysonq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2slmqpkvs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ryicjlno.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2oyxznnos.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hjxwxqsx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wicxwnhf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bgacbpht.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2jpxjwmrd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2cihyosgi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2kglcndtp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2txtsnfrh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2echwbiqh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vpjrhwrn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ikuyxfoz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2imurzwwz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2azvzoavh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2ymzzorby.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2dnjrhlin.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2efsecxxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvrouuqu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2gkbltnvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkcdcfdm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ixjivfdh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2bevaurmk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gaxfoejn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cjhddofp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2psukgnjv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2rblflwwb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2grhgywol.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2fgyypist.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2dksgjcxe.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2gulbpstn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ktqgahgg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2uwfzbidb.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hewszwma.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2faamvnwz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ecskjixt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nvcrpxuz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kagpjeod.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scpzofje.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2xtctbiyq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2opeisjzc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2osoyopva.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjavvzdp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yhegrjvb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2guhuvchd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2svwggbev.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2iysagory.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2zgbwuoed.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ewrzcvls.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ulvztbdu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2gfiricvv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2irltbuon.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2simgzslu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kqupgdsz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tqmwqyzs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vglsmyif.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lirjkszi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2sfkefsdq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbuuerj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2sbgvdfcn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uamdnlwu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2huqbjcfh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2korbvmxb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2pvlsqyns.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2eapwsncr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ptyenetf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2shfmvzsw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bpnhxxig.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2lbxrnkde.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uuintqyn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vrwnhsql.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lyzycgqs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2psdchoml.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2usricgkz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lgfuumyx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jvocsvqg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gnjojxoy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2bbjtyyhz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nhgozrag.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ddbnfigh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wpnhbkhm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2jtssslvv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xsvaqtlv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vllrfxmj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2osmjuuqy.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wilndltv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmaogyet.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lrdcrlyc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qrkwsayi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ocqslrbo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2jomjjjhs.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vzjdwgit.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kratyedr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odeebbzl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2qfvpbgmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2genmydjk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2lmhuvcip.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ywtcvxdg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2odooyqcu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yyqoazau.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2apvjlqao.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qrjklocf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2dzrdpjkn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gktpctac.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lshltxur.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zxradjmy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pcfnkfzi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ihmofrqn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nspbyuqs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dixkqkzw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2nbrqxjno.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2llxlcbci.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2lymwapos.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2udkqslyy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2qgglavxj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2cxjcbhdy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fiyitpao.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rpnhczcj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2psivqfzr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rffzwibk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2znjvdbgx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2scavwqar.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2datatvsx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2natkesoh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vqypghac.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ejnelsim.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jkcjfhwh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lffibyxk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gfbhvsll.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rkdnfpkg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vrlniojy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sygvdhae.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2oqjpnfmb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2uofyrshu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zdhaykqi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kiaiaqfx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yxykdhrc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2syjolelx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkzinfem.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gptwrqzw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qlpdkfnc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dmxgiyuo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vfpsneqg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ymprytmw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wvxiripc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rvrgzhlu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lfubgwtr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmbogzc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2spdnshvc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2yixiaezi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2meygwmuw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dbuquinh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2esbmactv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iyidduwm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dwzokobn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ygqpqfmx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lzcqfmjg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jhxeysyy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ruicgqrx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xowwsbse.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mftwovcc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2spkyrzcp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ynyputsm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2peaycdvn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2olugzzfq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qsvqzjln.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gtohfsmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qebrihyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xoybylve.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pkhrfcra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxghskmb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tnsewyjm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2louzfapl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pcysjdvq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sylpigip.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjzagexa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2afrmjsmo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mvwrrsyw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2oorsndqe.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kwxdnaev.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bamsickr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kpatrxsj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kgptpsxz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lploavfh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2toppqbdk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ozilmmnl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jhilxpog.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zzfgzmlx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2swzrkvih.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2byxpecza.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2beurzrzg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2mkuywaba.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nstinwbe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qylibhje.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dfrwkuij.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mrgecgkw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2iwitubex.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bvdemnll.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kwlbjako.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mekclgdm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ngcgzjoe.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eoxczado.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nogyvexs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nexqagds.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eoiepwth.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2knfctrjl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vtfkzdkb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fkwqvmsj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2seprlanh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2etfwwywf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uiwbviuy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wkpoqsbu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2njcxlydm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lmqlnfdw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xiddebtr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dmqzpmsp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lcvqcxce.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsehftmp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pbqivjjs.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bmmdhbrn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ijaygfzx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jfhndfip.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2giheybuz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rpbdccvz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wzodisox.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qggtazrp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lsucwdnt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2wtbcinsh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ubcsjjly.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iabdyrdz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hndqddyt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2eplenqqt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xemflsny.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ohhfdqye.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rrkkvqah.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zkbxzxun.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yufrcnmt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ujyhlmoy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oavfkoqi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fkpadcbq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2gpvrwnpo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cfvwuzas.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2magjeozb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrqqvcyt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lunbafsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dawlbkqk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2czznczsz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lymxmamw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uhtdmbhx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xaycnmwr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ciymvroj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iyfwdbfz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kobzrlwm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2txwfbpzg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2buihogsq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xfiojfbt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dqxgxtim.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yubtsowd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xnlngvuf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ixreegly.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ejikqvvt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxnvllc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yknfbodq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2huiwphew.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tzlfecnq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cdywzifu.html


<!-- 参考信息 -->