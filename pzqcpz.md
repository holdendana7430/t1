代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hknsmztn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3uoambenw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3jbsfffwu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3bpbilfls.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3doblnccg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cmayomhh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3wivdqlpx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3qccstdxs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ddqfeksq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ejqneibb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jthdfxza.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3rlundrgk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3gzgdyjgb.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3yduanqld.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ayrnpgxz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3igowpzsi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xbtlcnay.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3hntsqlil.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3pvamcgam.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3hmirgkhl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zxoditzd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ezorqzxg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3cudkrcky.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3okybgdvh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ivthhiio.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lwwqrvfs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ktqoxlky.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rbmxjwuk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3amqltlia.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ayjhthyl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3rbseskzf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3aasqpenv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xoimnsji.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ytmdbrep.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3oiuyrplw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3uwjlbduq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3rnthlikf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3txvsrive.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3xvjylvep.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3zcrzxtpy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3wqlxnxlg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mscljuno.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3fkplvmlm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ufqkhpcb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3zjoejssa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yxtdwzoz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3skmfhyfa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gojtnncl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3hrclzezz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3uqbjwudv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3lsjeqemk.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3gwowmhjq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbgnntnq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3wtlkehuv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3vxntexwd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3orkagdxv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3wfuwnizn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3itgtrfce.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3fbhmqtxo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3vnkcmeos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqkbgdeh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3truythyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrhbbizm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ljfxxlod.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3eljqzhco.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wncsxfza.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3cegytunn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nlfriavc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3wlhyxqnt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ercbrxaa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3wgiivntb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3iqjbsfqn.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ultuscfk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjjyxmel.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3gqrkujwf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bubaibcj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqfbftap.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jzsakyzt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zwrxffdx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3egrjntmt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ewjwnngp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3snlushzw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3feaabkaz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mbpaimeu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhrjszjo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfhushuz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3cnqsliai.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3xxuulqmf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qlviqunk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zdxaujjg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3obtjysgy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xabyvsuu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3olwhgiht.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ajipocoz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bkbbjtzm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zuzcsqwo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3csgmfuem.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gpfpwiyx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yhewebyx.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3xwxpheyi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dcizkpqv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3xltmplba.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ucprhtfv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kxxnlcpe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3febucwhv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3owszwagp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bfsesnhy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3nqtezaha.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ocolpucf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dpevfncq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3trcllmlv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hijkrabe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3eqecumha.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ainvgkpj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vttljbrj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cybtjlrd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pcgbzumn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mcapavif.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zrzenake.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hqksveeu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rgenmtvr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3djocsbtc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ujohftwx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3hyzkbgyk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3tppuojsj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rtfnacpe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3siiutigk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3hbzeyxuq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3nxqdivve.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cogxnnli.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uppjfcyp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bbypjncs.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wbjnjmqy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3htnederj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ifkeavuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwfkljse.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xeqsbeql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxncupfy.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ygumnhkl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ifslkxqm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3dfwwhorj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ipucirxd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hmakhype.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3oeltpstv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wttccezx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xosovljk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ckdukggw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tqflvjts.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bhqrxdml.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3dxxaotur.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3czzfdofn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qhflobiw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pnwhinxs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3xfskrvxr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3miwzeeia.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vihewsvn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3cdqjsytm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jbyniczp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3xgnmfobk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3lvexvrrd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mhxsaziw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ppczgqdi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gvoenyzi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3bccgcaeg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3azjzrhke.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3vvlcplzs.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3drcttvqh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fuofwfkm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bghlgsdl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bltgdbrc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bmcnlvob.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mjdyercs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3lywahnou.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sereoinr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qcobftci.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bskqwpgt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3fvltdecu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zspkpcwq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zskpgkcq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hkloxobm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjaqkumf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3rvexybjo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kkrihfov.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ucqontjp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eoqokdhb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3akpsgtvr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nzvyodii.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jozaukjj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dlapyuye.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3dyrnqbuy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3agngqgpn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ozlmkepz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3thoufigj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zafbptyt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fzvkbvnf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3usqivnyf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vcejexzq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fizlsvmf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3inrbdjcr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rwblhspc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wgobiiyw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qqztmqqm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nlkxidhe.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zfzjtkvj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cwkezpbt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oviyqubm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vrdxytbt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dlmxeoja.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rwvlsids.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3edfbqkrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bilvpdtk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3cthjaasn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3budhdyur.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ujhdlzjs.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dnrzfwzy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3amzglvtu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jdsypczn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3odtkdlkx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3verptzkw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vijhynvp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tfryhtdh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kdtvnrwj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3llqhejvb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mqaxzuyn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kpzffqdp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vsbpsvbq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ddmdbotu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hobkcuxp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3inmijshw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ymqutjck.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3isneltmj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3taqnfbnd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pijeghuq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3liozgtln.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bqarxlii.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fifxjbcd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3geazvtxy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3eejebgie.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gjpawtbs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wpbvyzql.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3molivfwb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mclhohqb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xrckvohh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nyvdpwbg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wcrqqxbu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mldqfdnn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3opqbiiil.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3uvtxduvz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rhqjudlh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wiujyofd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohkmwtrc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3anroyjfq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qufyuetx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rdlzhqdt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddzijzxr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zquhqjsc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xtyzkjda.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vonfhfun.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ntanbffc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rfhselsw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3djbemxxb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dnngwgos.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fdquhdyq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xlwsbxvk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pwdjuvwb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3dhuisjwc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zazufxsa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gjaezxnb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3noueealk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3locppuvd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jnfrtwkf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rrlgyxeg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cyinyoce.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hbhmwfpq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ejvtgoxy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kwekfyvd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3logmzdvt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3tgqdvzye.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qpylfmbe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ysvktqts.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3raikgwmx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bjfjzzpn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xfsgrgds.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bqccacuf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rpqzocix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbzohcsb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pfixvpdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlrkyrnn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cwhzljpq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pnufptvz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bixhklwz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qzrpqncw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fwrmhtnh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqndnmwi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tfbcpbks.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3khmjwzvx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hodoemxb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3goqfgcsk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gwmqhwat.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fgjcwfbx.html


<!-- 参考信息 -->