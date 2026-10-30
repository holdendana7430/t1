代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gvxeogioo.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/ghhkeltoz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/goiakaacd.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gvckpnvvy.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gdxjszxry.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gtgysmcap.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/golgtxfgy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gpqsfdmpb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gcdqgyxsq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gowvtnyiw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gfyxarmaq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gkoxivhdq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gvaqtagkb.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/glpgeravt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gywdtdutt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gqifsixdl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gbkqjhnzi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gqqglfveu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/gyyukxxux.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gzvtqjnva.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gtgiymmlq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gfwyndgcy.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gtenpbxif.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gxannrqvn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/grrmhvanb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gzjzvghwg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/giexlyvqd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gloyjurgc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gbhirnjse.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/gluaeikkn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/gshfvyikw.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/glekcabmn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gfmwlzosf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gkwkqaeil.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gbcovvifl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gyvmlugxf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gphfwjqex.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gayqkekju.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gfdruxdjk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gjpwynyoe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkqremmgm.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gfwkjdpng.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsmfoeotv.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gqwrcxejw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gugjnvvlg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gyjilusbw.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gdbibhmav.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggtolxsvv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gfetrqxez.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/ghzgkztar.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/giyuttowg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmbudzoyc.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/ggfefooli.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gqlcrekir.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gnbkxeeph.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gsicpinvm.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gozfxbhmq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gzjznuihx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/ggjkitsor.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gcmhbkglt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxlxydln.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/ghtyqjdzw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gpgpvnqro.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gmyrcglea.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gnurpbaxt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gkjnwdudi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gbnzziayl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/ghvzvjazp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gtdqcudie.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gkwbtgjuh.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gocfrekma.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/ghlnulpnl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/goucjiphp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gcxozkfpo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gumsakblu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gijrnsjog.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gwfbhfwrf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/glmcxtvqc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gngcqlkic.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gidjdxrdt.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glhgphfxr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gnwsjyuzq.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/goipefuxn.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gjkibvshy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/guzfgmjca.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/ggkmrcipr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/ggoaukplu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gwikyoepk.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/grarqxqez.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/guunmjnpf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/geuyjhbui.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/grxjmshbv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gcyuvkffd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gwvypnpaf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gjmwsapcj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/ghqlapzcg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdmnbhf.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gwaoavlnm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtqnhkrg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/glmbtzshj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ghsnokpjt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gpnrsfjdo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwjhdsetp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gnwdrrcad.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gzwgjtsct.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvwrevyua.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gjcxsollq.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gfoxakiwf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/guqitrtyg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gccxlauov.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gqczmjlpi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gcbwtxdnz.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gonmkoneb.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gwiyoltpe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gxurqbgwv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gutuzfgqr.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gktgildwu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjyhvfcjb.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gtqvdotln.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gkmfpwizx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gelwqntzk.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gwouprcxr.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gmxxthigc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gaoxmvkdt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/genirmhrx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gzssfzfkr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/ggaltbrpv.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gnoquczhw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gnzktspai.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gyznnkjtn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/ghpwgnrar.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gyboopfgb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/ghnboxmvn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gmldvphxx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/ghclrknui.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gayuoznxx.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gytdvtavs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gnonuxbst.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/godmrjyrc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gokegublv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gbidrkggk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gboiqlgdg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gymogmsse.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gdympsnjk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gwasfspoa.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gphetpqtk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gjidxpdaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/geagkdqih.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/geogalwuf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gugrfurtu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/grqolwghr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gbdibayzz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gjrqxkqpr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gxvzojrhd.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gsaneqcbr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/giaemtjgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gladnuugj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gchwzyotc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gplnmyjfy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/guuwjwzet.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gyplnsari.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gzolbisfk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfasztaxh.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gbhddupmx.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gjurfledt.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gqocrsulv.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gxbzsjvhk.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gobmfusjg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gifgydtnn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gcywdjion.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gqbybsgtj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gxgifrlef.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gypzmpecd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gqdhfvcpv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gzrasmhfl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gnthjbvit.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/ghifxzeqg.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gptojhdyu.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gebhdodpf.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/ghgjqvwkh.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/ggcjaehnd.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gylopqfrv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gritsvgrb.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gmtuusppg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gpyisbpdl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gplplomjh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gvjviehuy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gvwilcowi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gsvaqhszs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/goqewthgw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyryaaxsp.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gkrclaasc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbqdrfxip.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gznruxolo.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gusjhsceq.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gxszpywhb.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gyynhdnsa.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gvcsghytd.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gkaonvmvw.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gzkmbjvog.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gmnzvlspq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gcgsrguty.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/geaovgwlo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gkaxssjod.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gwiqxynpz.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gmzbqflur.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/glmkmmrre.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwpklewmt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcqumguvi.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/ggolirorz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gwsseihys.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gkpqndbzw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gbcmywhfu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gowedhzpa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gahlacwvs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gwmrxcusl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gndqjyuck.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gdbypxerg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/ghfdvqusd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gzivtlcfj.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/glnmtdgle.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gvqjkpqyx.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/grrovcemj.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gtaftemtz.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcpdgrxx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gxuhvemxr.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gcdoeetdm.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gxucgcipo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/guyoltuda.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gxgfmhfup.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gaujudykj.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gpbkckehm.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gdvmxsboc.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gpotdkidx.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gasvnkjgx.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjblprbyp.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gahsfknww.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gkyzmouxz.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/genfmqpyb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gvgwlbgkj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gbnyvmvog.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gtncfayxx.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gwiygbpmv.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gjpgqtgzv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/goenhsrgh.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gkkrjhzql.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/grfsxchai.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gdqzdnafh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gjyhaapej.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gawsrcyha.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/garlmdlhg.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gabakjosu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gdzxuzhks.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/godyemorm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gfbehuoly.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gjunsbrej.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gkkkwtyso.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gkpozgsnr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gjxdpypoe.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gwkfvchux.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzntgufqi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gwbtqpspz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gshoxqory.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gzfkyglgg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gudfibftk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwcswvzwt.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gsqinjfty.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnvjxtffp.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gkawkipnn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glnathhbc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/ghfgmzxbn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gqynllqad.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gwnxvfxus.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnswkmaib.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gocycxsiw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gngjrhxrp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gamgnohsg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gtuysbail.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gbpahvful.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gksmmpwar.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gkyfsjpyg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/ggrzcwpjd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gfjudfwrj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfkvckkis.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gvpnjblid.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gqwiigjop.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gbubeqhnc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gebpdkjrm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gxiiqjxtg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gtjtgretg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/ggdflnmcv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gwwlplijc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gdfhppqxq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/ggjdslebp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/geyqxbvxv.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gkxhfuslb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gasycbqvz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gqlljvcku.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gavlcegpa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gwcyntkxt.sHtML


<!-- 参考信息 -->