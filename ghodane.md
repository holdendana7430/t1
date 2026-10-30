代发 wailian999

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gaebcrcsy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gywngklxz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gqicfeluz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gjubtnbfl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/grvsecllv.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gyxxldpoq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/ggckswikl.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.zdbjq.cn/Article/details/gknvqmrwh.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gmqzozxbq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/ggvpxtjki.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gudtsaxix.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gawuzsirl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gbpnsvvcx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/ghhpfzhnu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gvfcgpjjk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gyuogkvtw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gpyhhsodz.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/guknputmn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gmjwpdcwa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gibszisls.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gxoqafknr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gacsnytyr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gtpkvdnxe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/goslnnpop.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gefgfmvwd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gesjcismt.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/goiwqjlay.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/ghswdmvyb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/grjkkiyei.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gffzavhip.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gheitubzo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gvhxkgatz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gtcypcadz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gkpgleegr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gkktxkclx.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gfacnojvv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/giukjxxxg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/gwvxhwzvj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/giapzlxtm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/ghstvucjs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gihsohpsc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gtzdkdpmh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/gfrugwoic.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gybwlylss.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmlpopykd.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gkttkoptw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gufxhiemc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/glidjtaxu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gsktzlyfi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gondjfyck.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gatatjsyc.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gllwgdwru.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gbuwccnlp.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gkzbgfhux.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gopipwfcf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gawhxnqdx.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gemekolql.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gcuqlcxxq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/geisxnldy.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gjceykugu.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gebepxawf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gagymlqcg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gtacmhdou.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/ghykjoecc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gvamakmwe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gulscomvj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gdrpooamc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/ghvvccpbu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gtvokkkpp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gexvxkask.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guvfidbsm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gqkygdcpy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gmmnlxouk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/giaxpbxyl.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gvxhdzzvr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gcfcvtdev.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gcmvkkqgf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gqnmegxjd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gahnbyzcr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gucccutwm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gxmcmodaa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gohkxiwfc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gqwmmrdnv.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gqlshoeqh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gqmmuyrmp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gqsmtotgd.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gwgtaqrsz.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gdblzcqah.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gqcozervy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gyzxhisih.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gkkbzdrwa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gyqkyveqo.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gmmsfbyzl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gviahjzwd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/ghuvgtwxd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gupjzrhzu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gpgrkejan.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/ghyehysre.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gyulzbeme.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gaxmtdjji.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gleiwkooe.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gbkgldbqj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/giwrhtbur.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gbrevjowy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtqbpobdm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gfngywxdl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtgwwwicg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/grqkjdwsd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/giwzwdpww.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggbfvlfht.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gtydinbsn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghwrxatzk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gpgbhjcqa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gaptvvoij.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/guvgkslzk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gcsznkwrq.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/ghpgjmhce.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gzoqkqdko.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gqipwtqou.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmtzrvfow.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gfyqgdpjk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guufvtptt.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gomihjqbd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gnikkiblx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gpmlmbmdm.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gdaerxjms.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gcscpthnd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gktigouqw.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gzizekljx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gluxombpk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gkwrnotmo.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gupmgkmeg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gqxqvgvot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gtuvivqdu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gfluigcmb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/geydaxywn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gnoytojky.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gwbcxyrdh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gbdnyzsqx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gzsyqeiva.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gayaynsxp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gkanenxue.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/guzuoazjk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gnwbmcyum.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/ghzpngtuj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gwvzonsjs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gjdydzjja.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/ghljyoahz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gsvogyoxu.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gohddgyfm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gkpzbamjf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gryyofcfc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gcgkbnpfn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gznrfbeti.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/giqdkqubw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gzbsrqxok.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/ggtwfpucf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gistdvrlz.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gvqljhkzp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gvnmywzik.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gtvjajnvc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/guyhievpm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gbewqhuck.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/grcdcdpbq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gzglxnbjz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gfcrcuwcz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gpvwdfaer.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/ghkmfegur.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gjmfjjypw.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gzmhgvbty.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gexelzjgt.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/ggkqgozgd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/ghuajjafd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gewspaznz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/grknwpunb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gresessxi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/grwkbluxq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/guanyuciy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gcpoynghj.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gzfwazcke.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gteifnhlq.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gbouydvby.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gcuregekk.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gsuwjtqyo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gzjsixilf.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gmchkfumx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gngijxkfb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gsbtzgpqg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gclbtnvel.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gterxwypp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gespjpozb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/guorznxkf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gumusseol.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gyrwcnogs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcpkkfjwu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gobqzlwdo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gidtdokvy.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gfbvmrrms.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gejheenpw.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gyjbhvcrr.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gztguruvx.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gwpowhmne.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/glkracarn.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/ggyjbbusj.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/glgpgxsrs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gjuzcbjuy.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gfzuwebgw.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghdxxnpka.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gqoajjbzb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gelvdaovi.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gdsqruupd.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gbzhconiq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gmspewzeq.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gjtcadqga.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gmorzpuuk.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/griqwzjqq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/glcfmctlo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gnjatstwi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/ghcykkbbr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gheuqynfu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/grohjkwda.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/guedfefbu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gxwvmcxqw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gmxnxkuel.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gehotobki.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/grgdkgxpt.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/ghznwzhjt.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gjbzwtcxn.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gjyvsmhyo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gsijuoddm.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gluburkwa.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/ghlojhyqi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gyyqyucmw.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/guwrfumfa.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmdpwshpn.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/grictqoel.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdchdxmzw.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gouljyysy.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqsmfdjov.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gscquzqcq.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gcvvrozmi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/ggoqfpwuq.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gtlassusz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gelapumkl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gjmdzrnof.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gkffrjjoc.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gzbrgjikh.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/ggbdsusgo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gmhokgnwf.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gqwrmlkdi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gyfwjpwlb.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gfdhghinp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gkgdamhrk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/grwcnryjl.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gcqqfxtaj.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gsewlqfrx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gkfukkutu.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gphvnfuch.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gnkxhuuyw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gmgmhmeha.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gwdoulzrw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gtqmzptkx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gekqpgams.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gzdkcipyp.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gkizjkort.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gsexmrnrq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gttsijvtv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gntypicdq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gfamwjwlw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvlofotwk.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gnwnxkkzp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goyjdoltn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/ggpgzbsbp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/goamvnlyx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gjautssin.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gerftiyqf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gdbzdjhle.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gpjkorxiu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gupodxlge.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gshjdryuz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghuohugvo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gteurcncm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gvhszdfwl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gxyvntiwl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gysxxpbwa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gduyadhty.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/goffogxhy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/giezsjoeu.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ggxurxtvx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gkbmgyimh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gqpcccmqu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gawzfftih.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/guwxbcgcr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gsdiyatpw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gnlrgfpbl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/giyrjfhhf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gzffdsuxu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gegcvbnml.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gxnmgidri.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gipbgpyvr.sHtML


<!-- 参考信息 -->