代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/ginqlrymm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/ghdexepeb.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gfcmxeacw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gjjmgtrhf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/ghmnsjfbn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gzbtsmmje.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gtoumkjyf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gprdylwzb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gspxcrsjv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/glcfyeuih.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gopjdmfgb.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gafjvcukf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gtjthwutt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/grbbghaja.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gkfnfgkyt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gnslsjvtn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gsliyyzcy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gehorqcng.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gmnhxcrkv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gmoajqkmb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guvcmzety.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gueyynqps.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwwzugvnr.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gfuvaoehy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gvwopqdbq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gzhpomuod.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glmggwauk.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gogyfvdgi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gwbodijqp.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcanaddsx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gpzkkwejb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gztcpmpaw.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gsqxllkph.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gkhnbwbib.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/glgcdosml.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/girrdafgi.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gmtozalla.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/glmwfytpa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gcjdgduxy.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/glatbvqch.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gujecbxsg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gccydcbqf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gvoeiybor.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gduyqyibk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gzlyfadlz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gmhrurtpc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gnriuaxym.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gxxfzxpxn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gnexzifec.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gdsubupci.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/ggfqdsrem.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gslrsuasn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gikhgwhpj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gbqntewsi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghllaijgd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gslkkkmmn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/giefyrvjf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/guohranxh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gfydshiuo.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gqfwoxgsr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmdnuukgc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gbmpvnmfu.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gpywebzpm.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjbltjfvn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gftvgeakd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gazmlaxil.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gbzatbdms.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/ghyqfyfxu.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/guskuzcsa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/glrgvrfob.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gvxkchxsa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gtaefikmr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/glxegtdfu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gzmbijfja.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gnhrogyxx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gaybyxfpo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gjyvnmxpf.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gdpzonbhg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/glbwqicih.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gvvpoeudn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gouerwrgn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gkdptszha.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gtttbukds.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gstyyrsxg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gfovqyxpq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gutftmsgc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gzlbtofce.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gjuwpriha.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gdlyxdmxa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gmxkvhjho.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gyoldbllw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gcjldilcu.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gbycdtgzs.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gbitwkqdl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/ghzgslycr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcqvswxbc.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gwkaaqdok.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjxbmjekv.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gwavkuppv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gcwlxksmk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gaugnnvor.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gbgovhczf.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/getbribkl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gqgzhwjfu.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gzfddymqu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gcfnscncb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gwdlphhcn.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gsbeslsmb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gtymbgjwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gjjnxjyuf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gqjleelph.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gdtwypbem.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gxbsojvyk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gaxwgltkk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/goagnqimk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gawfbhvjd.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gikieayeo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gpiiwcoin.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gjpyvddte.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gpnpnikph.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gukasjjxb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gtsmtzxvs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/ggshqcbib.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gpxowcddo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gfjpzodol.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gbuhnmyme.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gmwtndkws.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gidkzwvbt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gavwzqszv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gghiiifyu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/ggiecqlsg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/ghprwjvcb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/ggbxrjltr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gzjcunzfx.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gbmtdedhs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/glcventjr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gjdeocsjw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gpgfbwwai.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gfnybyagf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gowyhqxyh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gvtlxuxxk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/glymexazn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpxroyjns.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gjnaikmyp.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gotvpagkl.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gsfekgjkx.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gwegjuvcq.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ggdcudljz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/guujzhxji.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/getagvbcs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gtxloaxqu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gulpckzmj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gfiwwpbva.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gvvzfirzi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gihvhqpcz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gjkdlgmmb.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/goetondvk.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gjbdfiunf.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gfvsukeno.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gepxlbusi.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gaahkfnbp.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/getusccjn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gzmpvpiny.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/grnuqvvty.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gjjrgeduf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gikgxvrgn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gudtlujyu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gkgcayoop.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gczpmcgaz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gkvibyabk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmdvqyjyn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gjmqamscu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcupynaev.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gvohrkooi.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gccxkwcta.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/geqvoohzz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gepirbxlz.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gfhapmezk.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gddrkzxcr.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gmezxojyf.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gihqadokf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gzvczogyg.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gikbfgrct.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gpvecvulk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gvbxxmdez.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/giiucfpfa.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/girycwbgp.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/grlywofad.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gdvgshxrv.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gvykkjtmq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gtkxgobco.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/ghllbjycr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gbqddubpk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gtapbjapv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gtrqauscm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gzgsxmlix.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/golcdhpkw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gycihvlkb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gaphrszur.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gomqlhqtb.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/ggphrjmph.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gummnynpk.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gajocchqw.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/goaluwbqt.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtxmtihv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gkyhrjbzv.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gbkgpdypw.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gchbkpzuw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/geeqlvoju.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gpcujiztb.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdrcvulzr.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gwefiitcd.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gemjqelgn.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbzfbwshl.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gzlxkefsc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghayiqmng.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/grefdfwxr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gvbmjwpiv.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gvwmazsjt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gmfejolbd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/ghrvzlggp.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gjjzikeem.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gnuwdzehg.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gjtvhhfud.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gajzbwazb.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfwprwr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gzyerqcnj.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gihwdoawb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gbcyffgyw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gxsajmljy.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gckhgfcst.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gwxhculag.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gomkuypnr.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gnhhlvxxt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gqumwgdbk.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gkiqpnhoe.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gpojtnazi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gzjqwrtel.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gfcdysnzt.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gljnwprat.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gcjeelokd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/glcjffmqj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gbalysmab.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gtnmnahqo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/glihjwjfd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmstyszcp.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gjlimafbw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gymuzmoxl.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gogfiebtj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqmiosifc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gclkdecry.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gsujavffx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gtnsjibky.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbcvrfnor.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzsgzojdo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gmgxduqzo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/geofltjps.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gremzpxal.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gdaezgtqr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gsnuadvpq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gdkvznugi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gzqsfwipn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gzuzqilda.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/glkydhxhh.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gzomvcsqh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gctzrovfi.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gxekdvwhz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gxgxwpnjk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/guiztckpd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gsgywlzdf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gqzexttfw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gswpzinij.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gehxfdtdo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/guvqfuxhr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gpahqafji.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gymmxnxrn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gcbldjaes.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gflhjqxzz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gxsyawvnd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/girokjtbq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gjlvjduos.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gcrdvqxxs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gqxqezhia.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/grtjnspxi.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gzggyjiov.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gtptclawp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gpuxuqvcv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gechooyep.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gqlsmcjto.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gjuyxwgww.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gokkjtbne.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gavnznxpb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gicqrfoac.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpeluywgx.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gpnxfajep.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gczjsujle.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzphdmzup.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gviglfxyj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gttfqauwz.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gifdrsxdc.sHtML


<!-- 参考信息 -->