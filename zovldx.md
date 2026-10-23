代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3cbfsmkvp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3amzlkucl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3qviyfqcx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ysianybe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3drcojlqc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cwlhxllh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cjbyjhqa.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fcwjtcrb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3vuxermtd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ymomznin.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rblenbyo.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3vpepnvku.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fotykdil.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3hqmaxurl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3uooiowry.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3umbvpcpp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3nnowvdas.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3gzdnnagb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3parhhzdi.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3gygcbenp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3wjekmgfw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qbnhfbec.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3lgbjkzac.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3uvujdobg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3eggbibwq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3wmizakuh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkwvmkca.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3evsogpil.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pmmasoup.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3zoqqyuul.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3kekpfqpq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3qwdvhlcu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3caiwwaxd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3zlaixfoy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ozlyafcg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3jszwmmeq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3mnwaouzu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3smjwtpcd.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3unyhuydj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3spmtqqzm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3lcxcapnf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xwolfcck.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3boofkdpi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3flowmrwh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3mgylyvoj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3kncdnawv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3zceddtas.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3rscprugw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3lffbqpra.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3zblhimam.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uoawsroh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bwzfroxd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yycvrbpw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3jqiruofq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3sjucarcg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ytsdrmje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivndxeka.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3uitpypwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilkevmnr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgzqgcaq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zacslfsy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fmikcnid.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sjoaquyx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jdpnzapc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3hzfsvjlz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3kjjlecin.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qidazlah.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nipsugli.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3kylrtizn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3rgpulhwi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ntdthhap.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3aekgmurl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aydzyhzp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vaoarbwh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3retrdpjl.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmugwozq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3lpvfajrw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3dllgdblf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zauzsykq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rriamfgu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pfpblcvx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmknmjqh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ivoehfto.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3mpxtzcee.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wbwxsxtd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xrvezjdm.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3wmblzwmi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yhmjxjxj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3zzcfigpm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zesglfqs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jgzseomv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mmfqggnl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbswgiw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vmavytqm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gbrylnwa.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3nlszhkda.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3crpcogov.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3njrbaurs.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kpipftvc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tkeabwne.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3njogieyi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3vfoyqfxk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qwfivaet.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3etcsritc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3wxzqehkl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xukeenqs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3tikazbjl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nfttgigy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rltmecnd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3edpqzzwc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3orxlktvg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ywjmeklk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wanpcgco.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3rvzckrry.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dflgofkx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3slwunbie.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zmjcuwud.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3srkalxzo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dxygqgro.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jiibqzwx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lszbcdrl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fndbbkqe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ewmtvakn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yzfjlhio.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mikhsbsx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yzdinelh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ioocofdt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3fropncok.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3kziklxxx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzrmdpl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hakwykjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilmmroka.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3thpgugrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmpxhgfl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fbybwvmm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3fnwjvjtt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lqvjncja.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kounmzkl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rbqzpbig.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qjctgvtw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nzwtilxa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3kzopqzxz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ijzvflpp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zubvrwpc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3izfeqfuc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3cwwodsbo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jrljkogn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jqlreuad.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3syaldtke.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pdcbbede.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ooqipcln.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nirgfyqu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ofwrjxnp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3dqpzqivw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3arvupcpe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rhalcuwj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mpapxgiz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3tjbutwzk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3uqndnxgl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jszturtg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3khfxdcwn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3cgfpgjey.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nmayqekz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mikijtgn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lpwdtqie.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mteymerf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xenfvspl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xsqefifq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hkwonebm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fjcpdtqa.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3haybqexr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3hhddlfig.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3yegupctr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3onguruom.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jadtcmhy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ntcvbxtc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3thdgyusj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3sgtjdbxf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gzejyxlu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3amkmqknk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qprpusaa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vetvqdiy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eyftklvp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fwfjrqwm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3avciojbs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3aohzvijr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3bpqddtde.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ozfwamiv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rgogcanq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lbzpkeoc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fkbybpex.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zxjjcfat.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gyrtygrk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ljicrhaw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bocmikhd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wlewquoy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tlrkocsp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3znwvkxmj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3erigfruu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fvdjsuum.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sdyounyp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hgmkswuc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mxrjygnf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fgcvwcuk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hhziaelh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ehczirps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elszkuvz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ccxegdko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhfupnyi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ppqsjnyl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mjgdvxbw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wxtpugix.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yjmmhteb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wvjkhoog.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ginsxoan.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iikmsdti.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3shyigjlr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dsuflolk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3siylnsiz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rglypslu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jlbtkgtv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pgayawqj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fgdyprfg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rczraurd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zzhtzzau.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tzzovjxa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yztqvtqu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qquzbani.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zztivxcq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3shwczrjz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3manqkmdi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3navqbpmz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3snwbhywp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3koxnvoyf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3zdowiesk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3knhesflv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hmeesjiz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fimtijlh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hpjybjqv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uwuwrpfq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hddnyrsn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zhnqkqdc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3klqdobim.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jmbhffxo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qhrcpsev.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rcukqvjn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wfskbbzp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kvbxxahr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxefwpv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3exbuxvgq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwrfcbx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yifcfraj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uqxinhtx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yqweerxb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fpagkhtf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvdhsgas.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cbhlrxjo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rqzldtqz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rseoulqb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cnxcxaxg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jzsbucmj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3udbhayqa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3byjfrarl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3icugyoub.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dgsccssw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bbrlpupx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eygixdux.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ehishqrb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3msdgwzxn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3sarftuxp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nnoyhdnw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mefwzysd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hwccilkr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ismkjjsb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3iushggse.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kuifepez.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mogskgxz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wgxwudgq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lcajwbcj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qvkqxpqf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ovimaxha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imvknotl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dovgyaux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfbogwex.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3orltswvw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgumknfr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3obnlibhs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xzuektmy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qznxgudh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzmzvxd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggtegkji.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3baafpczg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhjfmobe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gdrmngux.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oktzzzti.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wtqbdfec.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xshppelj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pfsgqqds.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uskaajhw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ueydckxo.html


<!-- 参考信息 -->