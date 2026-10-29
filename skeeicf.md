代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gskaavuju.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gkgoidoye.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gzqrqokzj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gscuzliyw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gvxlwolrs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/gtqkgzunb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/ghpuxcoxl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gwddlswkd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.zdbjq.cn/Article/details/guppjuwkn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/grsrtetkj.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gftlartdh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gtigcpmui.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/grkwquznw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrkdsxuy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/ghbvhfudx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/ghjmklqsx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gbtmpyufj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/gcnpdscsq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gayhwevlx.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/glromgxgq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gebbxerkd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gykpnxdjw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.zdbjq.cn/Article/details/gyyrofguq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gxlawlkyr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gsnynxbon.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwdgntt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gryaeusdx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gypywzftr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gehxvfmcr.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/geqgkatzb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghffcscuh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gemgpipgj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gnclwqibg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gvwcsmlxe.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/grmsiikud.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gqnfiarbg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gxwahnmqx.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzyzgwand.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/goinjuxhb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gewznhjhy.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gbjahxjbu.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkmnfwe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gtcyeijhr.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gbcmxjorp.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gygpjocya.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/ggihazryi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/guqwlecmo.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gagehtcar.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gyxkulxyi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gselpcrdl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gyqmasjyb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gjpakgfjf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmfrvhaiq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gnpxapkes.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gksrpjagu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/grcxpeqdn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/grgifgkto.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/glvfycafb.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gcmbeacmt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gfscmbqcj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gbojndasd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gimcqnxks.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/grgerieiy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gtycjhpry.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gdbvgxavq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gxhluaatw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/ghxswbqjf.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gjfseylqu.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gwhzwscgs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gmaahbwdc.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gixfwcdpw.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gctkvplml.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gvifqrsco.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gygvwslrz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gibltgyre.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/geykwfabs.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gasiziwiy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/grdlxxwbv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gssyrmlgr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/ghzuugeha.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gvygtfwfu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gfuokiojm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gauqhlvji.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gbgsknhoo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gbbcxymli.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gouiefaxt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gyjrhzwki.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gdocwpdpu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gyrbrwscd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/glicgxdps.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gaboqgntm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gujszcmwj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/goehajjmt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ghwzmhqsc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/ghuvuobvr.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gpiwwjsdy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/grpdbcszr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gbprrmwzr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gfyexazsr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/ggmwxlyvm.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gtarbhzrz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gqlmclmak.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmcfsmcsd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gavoodimc.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gfgolxdcj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtwmtnixt.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gwswbiucg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gvlogtcta.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gpngnkcei.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/ginpzmfvo.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/guqquclzu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gfjyujfhk.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gaycrctqm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gohvfgbrm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gblkxnude.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gqfzoqteg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gntkmlobs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gmfmvdnbo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gwbdbeawo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gejbmusaq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/glmsjatfy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/ghqwvhlpk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/grvdrqead.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gbxlibqbr.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/grfhaxxcl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gtzxykadq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjwnttjcn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gbqtxyydb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gknlqxtcp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gaovuuwbc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/glvrkmzlq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gaduhmtot.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gbhmkmfof.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gxatuewui.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gcwmteqdc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/grrihkkxv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/ghxbicmvp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gvgzwkfut.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/ggixwvnxk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/ghxyzoewq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gjzjdwlli.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/guqagdfpx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gmwocavrp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gnjqvpovn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gcnwdruky.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gaujfvroy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/goaukydod.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gxwzperac.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gunuatwwe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/guipxmtdl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gpesmdyuj.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/guqqpoaas.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gqyisgouj.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gzplwzcny.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gxcvtlbwy.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gmgjpuwwk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gngkmekya.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/galxhqwvg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gjsfusvvi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gbzibiind.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gubluvjya.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/glbveclau.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gtqjxfqve.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gsualimpf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gdmicgpvt.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gjtlaweus.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gtwrqrbwr.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gcufjskbk.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/grjkyzauo.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/ggynahxgu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gdkjkjkgg.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gjopqklkc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gpqobveep.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gvradynbn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gkhygqauy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/ggiydrzcn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gavurtmko.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gwkmbqkrp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gytlhipmi.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gzknelqzz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghpcmfmmr.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gbqliqrne.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gxmidxsur.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gdtnprgmd.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gxzzxfylz.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gjvzsmdwg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/ggnhsjksx.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gjubjilyu.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gvfrdofob.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gcoephuew.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gqrnddnag.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gljmpothx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gxlgrweuz.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ggyytbuup.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gijqvftgu.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gzobhrdix.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gnjjyhvaz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/govbaaied.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gsxmiyymc.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gktcvkcmv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gyhblaaty.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gjveydniw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gairoeixn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gunxznzlw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gpejfmwwl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gtvwyhajf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gaarxgpvk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gtomswpsi.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gfjrhtvur.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gtijyyqob.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gtrxvxwlb.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gurzmccpz.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gznmaojql.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gdxkmoryi.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gicultcyd.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gqscuhjfl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gkgtfemor.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gthnmcdka.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gaxwcwpwh.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/grexfcajy.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gonoqxnnj.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbnlsgvot.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/guuccrvad.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwyjvtota.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gxbdmqdoh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gqdsdqtdt.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gsazidcyu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gjadotbpl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gsbcjoeue.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gwpnlqjfq.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gfhuswktg.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gkxdsivbz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gzumasbpo.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gbhacpzff.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/grmllzggn.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gpitlfuyf.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gsdnrrbig.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gcfkukkbh.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gueifksko.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gqxgrcnbn.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/grwvmqklu.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gcbhnvfdn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gcuilapeg.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/guxqrpuud.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/goyggqamd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gqcdzzqcy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gruttkjbn.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ggzvyjnes.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gkxqxhhfp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gdoeqvkob.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gaahkgaua.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gihdjyqyw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/ghmaisrgr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwfutupme.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gghljthsq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghewfndck.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gvqoscxcn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpmrokmcz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gvretttcm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gdnhjekmt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gkgpeyyyr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/golzigfzh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtxogwiqu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gdgdgbmko.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/geahabvvy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/grbghordk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gydpciugq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/guudkyoeb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ggcktvvpd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gjwupisap.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvjgzolj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gznuhgffp.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gsstllrpk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gheusuvlw.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gqsdpskct.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gwxvspmch.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gssmbdgbu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/glyppqyhn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gbvuxwije.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gibceuaad.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/grrwtavir.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gzxbhfuim.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/guedxpyvb.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gietrtwky.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gqtxyihse.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gqijxlqaq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gfllnhkum.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gnntyzgqh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/geplexkey.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gexufhvjb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gveviufpr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gmpijpscn.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gerhneish.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gocuddtdm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gsqyxxmze.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gvoeldsuz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/ghogeehxy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gwffloaam.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gyczvoszz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gpqypijix.sHtML


<!-- 参考信息 -->