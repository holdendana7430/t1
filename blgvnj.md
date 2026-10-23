代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgyewgi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3oujtcngn.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3kaecbgvk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvbosuv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3sonxpbvm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3sqlysayc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3frmdfuyk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3jliibqxb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3njbrfzze.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3zdogjfqo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3yxuoqfvq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3uqohfqqw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3zrcpfhzd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3tuvrrjux.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3lzzkcese.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3yueuuyel.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3teigstjx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3yckwlssq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3mvfdmzxl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3lafrxvxu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3fxdimkjp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xbnrffag.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3prucdmys.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gheblieo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gkdegiqs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3aywvauxo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3udvmwynz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rkbpsxac.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3glqicqbe.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3reqnvltv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3zgymituz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3vhvgzhcv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3lfgtmomj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3btmnglpy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3tesifern.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3usbenonz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vrjrjvsj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3tsmsnapy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3zcxelfpc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3tiepzlfw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3vtsyourq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ghvcdyrg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3niwuymib.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3loaiwegb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kqobfvln.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3xdgovwlk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ahjlqcoh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3arwtorlz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qallejdo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3opczgotl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygzeqnfh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uhmhqunb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqxuzdjj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3cywzedzp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ioaoqvaz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3rrfrbpuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mepqlnig.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3zxetmfit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjcqqqhp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3smjpuobn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hivtyuox.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3shvdjvyu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xaprdgzu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3sgkhllqa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3rhornskw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lvcvsinb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3nxuvzecw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3tiszmiev.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3tskijmzb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cakmhlrh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3upmcbevl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3aatvhmii.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wbeotdcb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fqlxckgg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3evirxnqv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3volhynpk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qictujeg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3pbxkcrhr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3nfkjinsj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hseixepm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wzlqtqfl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3eodqyoiv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kacxlfcd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3bpogrwtf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eztvbdoy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3cawpafua.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3dfagxgoa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3omlxcpvy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3sqfcsrdo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bqzuqkag.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gnvimlnp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gmzuthor.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fnljfkan.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3chrkqtps.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqlsstwx.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3meeunufq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ulzyadgh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3rmntblij.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rxfkgwfo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yvdoohfx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3vjaodsth.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ckicksns.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3saswkajw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3uezptvtz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3livkpjmy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cctoovbu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3iwcmvssv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xldabosa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3llntuuoa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ztzgdrlw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gmimtxpx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yutlxfuc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wunnfgtk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3crnwpujz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3buupnned.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3wqvneajv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wibypijc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zharoztj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3grfjdhbn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wbhjpmat.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kywtgxbu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqcqskt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hjkdrugd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3rvdegegz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ypddsygg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mlamoucr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ufjsvhqe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wgrjvcwx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3llubisro.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3okiawomh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wxdlokzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkjjwlxr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3lpswdssw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjcqlquy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3isxdjjry.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3grozrbfj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3nlrccild.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cttklfcm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zjwanbtw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3elqoplxg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ybstermw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nedwjhle.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ftnylovu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tqafyusj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qflctfge.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3tqhydzni.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3igqqkpka.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ycctogdw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3khsqjsoh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3kmobrbce.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3sumpletn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3nxwmapkp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gwdrggtt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3dabiaecj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3uisuzjde.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hzfietdc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3utgdcuvj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3wkoztzwn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mlilixwd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dhjrumho.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ulfbibdu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bzenegdb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3cehdvvfg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vnqxagkl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3njvugldm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dxwtnjit.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3kzyispfp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3dtzkjvgn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bxtmslrh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oiyzgzof.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ksoywdzj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bfnfwvej.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zjqvpdpk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cjohipsc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kugjvwhg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3kqoopzni.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3unegxzcx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3rxpknjvg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdodsuie.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fvpztuyj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kdimsftm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3nihuktqj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gomgembx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dfnjybmy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3goqodlwk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lsxenkud.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjgyiab.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tjfrfjnx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3awuvbstg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hdzeifix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lhekpylj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qelbapel.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jnnbepvc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zamjtevk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pwnubbub.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wongbvxw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ngzfusis.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vmiyhoxt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3itctgsqo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3puihzsos.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3teysmywg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vyriwyfx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3okgektya.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3nxxwsvdr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xqngygto.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ztjtiyyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rotlgwax.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lyapbvkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrouzajm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktwiydng.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ctvxvuud.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hgfrgkge.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuditbwg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymirrjxa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xlpunqnz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cbhjwxkv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vdcfmmbw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mguvfrxc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rawnjikl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zucdofve.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bpgefjkn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xuhapksy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3javnhohw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pfqbnjfi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3blqkqbwd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zpantnhh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zemqayhp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3htcvvwco.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3lzrcrjpi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3spqjoxru.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rydwqtnb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uzozeumc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3yovuafoh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xztxafcx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3sheixdqq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3psujptdm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3edzxqsvr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3tirsrfnq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xnfqedjm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yfqgsluq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ddgagwba.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yozfsvgg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3utovsgur.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tcjmysbs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3oikcdkxb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3oenjfrsd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dffzdzqa.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zkclefjz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kqzkxpsu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cncrcwlr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkbxpekt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3attprcvr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xntqzbui.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yrtpcujx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bpgzlknb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvrbongf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mkamqlna.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lozxohhc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vnlaajve.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3stcywhbe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qrtghkre.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vpjddcap.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mgkxjjgo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yzajyqcr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ardbjmkl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ubqceejf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rxjlnoix.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vycviwte.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gvinlogw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mfcrxbgh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3emidlazn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jdjualrk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3kdtvzohc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jyyxcayi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qvyncuaj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3etisbigr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cbykuxbj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xapjqjox.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3anjkkhht.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3teijvujb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uogswwqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tusrwvjo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mnfzrodi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnmdqbmr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iuoccakt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ukunnkyu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kxymynyc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sypcydjb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eyxeixhv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eevcwcrp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifhwtzcu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kzznldff.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fcmsbohs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3sytynfsm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bqjraumi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kbygnsyk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vxedauho.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nakgawfk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3agwctbse.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wqsdwamh.html


<!-- 参考信息 -->