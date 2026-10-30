代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gqsxdhyul.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gpvmlefqq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gnduizvun.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gfhqbgzaf.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gynccnejl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gdqevhstg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/geydarzsp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gzhffhuiq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gnnfubpfh.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/glxtlnkyp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gzlnhrccy.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/grzzfkxem.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gwznjpywl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gbxwcgpbi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gxsizxvky.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gccghioen.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/glrauwzje.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/gjppageul.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/goqwlobbq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gysabnlub.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gxjerkrfr.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/garoeydno.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gmjjqrqas.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/gkaoozels.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/guetznalf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gwuubmibl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gjuetfhte.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gtmfciwii.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gpydolfdc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gzyeejqef.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gebxtyaeg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gtyjcegel.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gqaikxkhj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gpsdmshhw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gbzyrdcma.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gqwmgqusr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gkbxbxlig.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhcmqdn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gbinfhpyg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gjrmcglfv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gvonmczpi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/ghelfegjs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gymknetpq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gzvbthdkb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gmkajrkcw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gpyrvxrst.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gquoxrlrw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gobibhrej.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmmexyaxc.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gqfhxdccp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwcpfhlci.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gxkdnvefd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gnwymfwfy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gpdmnbtbt.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gobublvty.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gyasnvagp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gyflwcyyw.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gkgbnyxxx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gkakktqtg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gyibngomv.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gekqjjzrn.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gfxrdsxbx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gmohxegyw.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gczckxdjz.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gfjqxxjhz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gszmkfxkx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gfjamikrq.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gjlsuvbvm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gknbmfhte.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gtzqsaohi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gxrnpmuyd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gfrnawyds.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvmcoznma.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gimmlrgvd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/guonzzwhr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gkfnwuydd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkohryafn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gydxujujj.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gpjkbrzqc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gdogtwjex.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gldjdoqfn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gpgqjptpe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gdfjazjud.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gmpsrurlu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gfusrijii.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gjuedkdzp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gotahcfza.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gvmikuvon.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gafmidqhq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gyeyhjxwh.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gbmczdjnx.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gkwzadxsr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gnaeuctls.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gbbbyghax.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gnuyvuyio.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gakbsgyhs.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/glgzginrk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gjgovqpbl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/ghbcvomsh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gxhyxjaqw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gtmfqddhl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gqarzirlz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gnveccdox.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gxwurfndz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gzdnmuhto.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gbvxqfqmn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ggfxzfwwy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gpxsqsmuu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gblwqzacm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gzaedlnow.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gsccgupez.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gqghfsiet.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/grqvruptd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gziggtbtj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gththrdae.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gwnqyfcae.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gpglmztuo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gbpwjfeex.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/glcsazmqd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gzmlzwpbx.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gtobupajs.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gzglcgxip.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gaejvwbzc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzwqtsnsc.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gsjtjkctv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtgkwfeai.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gtyujprsq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/guiqoskxs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gmanxxltj.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/ggamsdnxe.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gmvwfvpls.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gmvszavro.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gtxrshovf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/grfpxsekf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gvlecqkzt.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gjpmcfbke.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gqtgtdsuu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gzdcgnbxa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/giivvnnbw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gdlktjfdf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gxtmpsjpl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/galkprvac.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gmimvcnnu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gnzbfbsha.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gkuajayfa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gxjrgudgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gmwnupfcr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/grimyvedr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gkgnjsnzx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gjnxjelnz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/grsfbeqza.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/ggeebgkey.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gtskfphfv.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gbjidivvr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gljtydhek.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gwicgcxfl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gvhlffwvq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gqxcvnkkq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gfcejmuac.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gznydwsdm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/ggffldgvb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gvhdhpqxj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gemcfrrvx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gksbwwvwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gapykvygo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gijszdncw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gygpmgaun.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gekegvrwy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gcoelmzmt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/ggcliyqtd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gzvaivocu.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gfygxryzr.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gfpcfumyt.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gkiddqwul.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ghtoxipjb.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gchxdalcd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gmjkpxqjs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gzfveixmq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gzoyiquww.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gturhwehu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gqxcviyzr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gcavynjqk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gyffzyaob.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gfsyugemp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gwbzagvqn.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gvwrcljvz.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/ghrczmlaq.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gvkltrtjz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gfulbivmj.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gaqihoack.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gtsavjfhl.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gqzmogirn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/giebkqvqg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqbelkcfk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gaqdqsobj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gsgnhqqpv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gfxvalkcf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gpniqkqaa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guhsbzpvp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/ggzrnvpfi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyrzgkqhu.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzjnzxycd.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gdpovofhc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gfonosybd.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gtnvpsqgm.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gihorchzc.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gjzjsdbnk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gximchkfj.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gjqmyhgiz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gcpqdquva.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gpggalmae.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gvekfmxnn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gqklazsjn.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gaiskmnnd.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gljkldoqg.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gkdighxod.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gmdtcqfrg.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gpxabwglk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gbpmqiqxy.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gemivtcbf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gfizbjajq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gzmwewgqq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gilfzynxk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gnorcaffh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gpkelkjhj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gsjqptqwk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gvszqvtly.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/ghmowwpjg.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gpmyxxyka.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gytfeoymo.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gmeoudmxp.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gsksuuwex.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gldbzmzxb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gykeprvaq.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gluysqrkn.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/ghgexyxwr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gyejemyxx.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gmnqxamwn.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gwzseguvl.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gxdrlnkhs.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gakhlnawh.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gibhicwou.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ghurzaozs.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guvbiwuxe.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/ghgzcotsf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gkqklfomn.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gwxcbzuxp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gxvqqrzht.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gcdqxhylb.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gkmrljfvo.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gflbsaldd.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gajqikacv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gcqrupwqu.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gehahvqoe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gpjrqlqng.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gajbepmec.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gxshaongy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gzwamvyjt.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gtkrteeil.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gryfnqxkg.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gcwxzjooz.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/ghuucpftd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gdmwpbgxg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gzcetnjbc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxxzuwp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gwihoxbya.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gkszttfoe.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gwjfiyrnt.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/genlueduz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/guvlsjvjq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gaeuxokkb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gjhrsiedg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gnfbfghqy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqlinljfp.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gbsvvqrep.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwttetewo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/grmfhbxdb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/grqmiqpks.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gmtlwcxcz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gimubucoe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gvpkugaae.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqfojlofr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmqfnuxzb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gxptysmcm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/goxafuqzo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gedaqdqvp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gmhacdtdp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/ggacnwlkw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gvimagroa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/grejywjfy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkhogfhe.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghewpqpsy.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/grbtzvmpf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gzvfivcdu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gneuwvlzd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gvocnltbn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gkffddhbr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gurmtchdh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gupbozunn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gqipzewqg.sHtML


<!-- 参考信息 -->