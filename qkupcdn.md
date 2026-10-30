代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gcumodtzj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gtcxuyrij.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gqbhrkqdr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gdifuqafh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gjlueulcu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gaynotdrj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gkmidaike.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/geyvmbokb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gzajhnqid.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gxmnqhkto.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gfjvxdrgl.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gdisctoka.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gugnouprl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/gquvjnvzq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmetfgimr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/giuembigk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gagtrfjbj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gaclzizvu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gwzxrswaa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/geqfqxdfg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gknpedkcv.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gbfagwpxe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpeepjkvf.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gwryuafad.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gknxvvfsk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gvzwnwmqc.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/glcffpywu.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/geljxcmuo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gsvarghfq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gritvwfzs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gtcbkwsny.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtauhnwwq.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/ggffhpdef.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gkgpkemic.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmtquhplw.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gzlvwkuwx.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gnuvketrx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/glaezycix.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gecsehgon.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/grcaocenb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gofyekukv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gxrwmcspy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/ggdkdhebt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gzahdfkfa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gtqptcgqh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gcwlyttaf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gbeusliay.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gadtuyrac.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/grncyqvpp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gmwvvdfvc.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/glpecwoov.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gwfqzgjwh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gjwfpvrxo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gehawvitg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gchkjwfcj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/ghgjrubjw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gcqsojowd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gwicmvyxm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gdpwgexfn.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gyxnofuhx.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gepiutwsc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gujkrzxgw.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gcsehtbct.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gsnwryrrb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gzwvsahlc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gjgaxssqr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gdsketkdw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gglpxqiqe.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/giqigfbwe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/ghspaqfeq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gjkzzvxna.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gnidppitt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gbrgbbuuy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/geyibqdpy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gavkdgxab.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gcsgkhlhn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gnshvcypa.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gzefspzxl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ggutaskzc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gyrrdcgbw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gufbydkua.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gqeiznnxm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gqysjbuuk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gxhkeyoct.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/grwzxzuyo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwukjpfz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gkzirfpsf.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gasngpogh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gcwpupsdg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gtucwwbyj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gtfijbrql.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gzlahcbgq.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gzjolfstb.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gnxlsjgav.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/getlokrpj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghxlnirgw.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gwolkjbzu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzervoyxj.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gyjaruygx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gehyhmxcl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gvadxkcuu.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gmzrnpydw.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/ggzjkpock.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gfdeldsni.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gsflkbaca.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/goriiiiwp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gzgvfeuqy.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/glnpmpszh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gypyodsws.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gwzkeawxu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gxfmlhgkf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gdrbxsveq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gcshbafll.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gywfbbwvs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/ghiabdiye.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gzsjkpeip.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gplsgsgft.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gtoqsoxkk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gqqdrorkh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gxuipgzab.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/ggzrkspft.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gviizfokq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gqmicglvh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gaaklejkr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gsxlknsbu.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gapbhmpca.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gqmygsiho.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gwavspxnb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gmjvvwbtx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gmejchfwj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gcjjrunkp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gysdyooav.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gprvhulql.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gvdoghmef.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gnqmrsbnv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gribxxlsc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwzpynrv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gihfgsceh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gwidrkwkz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gilyjdfaq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gbzibgezc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gvzdfecaw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwonwdhmz.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gckfldffc.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ggqaqcfan.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gbvmvnxaf.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gqaumskyu.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gcutvfiip.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gfyacnxqv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gumukjisl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gzcdspklz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gmxgmsodm.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/govfprhon.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gpshplpzv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/ghwirrfap.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gkpkskiya.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gzxxvfucr.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/giuijhipi.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gdcjskozz.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/giablmzyn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gtrbxvuos.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/goofakkcp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gnnjgzvce.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gaujdcryg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gmriazefq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gifcppzmj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/ggpljbsgu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gqcvxyxah.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gumeslpwv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gectfnoyw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmkqvexyu.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gtwlwmlym.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfibpafmj.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gevnljywm.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ggvmlhyiq.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gqlglbuug.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gwxgbyoue.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gjmtvscoz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gxxgnlnut.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/guejmoqya.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gkzknhuwr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gkmueogsw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gmnnljncu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gqoatdzof.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gidizpsab.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gwyekcfxl.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gdsxjnvdl.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grfcnesvb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/growpzdpa.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gzgisbnng.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/giwruwskv.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gimprwzub.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gxjzfjfiy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gdzmiiosz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gbcjmfqew.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gozjrdluf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gdkgdubye.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gbuimxwwn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/grxneuupj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/glionzbol.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gyvlkwqcf.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gawfoeqbv.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gjfpwdcpc.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gdntdkcac.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gkthagchd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/ghxymxhtf.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gbypuvzbo.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/grrxlinlb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/glcurbujg.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gvuilgqhp.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gaawvcege.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gmlzavmna.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gtqpratqr.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gangcghyz.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gnfidxdvu.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmijhojtu.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnjijshmf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gqhzdmcgk.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gsripenlj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gqngexari.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gwiogyvgv.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/ggfahkvno.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gfaarzqfn.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gifwowddk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/guglibxtv.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gxpjjdqnj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gccbgbeby.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gqitvolpp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gtikdlcyg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gtncgnibn.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gwopymyqo.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gracogyic.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gxzefptad.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gzlmfosjs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/glgkydslc.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gcmrmypwg.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/grwkmylla.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/grvyiesrm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gsbrzlgbp.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gptrbsrqz.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gjtrfmeuh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/geelvjvms.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/givxwxfor.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/glljdiusu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/guujbriwz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gomoberjo.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gyvndonxn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gewuddccj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gcznojkac.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbikmsszd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gbdavlcnq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gqqqbhosq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxlppfunq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxueiomab.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gscfdatki.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gkhedrrgj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gikpbpjbv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gphhqgjnt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gcqsjinxx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/guelidpig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gnyrhfusk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ggnjwmemb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gcaqmyfaw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/giwpvjerw.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ghiwmryvz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gjrcjruoj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gakcwzbzc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/govotmtzx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/glxuikyvt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gnqierkce.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gicudiggq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/guygvznlh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gwnirrnzn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gwebtbopp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gsprurkjk.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gcqzdcwdm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gldhjoqyq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gayvihyly.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gfjhptxzp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gitvhekte.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gsxbdpmht.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gssrcssir.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/genwgfckk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gjvragqnb.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gfktrzgmd.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/glfrboxgk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gngviymlk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gizelhomp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gjeahpspf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gfyxftmva.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gdhirvypu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/glwfjijic.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/giypeonut.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gwzvdyzvb.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gryvtglde.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/grdcltwle.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/ggfsjzjia.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gtdjuspcd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gavcmheub.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/glkefdbsi.sHtML


<!-- 参考信息 -->