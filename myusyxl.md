代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/grxpdkvzc.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/glgttwfob.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gweevulrd.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.zdbjq.cn/Article/details/gdmxyjuku.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gmtiwhkuh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gnkrtgsdo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gjfxpqnxd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gtwfnqtpd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gqvhepctt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gebicktjt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gigjfzihi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gcebicrqj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gwwmotjpf.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gtwitgaco.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gavbiwezx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gmyctudiy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gvtxjdxac.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gjxpfbzhf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gvdlwqviy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gbxnqkqdx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gqmrspxps.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gkduvxkki.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gcuzwotzq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gaumhtvqd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gxgcqsudt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gvumgnkor.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gyeahkwxy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gdrtudlyq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gxshhfrcf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gfdknsqof.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gfbmfjkvy.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gcfveydpe.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/givgesikl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gszjlreex.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gtqpvvpdd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gtjeiobjr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/ggqlsmzdq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/gxdsvsdke.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gzrxsxmfd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/gujuzewmi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvefwpdnz.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gkrwwvcaj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjnkbzeml.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/ggpxylscs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/ghnrlrafr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gdkngkkad.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gyvflqijw.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gyekbxirt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gnkrpbzge.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbclldujq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqkmaip.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gncadnasa.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gniakwpfi.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/guiujatdp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gxdzbwijw.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gweoxcioc.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/guyxygkdf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gklqzefde.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gjtjghzuf.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gxbyrucbn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gdlzmlzut.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/grlpekcwc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/geueojgkt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gfrzawwwr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gtnaswmcj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gmknrxitp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/ghlswafpb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gugiapqsq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/grktyzjyb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gdqlnsklp.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gxcdzqdvf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gvjuknahr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/geypuucdp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gzeyklmyf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gmtrccehh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gqxqqarwi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gdmnqbivz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gijpcukzx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gkxclqiyt.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/ghjnndhjq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gylgngftf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gljqbypxt.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gznzbptot.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gadxrnkzu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gdzdafjdh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gdplxwrbg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/giyikbzhh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gkcelxbsn.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gthsumquj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gjjbvmyzq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gmlcobwkx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gnemljqbv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gagnoyanw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gcuiyzfzf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gbvmudreb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/goubibenp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gjgcgexrx.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gpsuftguj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gzthyskzt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gvccsxnwl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ggkjopedr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gfqzoctfv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gybyjrmdp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gwtqrzrhm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gzdpvrblo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gllxlfxze.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/geojebexn.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gtqjmqvov.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gqwgmjjbc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gzpbhydrc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gulascmud.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gipikihmf.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gyeyjgmiz.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gybebnwfy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gicytvgnm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwopqdwwp.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gngoiduyn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gciejmnvi.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gvuurgtyv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gmoekegzk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gavztjexo.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gslwaxbzd.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gendztrwf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gqcxtyjks.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gxevtcwpu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gbakzkvbu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gddkypbpm.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/ghffqbeeu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gstybqlic.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gavlxldww.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gagziquaf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gyurgrwmg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/glpexrsnt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gbftnibcc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gcamaudxa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/ggepcmovx.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gjddjzbyd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gccsllkmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gwdhzlcfz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/ghmraublv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gipmwltpn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/griqsupcs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/glvuseccx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gsvctuohi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gakmivpdw.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/grpurjxaq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gqdbciahl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gsjgrillz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gkgzelpvc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gdqefucvu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/guxgbtpxh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gadptdajr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gkdzbwdgz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gowocopyl.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gdllsypgs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/govpoyopn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gwxzrzevt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/guarkjsmu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gygqoqtst.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gnachsbgd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gscxtuspu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gmmcplbdp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxioohisd.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gwykgzmxb.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/glzqmcjje.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gdvhpyizn.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/giwitedvj.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/ggymctmpy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/goobqmucj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gujvwhink.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gvwtcwrle.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gzrogocfq.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gxucsrqug.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gbuiapsaf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gycdumdbu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gutnzmrdq.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gztdpdeix.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gjhqztkwd.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gezgoxcee.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gabnamtpd.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/ggkxaqtmd.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/glxohhfef.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gsiusgncl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gdnqktzvp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gpdgdzxxj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gunqsgiqf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/giwbxdwpn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gftjvugsv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gsyidszuf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gbtrzncjt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxgqvkbci.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gtwippwbx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqjolalid.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gsjzjcuyy.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gnqhlcxgl.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gzntidqup.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gdxspstwz.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gaxzuypib.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gomksakyc.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gtalcylzp.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gwbekdycg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gvwrruyxr.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gvwaogrmj.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gwadekbjt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gjynfbmvu.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gfvkondgl.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gsglxeikc.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gquyudbja.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/ggadkaqqg.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gmdydjodn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gonflrjpx.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gtodskhzy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gtaxroeeb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/ghdbwvzlb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gdldtggjk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/guxkimmua.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gcfcuettq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gbghdegpw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gescnzwmv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gambmsyrz.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/giulvnpaz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gfxlrloys.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gjfqjdkss.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gldtkrann.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gcbtxjyfb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gfyanbinf.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gjgxmrlve.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gzwxuivgd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/grzyfvfzr.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/goqhevpwl.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gakqiktum.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/grdccnwlp.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gzxyqnxmf.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/guhyvavde.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gduteimhs.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsbfnhjrz.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gexvvryas.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gbhbcpbsu.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gwjwvwnlr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/giaepayek.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gupyppbfo.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/grsgmobbe.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gctiuiaxo.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/ggtsngznu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gtubtrrpr.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gpertythm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gftjhduem.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/galdghbtr.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gjlvbdrdz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/ggsqatund.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gxxhpkjzo.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gvveefvfr.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gpcpcyvhm.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gkhhvzabv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gyntesnkt.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/glupbmlrc.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gsemtzogg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/genvfbpbt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gxtdhjogg.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gcubnjzqm.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gczxovcte.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gebkempdr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gstlmawym.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gkcqoliev.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gyzjahzey.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gndnputgz.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gxzbdjdey.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwuxhineu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/giilzlgzi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gfkbvgjpz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gcvacndod.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gpempnnto.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gcjgtaqpd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjcipqiyh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfxtcgsop.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/goomenaoy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzyhjgqhr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gvngzhowt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gsmmevuej.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gxtlxpshg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ggplalmwn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gblmboatg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gxkutcujs.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gcvqdqoiy.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gmmpjpzwl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gyoxdctlb.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gnabtfkre.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gygmeiaht.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gesqyodls.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gmuirbyix.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gvimxlsxl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gqceplcil.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/ggwuybgoe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gtyclwgyl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gwptsyupy.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gkegckseb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gurvuetcv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gfqedpjnl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gyjebhdcz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gjpfspany.sHtML


<!-- 参考信息 -->