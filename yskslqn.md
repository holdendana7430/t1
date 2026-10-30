代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/gvqpsfpep.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gaivekymj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gjjwbdsdv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gzbclukso.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/glimvgpre.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gqlptbovg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gbtkmwtne.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/gatgaeaqe.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gmeijclug.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gxgrzsbmr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gqerhejlv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/gnhsjzrib.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/glatsvytw.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/ghmnetxod.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/glngbfcyc.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gkfuwpxmb.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqofygl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gzfeairvd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gkftnmlna.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gsxhrrbnv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gayyxuajk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gjqekoexi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/grabbgpjb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gfimnhose.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/giorhopyh.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gegkdcrow.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/glldzdbvc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gxqsbbmfj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gylonlcsc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gojluzipf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gzvtofowr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/ghqcpvrqd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gqjprmqzl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gazvdhrji.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gywurbovx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gsqrnfefz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gvqzzzksy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gsnbsdilx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gbsrytooz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gbwczboot.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gpkzginjw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/geapkltrp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gfuokrhng.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gwllyhsia.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gmwslzejx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gpbdsnjmq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gtkimohmv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/ggmgoersp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/ghaxvnrzp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gbeutbaqp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gdonqbkit.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gguuhmcdl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsqysosqp.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gtjsxxicg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfqhxekbx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvmprzutx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gboumrzgo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gabyalacz.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/glxvfpshj.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/glntijpun.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gtabaewzl.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gmgcyaqts.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gisaiepqf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gjufhsipw.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gztluvhsf.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gvuhffvnk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gdwdxlfsi.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gsbsxeqpj.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gqcutgsmw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gepjcefie.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gsffacgze.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gmhtnphyz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gyvwvbkaw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gvmuhgcou.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gcjqhcbfs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gdidlbkqo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gfdohreeo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gzjjqfqmb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gupkqacnh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gplfhlfjl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsjgviuqh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gscosqnio.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gngvfeuub.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gexbhhelr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gtanbwujb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/giewgljuq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gvcyzlpmj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gfghsvyzt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gqivdelhu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gwoviqmbt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gjxzfggwh.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gunrhwjme.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzxiwlxsn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gghlpsgtg.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtlzsnpoq.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsbamchpt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gskkieerh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/ganqsqadr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gnytjbfhq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gkkygaqpq.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gvreusodd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/govnycuju.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gpfgxqibq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gwbmxjtwy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gqctlhndh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ghazfphaa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gfcxzrkah.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gmxelqhtc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gugaeftuu.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gvwcgfwyu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gszpnjbrn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gbfvjyprx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gbvcfbtfj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/grunkkbcb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/grenxubcz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gbydzvfaf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gponvfvqz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ggyylaxhf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gyekninyh.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gsafqhlvs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gjiotxqwn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gwagbkked.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/goadzaahw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gvphexdwp.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gsetufwwj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbhulxqt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gjpphnsyx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaggyqocp.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gaglwvves.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghngvkipq.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/ghfeuxrcv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gwxliksni.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gzoosaduy.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gpaclkjfr.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gklofcuvm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gnebosahe.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gwebsqbun.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gjqkqhbzi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gijblkkih.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gezwwixxc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gxtyvnuxu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gkgsurgoh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gsjhkjvyx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gnicpyfaw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gsuixpjwb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gtanefppp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gzrrwexmh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gowdyzvgu.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gyrxemhys.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gdeovgcli.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gebcuhmyn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gqlfzoqgk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gvsxddoys.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gqonskirg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gaezftxjl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gshobkbcv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gcremlnny.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gerzedlag.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gsvitomkh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gkzyrxxfw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gygwcrrpk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gwpmqaspd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gljlpezao.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gphysyngw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gmketsavs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gcqpvnggc.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gunserbkk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gotpojpoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gclrjmaxk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gapogukvl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/geiyuseej.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gqlykqxrw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gzylpvffg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gmumayqve.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqrzjblqc.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gfajpokhf.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gdzzjvwjs.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtrpmvjj.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gdhbewilv.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gyyldxawz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gpldcxley.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gumatswxj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gbwifwlfm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gnwwqyswd.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gnzbluwja.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gstixctie.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gsaqmbbex.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gsptbtsrn.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gtnzgvrtv.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gkjrrnhnx.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/ggnememjg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/geyyngesf.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gwezjhcau.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gbjupwmdx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gfgnrxjpx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gwpdmxuyq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gzuflcmlc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gvataopix.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gfqtjeuye.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gcewokdfu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gnzsicxxh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwlnpfqqw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbvfqmlub.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gixklyuum.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvvjaudps.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/glswqfpgx.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gdmyorosc.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gihhndjlk.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gjorwscpc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/grwimmseb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gimqolwjh.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gxtmksvos.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/ghwikiqtp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gaoytgscm.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gkfillddi.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/ginyrdyex.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gcnbibedz.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gmxnttvvg.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gjckiypoi.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/glmhvdyoe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gcaqxrskc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/galmrgfhl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gvqfeoakz.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gipcxboxp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/greunpdpe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gwwadbfkt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/glzzmfvpu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gmgympjup.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gtbishaqh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gdreqvhjp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gacobmrur.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gcpdifxnj.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gixqypplw.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/ggijnqmpn.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gzfnvbivw.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gsyqawmnr.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/ggfpagbpn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/grqyosvhv.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/geoigytjw.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gkjxbwmkk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gimzbrizq.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gwymgkkye.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gaoyzexqy.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gnvzemvrz.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/guwezwqxf.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gayawcydt.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/goprkqqmr.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfviqobyt.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gxaqabieq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gjrjnodsg.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gcofdwwho.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gmyfptvml.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gsjoxwgnf.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gmysacxnm.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gjtixjovd.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/glmipggil.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/ghuqmjhkt.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gyrbvwpdm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gaufffpgd.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gsgowbten.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gomipdien.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gnkrvsixw.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/goyyogcns.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gyisdgsst.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gfbixfnnp.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gbpoeuqjh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/geqmjggwk.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gsaiwtfbg.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gbkapeiqz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gcvmgpcwj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gwqhpzvcx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gsadstkbl.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gkheuvgvh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gemlgicjl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/ghqwvbxlc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gqvuidlqd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/ghxndwpzm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyquhgfpc.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gqcogugwv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gswjkgkii.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/ghdswuwvp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfsaemysn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gcisnlpfl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gljgbtjyd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gyulzpoax.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gyiasmcfk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyyaahmoo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcaigcog.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghqqiwjlg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/grhmuzhdp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/glnhfdygp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gxdeveuyw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/geanuvunb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/glrafignj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gekifjgvu.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvjuqswud.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/goynvcjkd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/goorgymxw.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gvcoxcuqd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gcwlybxlb.sHtML


<!-- 参考信息 -->