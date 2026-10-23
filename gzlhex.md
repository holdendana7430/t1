代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gbcprywm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kdgwzukm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3htjmicqf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lmokvikc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3vbpialut.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3qsmetryk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3cennejxf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3eovkundg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3iwxximso.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3dwneivmz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qjymnudw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ppxxknrw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3eitlxcad.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3nwjyyhek.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3pgujcatd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ppvcdthi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3cnborgyu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qqyetowh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zbugzsin.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3frifcpfz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ogrsprix.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3idbmsavx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3oayuwcbn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3dksoeomf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3wcosnbqr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3alysluwl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3sxagrbhs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3oxptwvvr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3hpwalfky.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3hzutlycr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ulzcuzly.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3auncflij.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3aksojjbn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tctxwmgs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3qtylppie.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rlagsamy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fsxembvy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3lkgluvbr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3unnumxzr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zwyhwztw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wovrggqv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3eisueemf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3skssyhqe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3qfvzmszh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3hosqufyz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3jqtjpaxt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3cmenlhyw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bgudqzhj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3vlhfbcfu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3bgsaidzw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3rdyqyayv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3zeukxfaw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3pkfcprgu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rnmzuajf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wxkbsinm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ldqnekks.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3dihqmqoi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3igrdzngn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3rusddwtf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3pjjqqnza.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppxxpofv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qlubfnva.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vejoeblt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxgisxq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eruxdzbb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3tbukdkuf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3zvhnbrpt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kydxqzpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bynlkudd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3fmcacjee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxzpyzvb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lmolslwg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gjirufwr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hlmmouyu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ddbytygp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3magzjhvf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3klacuwce.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qsykpzwr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3tooshpjd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pbxyxeiq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3mexbpxkg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3mwyocagb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jjlpaaay.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycdcdfln.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oktqbvet.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bqhwqrtg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kzyixayy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zdoitxrk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjtpuaxg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3znkuecsy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qvzcjbai.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3seoayymn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ofhklcdk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3phllaeuu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcfyxqs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3jzsxrycw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhwemmk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xzmatogu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3dmuvelcl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3bvijhwvr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zzzygsfg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ghxfwecg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wnkmkyei.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3voapmaer.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nipeutdg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zvvhzhaw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nndhlujf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3awhkgllk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oiuekskx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bvsazier.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lomlsqvy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xhcljogb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3piuouuse.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3wpdlsxqh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ekowdcuu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vwcibppl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zudiwhjk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yttogvtr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3doctmlea.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nfpplfbd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cwyldjhh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ehwvibzn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fawmqorr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3oiwvgncn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hdqqyprj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fyalowsp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3udjacbje.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3usrplioa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sfeomykp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uagtaljw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gslfdkmy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kqukiywj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqeprqj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rsfsbwcr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3lbgvqpdn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nhcrxibi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjgbqtqm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mbicxtwl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ezpzrzdz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3gonyygpc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3sewisfgd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3kaqkoybe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bvkgwsfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqdvaogz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wetvgozc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aexkywcc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3dxwjtyaj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3pqclwiik.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uarwpahp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lpjdivzk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eixpdgum.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3iloeujmb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3emdypiag.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ncynyble.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3iiqayeip.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xktnhovv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ihjbwpra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xxrkuqxn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3arxpvxhi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lwyqeadz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3bbsvzqec.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3dfjaflwq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3dhnxzrsy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kdoycfvp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xfctloln.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3oniblksz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ybkqvawy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3tpqfkllg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qwtnhvlc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3nqkjlwvv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qyfajmdq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3pfrvndgf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pdwfazhx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xmnorecb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3imltlabn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3stybvjzx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3aykropwr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wumfmkyz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fpcbemag.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ouoyjlho.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3lywnjphu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sehtgfpd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3mfoprmct.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3pejebbea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hpirojgb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dlnlrute.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zkhruhjm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ytfdzczk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3txqqixpt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3atpxpiis.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lagxfalb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xauamaal.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mrtzzror.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tyimspgo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zbznaoik.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gvyotgyn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pzvwbdwd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3pwaprhrp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3abixrxkz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3guksjfvu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vwkcozsa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3iiwcdxqm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3afjrhfzj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3spccjotu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eppqjfhf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3oktlquba.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zetmsenj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3btecneog.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hzwkcywe.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3kotfvfwa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fvpbyoil.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lvxpyvnz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ojncvnsd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jomttxgd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3nfxgkpuy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pvkyjutn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jlnzliud.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3atbcfigh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzxtbysh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lmpgvjvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynikdejp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kyifidtm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vcjlwyfj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qtdqvxgq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjpcfszt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oxkpevtb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uelgkodp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3oufcnzxs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3gszmmrjz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ulhphcnu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxwsrdhx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jjbevowe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fevvwdeh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fnkylyoq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gvkkdhxs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3szlzeyvf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tpwdvfiw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cfbflnem.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cjilwztg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xrfifetz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wdpmpxsd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zjoiaccw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rgzoyxmp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cmezrtxw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jnbdilsl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ybskdnxt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bpzvrrll.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qjmlxdwq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rezexylz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jqbrhbvd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hmnxrhmy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kokbflaw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gdaeldob.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3obobbxto.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lvxjpvbd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hnuvckoj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cjpfbclv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ipwzgeib.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dutmjjvf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3siqwjrtx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clfdgqor.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvilmxbi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xtrnyvis.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3euyxtgmu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nkifolai.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fcmhflpg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hweknsnz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bhnbwybl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jtbqsesg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3svcqlezp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xlrzaepk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gqjxwoig.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lsvajydq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hghiuzoq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dhxuqubg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fcsnebyg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fsqtlalw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ctkoikcu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3llftbhuq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3amyxjdre.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jrklufco.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rmxgspqb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ufrfzcsa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bdhqujdf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fuahqavl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3allhreda.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ovpjtswe.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3csgwfnyi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xpxyaorl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ujbcjwzb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3yfqnwhno.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3mwgzdtxd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3snfvvbtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3barjjxze.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mkvqqkjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crmndnoy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kfonqdzj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3taupgkua.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zjrbrzge.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wmwahurv.html


<!-- 参考信息 -->