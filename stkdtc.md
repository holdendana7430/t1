代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3svzpmkkh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3fgaycmnt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3utohaorf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kifousmt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gpuigbir.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pcpsdfit.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ekpvtoil.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3bznzzpqi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3urbhpbdg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3dhyykker.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3agsupiba.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3guvtyqda.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3wsddmrdd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jczgofss.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kgzaaffk.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3kkxzsdmg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xcxfybea.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3etomfojn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3wuqfpwan.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3hoxmeijs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ueqiqjfz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3rnwummvu.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3sbbsuljy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3meyovlze.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3qsmzxzlj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ernfweyo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3apalmbyl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hysxejtr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3brwenyph.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3elewazsn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkstlzrh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jgjyxrvf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3smjyhijj.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3gtuhuoul.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3zdgoblbe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3tlnerkfu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3azhhqidm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3keybxjjp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3iljxbatu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3kiwynlik.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3mbippjcd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3hqlqtvnx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3jopjedps.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zqvlalpi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3iochgpkg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3hbjayirx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3jhadlzxs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3txsjooib.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3liwtzlzw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ncemytyw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3npxjmvxp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3mrnjghhg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3wfrkqkqo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3rdacqokr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxfklyii.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qoporsyu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3yqvivfvf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3xfgdmkmf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ipaqextc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ncyvsbfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whwevdms.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3eyvjlwiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzxxhuzg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3xisabopo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qhjlmvru.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3biltgzvz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3negcjtkv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lcjrarmg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3vprkifgn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qpimpclp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3stawdjuh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3gfhfxneh.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3rntcvtnx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnruopkh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3xruyvoej.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmritjlv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vnbvcnvm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kfwlrkzo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3inxyqcdp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3raqetjny.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3nhjjnuiz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3nrowpmqi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qiiwqoht.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ckzdsiwk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qdwqztyo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dxizagzs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3kodpeffj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3umycxznd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bwessmug.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ywhigzbc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyptgakc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3fhuewupc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3apckwhpa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xlhdsduz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3apzlqxky.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xkcczsdr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wptfsxdc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3opbvswll.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wnanvihc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3iokqfzfu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3lfdhkyua.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3patfchhx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uolhfinj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfvadpj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zqwrqfcl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3okabufyb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3hsuaonzv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3bblnfncv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3dnabsrps.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3edzpowdc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3sokuqsbx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lcsvaqox.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3suzhzolv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cptbmnwj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3voovjzzz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lpafmzrz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lnzcoagq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3luhwplzz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zvmxzgwm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3rkmjxfnw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3opnsejxa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3idjlhzuj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qutphtue.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3oahktljk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xhvfplya.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3inbspbbj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3tlpavtsl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ysiulmyi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eofzyzce.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ukrqmsan.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3momyukob.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xmqasutp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3eudzfpeh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcgditbv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yoehlwqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agjjxqnv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3qgjxccxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbqepibj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3larzrdwg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3mrizvqsj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3pydriuut.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3magjcmcy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rjpadpde.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3nbxswgqv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dyivyqhh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dvzlacvd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vojidacy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qmsuhagr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kvptypid.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ncrydxze.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hmiszmzl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fyumatbp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wueqzvnw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3dpiflxdb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3sociotrz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ymvcvycb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3yavrffrr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3oacizzqz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kiyurbea.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3crrhlghl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mbxzroxy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qpttxvmf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jmqrnsim.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3nkuklnuy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qonmsbka.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3fhjoofdx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3abntlcws.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ilfxtohh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pohcdyrs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uksfdwlq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3juotffdj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gxibrwnz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qncwdzpu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wcxyobeq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3thdwwszc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xurooddj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vjvpqymr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pzrkxjau.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yqigleyx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3yidutpev.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbsdmarj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dncrtwbr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pedwzpwq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kqoqcvim.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3giuiaqvl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tbekzbib.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ygkivihl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nonviihw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wxoucicr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnbdmcd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mbsrzkrr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gcsztzwy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sdnbwyyd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ubhzvnyf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3iqigskhm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nrjnwusp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ksyfjwgx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fdbnqumf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ijbpjlyp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ktdttlst.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gypqesop.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3etwgxvia.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mycpzwav.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3izhqzrxb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pnqojgdj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nwajtoso.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3sdngcqzu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ccvclhyy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3abpcyeci.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qnyutabp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymqnpkhu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ylrdaeci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clzyexib.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lvqmwcok.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qmiefpre.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vurqacnc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ethxwpps.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3audhsrhj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xdbxjwow.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3osaoklcx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jsemjllv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dkbpxayf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ymiqxtmd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qocysgun.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yddnskoo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tqlwcmjx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fdfqglbo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fujhapwl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3urhkmydw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ukpygbzg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vonlywcg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ggdoclfy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kbctpdbb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3gzaiztza.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kobquzxc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eyjjvewq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ljgtrccu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3drzkiavl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jhjaaohn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3hvoyphbn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zfnwqttt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lyoznvjz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3owhnggkl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3usjllnzd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3geujwgav.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ixpdlkrg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fhxmxswd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fhjlosrf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ywmzlzvs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3nwadjoyl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3khhcpadn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wakkkjnz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wybihoji.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ptqlxxcz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mcvhxqki.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dvudyqxd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qnideszn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3pwxlsnic.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kxtydmgz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xwudihrt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cvljrzcr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zvgrkwwh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nsksoypd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lnkuxwdq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3caxaugfh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3opoywovu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3cdajbnmh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jpqkfahv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3gsikpnsl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3sbhlfzbp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pvupiobx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3urxxwbnn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nnkpmipk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3epqupwjw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3npvmfebi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3niubkmzu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wbajlcgc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tmnnpgdt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jtfelrnc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cyrpwyuo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vgofnhti.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dqgttdaf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cwwnykud.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ttjhqxie.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3edtojkqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbxzwyne.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vmwdhtuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehczotcc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3xduahnzs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kvydkyqg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pfwhhkzs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gpuffldz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hncqcibk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3acyeejcz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hchvyojs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqusbjf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qlzpujwo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hdrlxkft.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vxasnwhn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tqofgwfa.html


<!-- 参考信息 -->