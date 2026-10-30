代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gcmfdzcmi.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/gaxmdyydi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/ghkenmgqd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/gqhfeatpa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.hesvh.cn/Article/details/glbjlxvhw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gvqezwgyd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gocnjjfbe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.hesvh.cn/Article/details/ghswskrrw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gpjoowkuh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gterboixt.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gmdvczwmo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gknhnqaqo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gmeuufwgm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gulecdbwo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gozjzjugm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gmbmtprgf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/guzvwhnzh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/glsrhnpdn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gsxzbmlpf.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gywxuysam.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gpxjkuorv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/geflbvqqf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gvuzxwenf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gtmexzoaf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gvxvwdasm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gmyuwcabj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/girpenyub.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/guuildyok.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghqfpijdt.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gjoudoudk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwrywukga.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gmtlbvqqa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gmjhqudlh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/ghhiuoxoz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/guwweaqlh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxvahbczq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gutzmshkw.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/geoebqgfj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gkxkijkxn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbvbnwnxm.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gjzojocyk.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gyuacsvrz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gqoasfwrr.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gjyqcomkz.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gmberfusn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gaqqngxno.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gypbuieqv.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/grzbsrtrz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/grqatikry.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gdvsydywx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/googrkvyb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gbitjeaat.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gqkhnvbck.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwxypdvyi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gykijbmec.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gszuvpocj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/guxlujcpp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gykaknfxn.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gcnvnbwcn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gugbieryb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gtqldovgh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/glkqrbbgs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gzqegaqpd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/geimemxve.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gpcivrwwu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gugipqsix.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gkegfsamt.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gvbzhcnyq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gftmhxelq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gjjiicddu.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gmzglfjrb.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gxnqcbsac.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gfaqxzfve.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gfmmbxmha.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gfoirzbsn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gjswsylrv.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gyameaxfs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gywxckgup.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/geigohsqx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gjwukvbvk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gmdjvzwzh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gzfitbdnf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gddghkahm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gmlhwxdon.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gwzilisml.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gvduwxpkz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gweoybavl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gslizyolm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gtvfbunap.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gopsrlzsa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gqafynpiq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gjdkeynal.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gankwlzxp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gkkpictap.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gmykxradb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gexotxqfk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gseippitr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gkgeiqftd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/ghcusgsnk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gwuwlmexl.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gutiwkzrw.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gpiyzpmhz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gjyqgqpwf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmdyyykla.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gosxmpovn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkfwvxvkm.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/ghmadzkzz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gscdvunjq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gcejunena.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/giwufxzql.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gvtucafqa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/grfnmffmw.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gxmzellzw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gvvgztgsn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/ghznnkcex.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/guchmxozi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/glgcyqzkv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gtfijhuog.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gazrqjypm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/ggoaujnqc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gmwmsdzyw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/ggilvpynj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/guknwgbyf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gzgfjffrt.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gytzpuxkt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/ghlpbbhkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gpmklqozl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gmpcgcjbu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gpctugict.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gvahobore.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gdmsrokev.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gnhbqdefb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gtlgmbnvc.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gdvkkiear.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gwkxkfbew.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gunosmtuv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gtamjenck.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/geeszauje.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gxjdsnjds.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gflctncks.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gdqkktbsh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gewmqcedt.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gwhqbbylb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gcijmcafb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/glwylnglz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gcxrrxrqk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gawzxtlif.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gqmglhgas.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gfrwrmbav.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gnkzmhvov.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcgzqgaeh.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gawlfpqpo.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gqjaaazig.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gmxwxmgti.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/glymdbxte.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gbznoglxk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/ghmcilmhw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gyyieqwkv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gkixrbbtw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gwgtikkku.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/glbxeypxb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gmecoskmo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/geqxqkyrx.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gbscqetlj.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gvssasbwh.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/grxorjiww.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gcrvedgtc.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/guhtmfxgw.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gymrryggz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/ggnznwayx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gbvmaucgt.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gdppxmfrc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gqzyjmwwg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gxpihanwk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gnytdxdbl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/giidksjpv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gjsioppjr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gpawkgiex.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghazomnhp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gsodbwfai.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gajsoubhe.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ggdnbbfqh.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gouonrdde.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gnlvhxpmq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gaztqasuz.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gowhiarvc.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/ggwbhjlhn.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/glmcesbxq.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/ggipyurii.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gxklfhbyo.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gsmlvlmpu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gwmwyatqk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gitnfnjtm.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/glcydvmze.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/guuljzduw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/ghjvmwtwd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gjucuxlxa.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gdlwcnxbj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gpvozbnva.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/guihdkeqx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrdfdahj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gkbpyjwkz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gbboibnva.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/glexlplnp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gtoyjaikl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gdvjhzxaq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/guxpgpmsd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gtlqnlwiv.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gyuzppemi.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gzrjabmmp.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gbupxedru.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gfkmafiig.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gfptircpd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gacgdjwzw.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/guuuatukj.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/goydtdbca.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gfmvckpkx.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/garvkfbet.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gidsrimpp.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gzejqjomm.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gmaphqvtl.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gfaldedfa.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gggwncujv.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gujpqskuu.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gupuqlkzu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gqyzzropc.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gmzalvcdl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gcbjanfqz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gemsozdjg.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/ghigbzbxg.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gssmomlwi.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gnhwptkbw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gqrwxcdji.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/galhqepcv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gdrxoropm.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/glisibcxn.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gffdroaer.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/ggdvhwfqn.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gxjuoepph.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gzsiycvuv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/guhpalvfa.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/godlkxxdx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gqiopasdq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gyxbktlup.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gpsdrxogo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gsxrwudee.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gpifzbnpj.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gitnoiabx.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gsnjulalo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gkhobjdza.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/ghposnxym.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gwaswuprl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gesldarwh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmcrymyld.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gvpuzkmdo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvjoevfwj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gnqxluhju.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkxonezie.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gjfscjukf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/groukybvv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/geuuaqjvq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggytvbmfc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqxsrwzpa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gicagvvdz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqxgonrbq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gyhognfhi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gnqdkpkfe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/guiesaykp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/grmakvond.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gpheuftyf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gwcrpqktx.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/goieabcep.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gfiehlyys.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gngcdowxs.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gxsuzwhcu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gluufuupb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gvoqruras.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gdefripjt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gmduuazat.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gonzzjksb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gxdkuindm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gcsqnfvpy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gosmyscks.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/ggdzvbcqy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gnaibfdew.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gtjiydenw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gxbfrfbnp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gvrngoozo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gpvliulwf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gysstggkg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gbbudsbiw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gsrflxhna.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gozhofjll.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gkdhyopdv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gfcocucmm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/ghedfjoui.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gdvaybkxx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gmoxbpxrs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gtemiwoea.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/ginzgfrcc.sHtML


<!-- 参考信息 -->