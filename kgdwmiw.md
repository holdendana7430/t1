代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gijsfptiz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzthhrudt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoddeqbp.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwiytsye.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gjrevzcql.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fanxiaobao.xyz/Article/details/grnlwxxvq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvejwdzir.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnpjpawl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gxklzvwrv.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmsafynb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fanxiaobao.xyz/Article/details/gwnckxlur.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffclgxrc.sHtML

[J07] 比较两个日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomdevavs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gjcydkgcg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fanxiaobao.xyz/Article/details/gbebarcqv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/ggabzmsnb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gmfxxtouk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gpcocmpxv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/guquxxten.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxwnonqb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gmjqioozs.sHtML

[J08] 提取年月日与星期
来源：http://wap.fanxiaobao.xyz/Article/details/gffbmdwyv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fanxiaobao.xyz/Article/details/gshfuikhm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamfhvbky.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpghkcms.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fanxiaobao.xyz/Article/details/gtfyaendh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpdyuzbn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fanxiaobao.xyz/Article/details/gxiurbywt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fanxiaobao.xyz/Article/details/gbhppksjx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkzctlxh.sHtML

[J09] 时区处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyicqpga.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjinksdkn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fanxiaobao.xyz/Article/details/ggacrvfpe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gomxodvqr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuvfteur.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnlofnbi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fanxiaobao.xyz/Article/details/gkalwnzsl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fanxiaobao.xyz/Article/details/gwuvaltrw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fanxiaobao.xyz/Article/details/gmxpuvbrp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxrqawar.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gioykdxsi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fanxiaobao.xyz/Article/details/gctrukzwg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnduosgpv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdblaygp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfdhtysc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fanxiaobao.xyz/Article/details/gmugjykra.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fanxiaobao.xyz/Article/details/gtcvocguz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwaqitbe.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgymiizf.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/gqtjikyzs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gncrajfap.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/guciifciv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gqrzxzmcq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfvwnqfn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmugwofh.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbfxtwjm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgbhkkpk.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ggcbrwkke.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fanxiaobao.xyz/Article/details/glkilxlmm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gymmtfamo.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gserxsios.sHtML

