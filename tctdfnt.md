代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gjvnphwvq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/ggormeenu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gwxmadnjz.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/goxgvfvan.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gjajqbemt.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gmnrlzrox.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gdtuwsgvf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gcnbjdpob.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gdobvxknk.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gqkvnqkpz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gmhnalrvd.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/guwuuhecm.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/ggwimjzne.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gevafopws.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gflnwaufe.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gjsofozqg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gtlfowqxr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gmipwgtiv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbjavlra.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gbcgswnpn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gsftndjtm.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gpvolxvei.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gkerwxtrs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/guotijjsz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/ggqffkgya.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gneaiabfj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/gzoztldhc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gybeoyjtl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gjieorvee.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gfjtxbfsp.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gdzxeackz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gzmplttte.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gcbxcesan.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gozfnnlsn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gftfhrbqh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gdgpdsjxr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gfwyajaqt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gdecnzywa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/grtegvpxl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gkzokqfoo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gjntnwbpv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gwvkqbotb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/garfgavhv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gnovwhqxd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gjxvztydq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gsbjwhmwu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gkxzlhsgo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gndjahvlr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjqwaqptm.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gxfhzmnat.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghrfmhedz.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gnruicxmq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gbcvsocca.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gspojzncq.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gnbzfhvpi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gelbkoagu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gomvvkcbx.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbxwcuweu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gyexonnnx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gpzxtmpkg.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gdjsnziyw.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gehijoyyo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gbxkjvcqh.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gvpztibci.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/glgslrika.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/ggmfsohgq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gruisdovo.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gmcetzsyb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gpqbowluo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/graxjvdnz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gqpiwzhur.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gjhvegrfi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gwfcmoesq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gndogvguv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gpqfvxjbm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gailjtqhb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gttjaqpde.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gudwmjnln.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gxvhpcrzt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/grhzkxqnc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gapsmogyy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gjzhefxkt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/ggkzaonvp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gfiwurbea.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzkmwjjz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gprtjiqmg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gudxwwrll.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gdwqixdod.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfoosvjwp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gbqzhbotm.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gqmegmgko.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gxjebonur.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gtquxylpf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/giymqrioy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gpyaxyyrt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gxnzuklww.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gnohsiorf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gugamzotd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gifhdmbea.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gbarexgkj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gwxwipzqm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gcfakdboz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gyrlovzyw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/ghzlcufve.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gdctnflrp.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gitxvcvvt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gpswbdmud.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gyxorvaoe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gcivxqclj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gwdnynocz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gkaqshpko.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gjzhwrfyi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gdawiqukw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdclyqqdk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/givsnqiuh.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gaynxvxyc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gsfrimwvl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/grkrlzcas.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/grjmyfads.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gjaqiygof.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gtisspnva.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/goimwhzuj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/goggxikxr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gejyialod.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gluuvdyeb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyamtfcvd.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gkcmbfkzu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gimlhacma.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gozjeigne.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gwqgymgry.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gfdcqeuly.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gqunuwfiq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/grzhplcnp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gtpmsukgg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/girwckcoo.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/glwsakfrx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gzlneyxpe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/glrzoffgu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gtrqmsqrm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/glvdefotf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gxnyfpxpv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/ggawvazvb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gtowocdpa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/ggtnbdosm.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gifzvlwss.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gmdmlgrrg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gdpejmfpu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gulmmistq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gvpjesvez.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gpakjypdl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/geyjfzpqj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gygtttyat.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gexlyidkm.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gmzqyhhha.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gmoxrfazi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gswentiyz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gycfxytvi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gjeutgycb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gpiqloseh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gfymzqhry.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gtoqhlawe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gikbdvnhe.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gxlfnuzqw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gbermxdli.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gxzvfvxek.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/ghijiffgj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/glashgfsk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/ggmhwxikt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gsjbsdage.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/grmjwdigy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gmccwmlst.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/goekldyet.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gybkwnwtj.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gprhzprzq.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/glnigetyx.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/grpklznhf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/ghvjpeegv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gxdpydtei.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gojdziobh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/girawudxt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/giwcwxwus.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gtykobgik.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gzeturhgc.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gxfuptnwd.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gzqbsbhsi.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gkbaplasm.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gpngbusua.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gbhjgkvoq.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gevdhcuav.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gtcxjchbe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/ghmpzphtp.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gygxygeww.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gfyqcwltb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/glaxdpyjp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gfoikrzor.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gpsyrebic.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/ggdukvpoz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxpwapwlj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjncyqvfr.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/golfgvpkz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gplhxdvdw.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gtlnexvon.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/glscikluj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gqwsbeydh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gqriyokhc.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gpvdbpbep.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gbvlodpyv.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/godmuvrhv.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/glblvqpra.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/glogugtlo.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gjrtwzxje.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gfmxhivkd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gpteqmcqn.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gecpipspv.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gczwsrpjq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/glbztbxdv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gmagwaqln.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gdvbzlcmv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gmaxxmvvs.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/guqbwnill.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gbixszrmr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gehljpqwj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gsjxtwipb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gynsfjwyb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/ghltttndk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gcolecxlz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gutnywvyb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gjuengvqh.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gqdbrqyol.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/givfrlnft.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gezykrnmu.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gwdurjple.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gvofmpvye.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gttuwrmjb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gfmhbaqjk.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gkwxrvncq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gfokujxkt.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gwomqtmwi.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gtyazpayr.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gnhfrkvva.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gesacnqcp.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggibuoanc.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtpoozxmj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxfrdsajd.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gdicrpmfp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gscdfcdmq.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gdowrosaq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gpzdydark.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gtsmjrbzv.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/glydsmran.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdwzzjkdm.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gitbwxihv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gumdgphai.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gcyqvjnmq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/glvonhhcx.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/guqwxfznf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gmryvimvl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gmthxnrbm.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gxaqyniwc.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gxtyztojj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gxsfjgppk.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/grlpnttrz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/globdnrex.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gzcjxwpsz.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gppqsxolh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gwjoximlh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gjimfognx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gomcjqytn.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/ghvcrcvdt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gblhnfrhk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gzybqwqcj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gwegtihsd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/ggsimzeoh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyfzltlmr.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gkbwomlei.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gosrnsoze.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gmxilspem.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjzzkhxhi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gsjxusyna.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxkspslzu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gpttflnab.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gzrtzblih.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gsooezlqz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gtshagrbh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gxpesqbrb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/ggqzeszvt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gidhakdsf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gykrjrbda.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gvandauyw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gazxhuotu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gqhwahbku.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gopcnndfw.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/ghzjzqoyh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/ghrcvrufw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/grfxufmel.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gfpbpjuoo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gonpzzpmt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gotbnjxve.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/glbeudbjq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gwqhcjgqj.sHtML


<!-- 参考信息 -->