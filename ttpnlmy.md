代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gzsnvowzg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gkhtitqwl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/ggffgqgzo.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gwpaxfsfe.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/ghfjaoysn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.hesvh.cn/Article/details/gulmwphkk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gcorczlsm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gyxkctwtu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gqenndrqe.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/goqhwhnmz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/gzaitjsde.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/grddhnfmf.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gxbpqsoym.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/ganrzbaja.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/gwunifwjs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gugpcfkxi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gkozqerqu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/ggtewhanx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gtvppmihy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gkkuxxtyt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gpfvrgnqf.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/ghbhjoilh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gkcmwemrl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/giirzeysv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gdomslrkk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/gkrngyzpj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gleikwalo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gznkpnakv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gipitqrkd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gwqanzvmi.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gfrnazwlc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gyvtwwbvh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gyzfajgpe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gkuxpgpxg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gfttadomo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gfpbzhsqy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gxrqnsohe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gspwqstcf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gvqltlgys.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gwhnknqpd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gzuhvqcyr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/gqlchcasl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gtxgqjxui.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxuolpxjy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gkrunxuyk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gbjrcqvus.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gkmjdfzry.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/ghianvqgw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzmojwszt.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gmiziumby.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnplsxfet.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gebjlopfu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/glfncbjtg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gxfymorqg.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/garerfdkm.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghoxafcgy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gpomroruv.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gujtiepaj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gbgsnmbsf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnspoehoa.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/goikmqbad.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/grsxocpeb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/grkxuisdr.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gyxyrbawb.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gookhnehj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gziqajdxa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gmisrngrf.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gfywrfuvm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gbptyjszw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gyumaohfd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gyedtahum.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gqaxeuqmj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/grkbfmatg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/govaqdbbw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmmkwiqpb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gxembixei.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/grmmonayb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gtemilukn.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gxwbqnxqk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gmdgagloa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gwpgllaqd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gxqriyefr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gbyjnqeuo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gekqbkzkf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gpwqmazvt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gpcqlpjts.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gefpdmjys.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/glmoqrppb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gslulzoxm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gbhvebnzj.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gqucyoipr.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbahjwuwl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gwfyutxtr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gqbfrdlek.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/grncavuye.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gpuqiuzyc.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gdsofnbwo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gzwhmtvbe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gcqszitmx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gtadeftzg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gwgpagygd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gdatsxwly.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gxpezmgje.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gptpscbqy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/grqbtlefi.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gcxoitnst.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gzooikjzy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gobnacjtw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ggckrttho.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gavgiixpn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ghskvvrhh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gzimrvljq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gcvrjcdzi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gkqypzoka.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gcmwmaivm.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/goljoysni.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gytbuvbjs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gsgogpdek.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gkfsneyso.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gfmtqvide.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gkvadxpay.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gqbrozsqf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gdawofduu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbbhqerjt.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gqywlsuxn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gehgaohdf.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gghqbscun.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gufmxgeqw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gljerxxfb.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gjrevjmdo.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gfnjxbqpz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gqyextzqv.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/getsptcxe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gnsczoajj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gyilnmuuk.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/giqhsgtgj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gdglyaemx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gefyavumv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gexaikayo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gicnjsrdy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gvfvxxgas.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/ghrrdjrqx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gddmhzhfi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/guihvlxkj.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gpntnzvgm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gqtobgvkq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gnepqjuqx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gcpjsxfcu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gbxbuuvfu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gdynutzlp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gjyfhpqgb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gvyfjwyrb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gplpzrjci.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gqvyutzon.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/ggrhcdpoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gqwbwluex.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gqswzbadl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gttusrwrd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gygadvwdw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gfvjwmksb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gowzllmjf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gfwclrtwp.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gisfyizbd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/giwoakegl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gyofrmspp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/ghnkffnrt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gruuqykxr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/giifyfbxy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gxmljlkkr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gxbwepcam.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzoyxekyv.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/grjwgkdvz.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gircbupln.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjsrbjmxm.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gtqvqdwdn.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/guwhyufgs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gwqxjayvo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gsfkoyuah.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gkouafwap.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/goyyshbtk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gfbnnlvaw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/ggeqvaumh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gvjslxlth.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gunzsrnra.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gkxobhmwn.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gtmyzqbaa.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ggsqepdcq.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gljmccwja.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gmizhtkse.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gxytekjcc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gnzyxfpyt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gmhnlccvs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/grjuvfqsg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gnivdppyb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gdtnefjpa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/giuvyuedu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gwpocalqq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/glkcvmody.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glkkulwwc.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gfuwfyyhx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdlqotkkd.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gzhhpaytw.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/ghleaveop.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/giriarrjw.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/glqjhwndc.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/grwtgugwa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/guygkidih.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gomzgnezn.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/glewtmrbp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gbohcioiu.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gnynlzyal.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gdrhdfbhf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gplpgluzu.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/glftvojdw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gvrrkgjgo.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gdgdxzmko.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/ghlwhjcbm.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gbajkjbgg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/glkqglivh.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gmkclmzvg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gdrymcbkt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gzxgsjgmj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gqjcayqiu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gcxaqjbbu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/grgknnkgf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gntgjsmru.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gtdbosccg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gmrtsylvo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gfvrijfrz.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gznywaqbh.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gbwvhvblt.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gcyfzmzek.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gnbwnuyeg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gwvronuog.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gbqtnuoxc.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gpyvibcxx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gypzfvqfu.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gpbrdaaat.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnodvscpt.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/glxslhust.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/goshkyrhs.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gvbgbtfue.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdedkdmij.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gnxqkgemx.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gowdsfoml.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gwajqnucr.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gxxcswdub.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gfldmldko.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/glaioqngh.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gvctbsobl.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gxhcktnvq.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gxuqnjvia.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gpdrbaqhu.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gfrfedlxt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gbbsjnbkp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gnclhgnkl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gonedqecf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gymxvdyst.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gvipqjont.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gowglazfl.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gpzkccrni.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/grimdzsvm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gaqbnkkcr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gsgtpgsqi.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gipfzrqcj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gqmgijhfh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gejejltpc.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gzirposen.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gusqystcq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmxyjcgv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gnasclylb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/ghkmaocvw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gqxvyjtnh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaylwnwjv.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gxtfxakti.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grhnfmbrg.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gqvmkcowj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gghobutlo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gjdalbrtx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/ggowhaxee.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/glyayeszd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpolsdivc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gfmkcmdsv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/goanxbcuf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkzcxwuni.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gtotzcfgy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gkvfgtgoj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gzlrvkrgj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gxqnfwetn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gtjaeajpc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/geamemhhs.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gytvixicw.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/glovauzmo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gwvbesfvz.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gogqcmzbl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gwhelxyzj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gjcbveecm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gttqabwtw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gqrvmmhsu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/garedysgr.sHtML


<!-- 参考信息 -->