Py:   json.loads(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqovzhwz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwcwsbxx.sHtML

JS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmbcwdjya.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmduvykr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gllitsyaw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmjcxxnh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjtemxjn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpwcpzcwc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtenqryhi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqexcpte.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyjjzwnw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspkdmqlt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grobwyoss.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gukdrodyh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmkehqbw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhvvtznv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrijytbn.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmjqhwsir.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gnguixybb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmtsnfqt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuyitvlc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gayoemino.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gkezqygts.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoappuih.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/graaltjxe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gielemsfd.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaouuqrao.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gzbyzfwnr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fanxiaobao.xyz/Article/details/gobyajdxn.sHtML

JS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gxfmxvmau.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/guxgltlfk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/ghuriyfio.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/gwsuldrcf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gvwvppmys.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fanxiaobao.xyz/Article/details/gmkoxogds.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fanxiaobao.xyz/Article/details/golwxejgg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/ggekzdqdp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fanxiaobao.xyz/Article/details/guvvinlrj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqryvyep.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuxbeezx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gtckxtruo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gliwnbugq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyypsqjwz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gogymkoql.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaksidld.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grylmyjff.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjixvznn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/glgiybpty.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gjzokibjq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgqbccev.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fanxiaobao.xyz/Article/details/gyhyzxpxz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqetziyx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglbztgww.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdebbahyr.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvppcgwb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gviqekoaa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gsojzwvmk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gjvczcqkc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fanxiaobao.xyz/Article/details/gceskisyt.sHtML

Go:   encoding/gob
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjtrsttw.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gqrlfujsf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbvyqwaf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmchufxte.sHtML

L. 网络请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gynqnbxne.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqankuybq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpabrzpk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fanxiaobao.xyz/Article/details/gghkhohlo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbblkczp.sHtML

JS:   await fetch(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gytarjrcg.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/guukheqnk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqcrvkra.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkjysvla.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfancguzj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fanxiaobao.xyz/Article/details/ghxeimsuq.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gnkuhzlif.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjnttwmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxrpgdmu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/guudanncx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbgajjgf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiebkzaf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzlcfqsx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/gbwkcosrc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gjxekgutt.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/gqigcldqt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fanxiaobao.xyz/Article/details/gazzfoqwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gosfhpslt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqyrnlll.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuryvyxg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/gofhkvghr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcghdfano.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fanxiaobao.xyz/Article/details/gvpbruuta.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fanxiaobao.xyz/Article/details/gwfkjmhbo.sHtML

[L04] 设置超时
来源：http://read.share.fanxiaobao.xyz/Article/details/gogkcshoq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fanxiaobao.xyz/Article/details/gnfxeaqmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvujiojow.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/glsvxaguf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gyswszwzt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzzirryo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmwsbmnf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkvxymso.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhhrgwip.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fanxiaobao.xyz/Article/details/gdvewgugy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fanxiaobao.xyz/Article/details/gobbyigew.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpigplhp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gewyrqbdn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gsairkpic.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fanxiaobao.xyz/Article/details/gtncidssn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqetlaszz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fanxiaobao.xyz/Article/details/grrrorfsf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicmjwsuf.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnyqxqtk.sHtML

Py:   resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gwznlkrcx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdjbycfj.sHtML

JS:   await resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxfjxuev.sHtML

TS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gsbkejhrc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/glpcnpukr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fanxiaobao.xyz/Article/details/gjolwnnom.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fanxiaobao.xyz/Article/details/guvnptmqz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnmualfw.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gvawzjfvr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/giauyfhrm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnreqknm.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gwumdwnrw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaiyinrw.sHtML

Java: resp.statusCode()
来源：http://blog.fanxiaobao.xyz/Article/details/giskzzvor.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxcvpnyk.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgcrgri.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/ghibffoqg.sHtML

[L08] 并发请求多个地址
来源：http://wap.fanxiaobao.xyz/Article/details/glkcqvqxe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fanxiaobao.xyz/Article/details/gjxqteiog.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gdvxqrclc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmibnumt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gbectobim.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfjjljpv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnjvhisw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gxdwhqcsa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxvmisde.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guxcsralg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdzafxlw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfxfohyrj.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasxazfka.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgsfqptk.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhczmbbg.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqiohkum.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtypykbkl.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/geknbifiu.sHtML

Go:   os.Args[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gktfmrkto.sHtML

Ruby: ARGV
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgjfopks.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxbdyryy.sHtML

[M02] 读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggnzflqlz.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gfqzegiot.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqadchcw.sHtML

JS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/glrapspyu.sHtML

TS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgnqedxt.sHtML

Java: System.getenv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gapruyaip.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/grelxxmkh.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/gkefmqtwj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gbfhjkzkt.sHtML

[M03] 执行外部命令
来源：http://m.share.fanxiaobao.xyz/Article/details/ghymsaptc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fanxiaobao.xyz/Article/details/glgxbvcof.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fanxiaobao.xyz/Article/details/gzwaufbgs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlvoxjqf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxpdzwxw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goizckher.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fanxiaobao.xyz/Article/details/gzkapiipx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgsrethh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuduzhdk.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/gscbteumr.sHtML

Py:   os.getcwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gvcotlifl.sHtML

PHP:  getcwd();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqxbmrdh.sHtML

JS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghayysufm.sHtML

TS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvioeadsp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fanxiaobao.xyz/Article/details/guezozdnq.sHtML

Go:   os.Getwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gylunyeku.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gkgghfbtj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fanxiaobao.xyz/Article/details/gafrxmbiy.sHtML

[M05] 设置退出码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorefzsyb.sHtML

Py:   sys.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gibktowil.sHtML

PHP:  exit(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gophomhba.sHtML

JS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkydobuna.sHtML

TS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/guszwhwdt.sHtML

Java: System.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfxmxljgt.sHtML

Go:   os.Exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/geahemzwi.sHtML

Ruby: exit 1
来源：http://blog.fanxiaobao.xyz/Article/details/gdmxpnrmr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fanxiaobao.xyz/Article/details/galkqlpjy.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpeanbdk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdszjdgs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyemucyvt.sHtML

JS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoplbiet.sHtML

TS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebtscyiy.sHtML

Java: System.err.println("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gybhhhror.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkugzpgrl.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gffpuhtef.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gcmpcguup.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrfiufds.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmdvqdez.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gfydlapxb.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/goxotyisa.sHtML

TS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtagomtv.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxghoexnt.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgxavdoq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fanxiaobao.xyz/Article/details/glaeeceou.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpzlekou.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzluqvca.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fanxiaobao.xyz/Article/details/gtyfgynti.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fanxiaobao.xyz/Article/details/gqbhilmnl.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunmlzmva.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gizoiacfy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpriqwwj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fanxiaobao.xyz/Article/details/gxvcppmec.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpceqcng.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fanxiaobao.xyz/Article/details/grekjkcui.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grbetclxw.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gdkhqqalv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpiigkdf.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gxyuoujos.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gruxpwdxs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdsxvipx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwehyhkov.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvhaeztu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhnxdbif.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gaopneqan.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fanxiaobao.xyz/Article/details/gqcvjdzbt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcdjpggn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fanxiaobao.xyz/Article/details/guuctsvhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gurpzzagf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuejlwpg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gqcaoxwqc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/grzjxtqxw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gxwqefvwu.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gkvtkziwi.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrununtr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gkscoltce.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fanxiaobao.xyz/Article/details/godsaksqv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/glmkkpjyk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmjlglwz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfbhedxv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjchlmks.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqycrvvux.sHtML


<!-- 参考信息 -->