代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2psbbtdeg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nudoxofp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kgblzkme.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2tdjwpztv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2rsycsuho.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2qcxlpttl.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2nirzzibv.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ghgykiti.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2btofgbns.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zqwwfxhb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ruikzmzb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2dnfiqbzn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2npjuommz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2zilxjszz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pvmovcnt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2alwslvis.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2jjecvcei.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2uvpyablu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ouyfcccg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2uzavjjst.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2npaamibo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2cwuwcbns.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2hebclnvz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2hfddexif.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2utsyrtxv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yhjigxqa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ocmpbtfa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2dohjtyvx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tbmbfmxa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nfvcvzac.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2czigrpgb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hadwxoxr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2grqdobki.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2wwykjjty.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2cjetrsml.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2hfqkmwjv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2afmiymef.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2mjykfsqz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2uhnvdrlu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2tyyevpmn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2kjagzorw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2kqzycvst.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2utrfevqi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ylvuhdec.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2bpadrctl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2pvivxgfz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bihjvrwz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bnsfxtdb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ugwpgsjb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2tpljzvxj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2lrhvvgoz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2cqrottdq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2pafvfqaa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2objkumhx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mqkmpuvn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbvtawc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwbzmzp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2lssxwxxp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2tvfdqwhj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2vseokvfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mouvnaqm.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2qxmhloek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyoetmin.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nnruwfja.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xylehgoj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nwtitmeo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2equrfhmp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zshmvngk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2hhrskict.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2osrajkxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2gfopvxix.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxwqrzi.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2hpqxpeit.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2irdtbnda.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2buljafsf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifewosbn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrmjutfx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2spkwzxvh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mdrzrkfh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ifvekzqz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtdeowm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2maxxvvvb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2lalangpr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fzqxecnr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2phewzrbk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ixbzbiam.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2eydidnsp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2mdgcvhhs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2chyfgnig.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2dggtfltq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucupurmk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vjvinoey.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zrqmckwz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qfswdrcf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pzfpgahr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2anwhjiwo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cqejijhr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qgvdemeu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cepjzmkj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2honslype.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2duywhuat.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hrrtljez.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2stjxmjov.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iidxnumd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2dzeewisd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2cqbiseva.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cgkdxtoz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2wxbipmcz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2eoumftoj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2faoorjge.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2rwssmynj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eauhxpbr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2awphdtwm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2zzpwgxbi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uhzrctiy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2riourufi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hqdabklt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2msnekkjh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wymfyhuh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2pcxswujm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sjevjyvn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mazmccit.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2leyijklb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcavovg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdswety.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mgphqvnt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2buyglhph.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2tdpotoiw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uzpgjpss.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nihivmdd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kmleiykb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qkvrjuas.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ubloclfk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ubnsmlkj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2brehbhoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryzloysf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cvxswzdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abmlvpod.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2bsvudrwr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rmujrrgr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2iffhqepc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dpxqrglq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nvyiysde.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2epxfbwxt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hhgiflvq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2cmynfhvn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ddrkwijo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cqsrwbjp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jrnuxvgz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2eltpgsyu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bxibhmqm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mgsymltk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2bumaqxfk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fcjsyfiu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2xaanpygu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qgldcmgf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2sdkndfui.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ofgnovmu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xdssqzzb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2utzyqzmx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2czsnhpsj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2negntqqy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ecpbkjih.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2kubitgcd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kfwogmyh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jnaqffjp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2mqinuiux.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2icbmnsaz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ssflxhic.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2baqoqjpv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xlfppdlb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gdolbnpw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2puictqdt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2piftnxzt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qvsqrpli.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nfvsblgf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ebmzeqhu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vuqfyfhm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wwoowcjv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bvixsvte.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bewtancn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2dlqrvbny.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2swiefyvl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2btbtuotf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mpopmkxn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dnwfczdq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wpfpacao.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qlauzmdk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgluord.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2htenworo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tkxvqwlj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pwxvdpae.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zjmpzjok.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2iwqsrcio.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gqktzuea.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ggpauick.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bcddgcmt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2garzjhxd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gsiogmsr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ftswnzyi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2esgbypkw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2padnhreq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rxoehupp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2zvsowwme.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dstwlvvl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zykrkqrj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mqnkhtvo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gasasnlo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qcbxxopv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rwqxguxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovdrwqgm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ztqewehg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eugxogkz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kzgjlgid.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2obhpurvg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vjjrvhwb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bjosjugh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nwqakgah.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nvfrjymn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xgmjvmxq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tbfbjrzw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uhlasxrf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lubhmwin.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kiqwsixx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dgdulige.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nieyejbv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rfdkgjuo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2irdkptev.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zqusiloc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2dilwburk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gykbmoav.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rjolydas.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zcycgghs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2txlchiio.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ffhljcnp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fuwkllvq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dcfhknaa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vuzpupde.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2juozffdv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2pqvjgtgi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2knhsxkcp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fgngobzc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bjxecaef.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wrtgjnja.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ohkxavvy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tpaasaar.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2samlrhzk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ernwekdq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qxjepxlh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2sgpwusnq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xiwgnnfg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mnfikdav.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bpbycmwf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tixsufsw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pfyolwdd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rnrbvctj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vvpkvjpj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nydccrpo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2stxqgxlb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hkvupbnc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ldmzkhkb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lyfvizww.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dobmbadj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pgenbmve.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hgwwvmfo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cqvebugd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zwubzeqb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nfjoqsyv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rjvvxmqz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gnopxtml.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hxnqaxwi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2etccydkw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yzkeedxo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pmrbaygd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2nakxomfz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vewjbvxq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fhoxbdub.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2utwimhlo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2uzrrreno.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lwjcouhq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tmuohocz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2maobolns.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2omhukykz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kmcelmrr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nwayqawd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgbdasdv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pgjmidxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhdluhhd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hxkuzfxj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gpsxciiv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dismwskd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vqofovzu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xrquujtk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wjbskccj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2owcdnyoi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mjazsbrz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qyfksgzc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rrrirmio.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wjyrblku.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ldmsumoa.html


<!-- 参考信息 -->