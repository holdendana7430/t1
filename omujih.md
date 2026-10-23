代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3rlyvixff.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wwgemowv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nfgmstff.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxortfyd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbwqvyi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mvwibmzx.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3hsyhkogl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3zofpkmjw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3qshwzcvn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jftnlyar.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vwuvemxl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3uirvonja.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dyutxcpx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3azpbsafk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ndtzoxyc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3cxrcmcmp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3bwabpeyd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3uvybkaot.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3fkisxzsi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xdbmssjl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3uejtzozm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3owongepc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3mrksvuio.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ajywtauf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3tdmvyqmo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3aravbmnb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3nqsghpab.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3qjdmeihi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3rqirardb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjvyvpda.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3zvpmbsim.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cxtuxmri.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lknckazh.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3dtrynlfm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3jnaodump.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3prxfasqi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3evljwtkm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3slqzjzam.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3pzgmnbnb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3sbnyzoks.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3oewoajws.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3oyqfhhqi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3cccrzkgk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3wgoqiqoa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ksknmefz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xogqjgun.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3atnmegjx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3bwitnemh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3rsdqrwnk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3vkdtayji.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3tcolpnly.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3hemhcntd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3mlxmskez.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3yurltpem.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3imaysfxd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kqwaslfc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzozurss.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3lbexzsbc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3pnxtjxpb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgipkeyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywkawtog.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3pxbhquqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbqmxyvy.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3qwtlkovj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3oujidjhe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ppfhwfdx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hvhgtkav.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3woktzzyz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3rfbrlpgs.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aocskkds.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3bzvnwtcr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eidznqha.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ptkhbtys.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imnxzzkc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3mhicfzsa.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrchdcp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mclbjkyg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3noqwvhvn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3fatiuxoa.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuncltfy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhuzixx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3tvpkiddu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cgkpejfa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hrhipsvk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3eegugdzk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3uphcnexp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3lpppnjka.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3mhvldmno.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vnzzhulr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dbmqjgum.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rkgehsit.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sfvyrgnr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3oroxfdgz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qgasbdqq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxyxgihc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3twhrbcpg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uijrclwv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xkpqrqjt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nzpjvntw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3tpiousct.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ppuxbajg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3mrlbbyoq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mlcwesxj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ebmjcnnr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3crqkefej.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3pvczldll.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wlriiyim.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3egaqeepb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3rjckpaed.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kvvuqfno.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vsujyfqf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hbyhanqa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vsjjsuti.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3qhjlicnw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ovpgcxke.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vsqxngdo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hvxadjjj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hkxvhfvz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qalgfuad.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ziinhkqi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mfmreggn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qgnhjaun.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvfwipa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cczkfoil.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3fxdoegqh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tnoizrqq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3aiwtdqcj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3rmydmeva.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3wbutzcaj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nfdswale.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dpkivlij.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3plkifssz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3dxfcnekb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3aipgxuzm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ugkzhtxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atwntvvb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dfcmjynl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enkqgoob.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ralnsvnu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bvxubwne.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3laxcydks.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3skkmosaj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3neockigf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vqxprzxr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3iphvzzze.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xzorrgwb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uawuobit.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eeabfekt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tlrsiyoi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tfamxnon.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lruhltws.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uidysyiu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lkanwgpg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qppqfpsj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xqxasjqz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3aggcwggi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dnvlofda.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3etdsyeze.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aamjnfaj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ceetdtvd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xvugsjei.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3gcrtfuje.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tenmypsf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3bnlwxsva.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aaajfhqo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ihksutfd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3esikzgwo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mtoieqvo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ptiiqsds.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3phwffqpc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ygunyxyr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xayuyahw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vgepwbwy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bynrziqh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3fdpsqluf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qffvqgcm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qfqflbcp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3eibevavw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qshgjzxz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3swoesnil.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jgelatzc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3prfoylix.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uahfibws.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ejyxtigs.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oytrzckx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3irfgbbzj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mxjxcvpa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uesitjok.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hdmfubxk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ytlrwllu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jqorfbft.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pzvdiyko.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sgyyzotz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gzxfmmic.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ejtvrnjw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3esmpoleo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nsjfvgup.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fzjgxftd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sjjuejas.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3thrsopxq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rqgnyjep.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dgtsxeuc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vhzdklhq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wntrlpbh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ssiaprky.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hzihqfzg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3egiymcaj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3saxbauly.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3adcoighr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xcumvhgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byupjyzy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fjhqpwsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrcjhhcy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ecytqrqs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jsgshrpe.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wwktvhaf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hwrkplol.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pihfuctt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vnzlspvp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bwhvxemq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ixctnzdl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jyvdgdlm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mkuhozwv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eetzpgcz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xlllgnrw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dvthfgeb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ouqouvsg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ldrlpdwz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3swxlgjsa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mjcsxigy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3byqhcdwy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vbdlkqub.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qjatkqjj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wwvflfrh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pfccmqzw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fskvdzov.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bfpybchp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3filgjyhr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3miliotff.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3esmgdfnl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jilihkwk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rqlrfqgz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dhqobbed.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3slkqrkae.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3elqrkogg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wrvdtqaa.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fbscxdcu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vhpzslrk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zpuquaij.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rmqtkjgv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kamugrph.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cwfmfpch.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wjkvwlny.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mhpnbcdv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wytzukpb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kebtytpe.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xmjuuxug.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zcztmvmq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qqzpwqww.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dzclgrou.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bctelzcw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yzandtar.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uqevjtwp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dqdfgudy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3afnxwbad.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nbouojuk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ngacyfhe.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pfjlnent.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3chpgnyvj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ytnfgbhg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ynjwrlno.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fimkmjwh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3dnvjltpk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rpidyrts.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rblcxvpt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sdkznbtt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wbfftirp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uejruisl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kuyaylwy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nzlunkci.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xtzyythx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3amuwkjye.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ugeabnpz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3dyzblbag.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rzhtzfow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igqlspmo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3befbseay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rejccaav.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lrgozqyp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hdowjylf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rhkuacbs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3beoawzdj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3alslphfz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hndbopla.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwceiask.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xdlwoudf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgrxmbyx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gkjgkejf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hkfyjmpd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mhqfjwwv.html


<!-- 参考信息 -->