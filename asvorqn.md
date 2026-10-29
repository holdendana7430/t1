代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gduuljgsf.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gpinklfcj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/giyreptdv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.hesvh.cn/Article/details/gwzudmlau.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gmlbewbfi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/guoybdnkd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gmpbnzhxj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gznkqisfx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gqmpxtkwm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gvsinlpuv.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqlyrcqmk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/gtvftmfhe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/glfaozsuq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gsqhwppam.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/geffdyzaw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gcffzcsoq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/gvmhfoprl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gykmqijlt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gboflvuog.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gsehlrgjj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/gwknrprfz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gjamfhqyg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gtjkdbjsv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gohgzbwoe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gvwaxzzxw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gvrgjilpe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gqicbfwsd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gografvgh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxmkzyspx.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gpcxgxcpz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjfvkvhln.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gvihoxtzh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/grutntrel.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gpgwjdmel.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gprsrddiu.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gwaywvnwc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gkbzfdvuw.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gfumigshq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/geuuqqsta.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gyqzqpixs.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gugwtizwb.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gehxquqws.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/gyjoflejj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/grvoovbtv.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gfsjckwfr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gjgqxhpfr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gtbjgpuzr.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gmhrhlrsj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gmoiryskf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gqsrddiwj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gwvkxjxic.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/ggtumdxcv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gunftiujl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gtafvearh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gfhkibtls.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gswytfcgj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggfqbdkdn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gvylxhxix.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gjcmglwcp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gchrxjrhd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gaiuuzwvr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjldmnjix.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gftbqjode.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gnuqhepsh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gumbmxusl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/geauhxbqq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/glmiadgzv.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gwimnzooj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmyvvacxl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/grmkwssyt.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwgqfhjoe.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gteedzhpk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gcdhuvfzr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gexpxusno.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gauzeuzes.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/glwngwzdn.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gicnnvmvc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gecydlpas.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gghwjbswv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gtagtwbgo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gwjfducwj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gdtqmrnxy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gvyodikjr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gkhqdfvpp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gjudpwctk.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/ghnrbqihx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/girmwbouj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gmmwxqamu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gbddagrae.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gkhezhxwu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gdlswpthc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gqhklcqmy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gwvuahwnp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzbwxvflr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gpadywood.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gveligzrs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gxnjtsqid.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gxigceapi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/grawqytdd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/guqgnicxu.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gofmwyucs.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/ggblchjhg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gpeoxphvn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geqasthlj.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gxlsiseda.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfzhnalxw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/giliufeln.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gsxabcmao.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gdbvqqljf.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gaoywuexo.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gpjtqzqla.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gowgqxtrx.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/ggbchzntt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gijgmxowr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gezccbidc.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gbtjbzwwc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/grdhhfswq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gefdylenz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gzfppthfp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gnsaeyfow.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gduzrkeoj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/guyodbuhz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gbwcbblnb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/ggkzjenwr.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gvwzksnly.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/giunybdae.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gwqbqzinb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gxuuyxxfk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gtkbweopm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/grhihkaom.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gwoqvcaux.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gyrgosiue.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gllnohodx.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gmcyaetyb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gzinqzexm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/ggnlqehof.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/ggdzlbicq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gneuytkwb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gmwdtllur.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/glxsxmtqq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/glimujarx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gqgfuhark.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gpqgwbwin.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gvndalxxr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gvlhfpriq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gvncagiuo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gchgttcye.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gxgygdsew.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gelrupwux.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/grgdadoyt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwwzxjuxu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gtyvszsjt.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gyfaehoax.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gmnvjjivu.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gbmmqxqzb.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gaafvdhua.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gwpnpcpoh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gsgqhjagh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gisbvmepm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gpislmrxm.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/goxtakzif.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gtrdoxzpp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gzhishixl.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/grtdipzru.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gqiruwkje.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/giwuamosl.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gixjhxtrh.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/ghvriidbh.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gncfqoibx.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/girkbmgpn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gzdjzaddy.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/glcflxbse.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/guitcyahy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/grcgfvbsf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gwqhogzpl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gvrgzunzg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gamzaktal.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gbsmzfpxb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsbwvlmbx.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gzmeffdki.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzfcynuah.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gutsshkby.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwesbubxz.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gkefjhuxj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/ghrdvmxcq.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gqdtsypsm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gfjnflojf.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gvgfuouaf.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/grnfxffea.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gnryzmznn.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gpbroemih.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gwyffezhy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gyegxtgsa.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/guvnpbyfi.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gtrkwdbuu.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gsvooqbhz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gdzrvdamz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gyxpybvjj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/glczitvxd.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/ggdrnippg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/geonbujjm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gtqifogso.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gajzsuixp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gaytrxrzd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gaowslmcl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/ggvrkxklo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gppoycsth.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gdouyuidx.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gwuqgxymt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gztvqkrkf.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gkqppzjpo.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/googjcpku.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gfdiudqoz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gtkbtezmh.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/guxjgwkrz.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gxyjnblwb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gvdztwsgt.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gecbpdgra.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gsqondhlg.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gphrbputy.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gdyxfehbv.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvlnpgcrh.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gztrkclfl.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gvjliphrn.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gtofqhcdx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gztkxumvw.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gllxwzjwk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/govgljyxn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/glkhonzpy.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gflgmtbmb.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gsbwukvee.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/glxmpgicu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/ghkrbuidk.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gzkgiusbu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gjtqzlepm.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/ggozlznnj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gxbwmfxtk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/ggskyiuwi.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gmblpofxv.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gacxyuacd.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gmyasfccg.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gsctdtlke.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gfosqupnf.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/glccnryzf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gypoixbir.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/glplisnsd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gtjoqxreo.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gwxxpezhg.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grmsjwfyu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/ggfjqulcb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gfggqxzbd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gtabumnys.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gdcaahrtb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gopvccorq.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gevinhuhp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxbljeqcz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gqxjhdcmo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gsmikbuja.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqiycywod.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gyrpqzhdt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gvhsanomx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gwmjngtdc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjhuiuljr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gfiyzhgsj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjtnewwyc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gpntlwwmv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gffaiktbp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqheallhe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gushnqcvu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/glzcezjkd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gqjnoovzm.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gtocqpllt.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gjlnnpqne.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gicbsgjfi.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/glnyrqugh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gcxzjxiqc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gzsrvnqpg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gakhaeubt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gghobpqgi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gkxczsjkd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gyazcpcfj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gopxhbktr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gblmjaffy.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gsfchtotl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtmuzvgef.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/grwynpmrt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gviylnixg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gzeiowvfo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gyqxnghxl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/glvwqqccz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gdptsmdxo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnyekwldl.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/ghhnnxheg.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqjjibaye.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gikuuqkms.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gatcowymr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/geqowfobn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/goooglgbh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gdrlgzkmi.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gfgqenzxo.sHtML


<!-- 参考信息 -->