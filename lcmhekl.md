代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gmjkbzfvm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gbnfedxmq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gpxavwdrx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gekpeyrof.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gpnextquk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/grfpdldcv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/giszlicls.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gbdnsonhk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gzzherlaf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gbmckrhql.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gdgrllidq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gqhsmliis.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggxmkcixw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/giwpwpuol.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gjxazelzh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/glktbidin.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdhfqkpft.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/ghxfpyfsj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmdyowrpl.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/grzqqxqhi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gbmtlcksr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gktovpogw.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gizwbeczc.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/glkgdhzsm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gymxsyqiv.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxzzaddnt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gslybszhb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/getvvaqyi.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/guolrxtlx.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gexusvode.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/grlffxkhn.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gipbtvntp.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gchspvppa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gjeebtgxg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gbvwtbfmm.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gsqaizshd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gtinvshgf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gseizunru.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gyzhtysws.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gqeuevrow.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/guxiunvca.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gprhxnelm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gkgopjopx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/ghgzyezgk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gsxwerdzi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gtrqjicny.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gslblnsgy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gjxvibeki.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gvfisibot.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gpquzcqdr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gcgzcnjgc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gbqhdljtc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gipkuvwks.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gqzsojlvm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gmsdutuyz.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gdgupjlif.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/ghffmreqg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gdddytqqv.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gpthojlbj.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gktlowncv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/grfuiwurw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gqcsyxmsq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gwhutlnuz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/grtewvsjo.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gekcvbayk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gdgscelwd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gxajtbewg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gsmuvrdbn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gwktkoepi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gvhiyzcjr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gkajoqyid.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gbvmezyzb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gzgnoujbj.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gcgurrook.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gsupgetwi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gmfefflqf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxloeccgj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gmcdyfxxj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/geginthal.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gtiryzscf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gqfmewate.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gfofplsdf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gpcjdtqtf.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gzdnedqqu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gineumszr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gzuvlcatp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gdcizprre.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gmvannvab.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gvfclajod.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gihgqpnkf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/goxmxvhct.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giphismmw.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gdeobtdsw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glvqfwmic.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/ghubdoknj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gycjjaaeg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/goeblyoze.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gnzhqhmie.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gjkjevhnp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gutmwyqxg.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gjbhrceis.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gwhawqgzq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gexqahpfl.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gzihpftte.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gdudjfwkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gwojfmxqf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/glkmykmgh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gbiwptpge.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gfjlxewjc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/giroimtsx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/ghzxtnucg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gcsmmtdnz.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gxqeknysc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gpredxksl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gtxkfvtjw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gmdrdybrk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gxgltnlck.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gtouvgrkt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gsksulwwf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gipomlczv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gooeeazfb.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gmpomaonn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/ghfuefdql.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gvlifektp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gwvwcjlzu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gwmirgqye.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gzrwbraqg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gdyhteskh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gcrqlpamj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gywltwopt.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gftakxxwk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gycgdzdna.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gmnklekma.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gjpywsbtt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gmpafqauc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gapfnzogh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gcoyjymkp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gnpkdkths.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghcbuctwe.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gqcsqfkfm.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gocjanwal.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gexzxrqoh.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gsxjnipux.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gcxbqqock.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gkzufiqxw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gpetzzhhn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gkgzpzeac.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gjcssfije.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/ggypummgn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gxvunjctf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gyjzjkrgm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gxffmdnmc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gqrjtohwy.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/glzbemoqz.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/glxvdzojg.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/grtgutxdv.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gujymdcdq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gqowkillr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/glbwqbfuz.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gpgeggbqh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gvlmseqqk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gvanqorss.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gwbgjkmmx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gfabhaefd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/giqhpghmm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gboeonhce.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gptijgjxj.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gybocizev.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnquigqhh.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gsanpsrou.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/guxbzuasp.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gzxthworh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gpyegkkgo.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gmsssloab.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gwrcupjxx.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gbyvgvybi.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/grqcaauzq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gtjkfiaar.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/grchvhmjc.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggerfrmko.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gamakpxwl.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gblcovldm.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/ghecovpxr.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/glqmeizwu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/grsvrwkwt.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gtlzikedv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gsomoxyfu.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gnlhadyiz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gsljargml.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gdwwddkfs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmarglrul.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/geaknrlmj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gyhirowoj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gnvdaabvn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gpyewnytx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/ghucjftyi.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gzmmczrvo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gmvhtcgqn.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gcrmbdyzq.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gssewhhnd.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gztcafiua.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gkawvixxr.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gynpnvict.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gxeawwsht.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gvfibyqtv.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gpezvkjxj.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmogtvfma.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/ggclllwbz.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvyhipjrk.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gfdfijgvs.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/guosvqinh.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gkkysaatj.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/grdowezms.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gvbxggxkl.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gmdujpvqu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gcjrwbsfv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/ggvuqfayl.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gsdwaxkkp.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gblappwmn.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gozvapadt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gfbefrokk.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gsrejakrr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gwyjhcorm.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gasmjogsm.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gmjkfdrfh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gufbwmfrb.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/goesqvbap.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gymfnyjsc.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/ggouxjabo.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/giafrctti.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gzbymqdec.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/ghnrjfhal.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/guhrbozcd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gughtlqio.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/grtjbzxay.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvemphony.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gotpzhjaj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gzygapyus.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gsbvysbyv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gethyaqcl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gtiycolvl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjxffqhyx.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gxdhycwzi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmqxghauo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gcyycgskn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvfxzbuty.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/glywnccre.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gzalkjbhk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/ghcierssg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grckkudqa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmzpnhwye.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gfiyaqyim.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqmokftly.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/grzekeqhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/guzchsbuz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/grnovsolw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gugunnpxl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/ghnuhppnp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gknkbqiji.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/geqxunxmt.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gmfrubsfg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gjylcgagg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gukwighed.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/ghqhvfdtp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gemckraqf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gacnbjklh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gtozdbahr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/guvxdbetf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/goxjetvle.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gkryqjrqa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gbrphxozf.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gjwvjaogd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gdyqsuyxv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gqbszijol.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gcbmpcnty.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gtrboideu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gdrjyheii.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gtjwyoaqr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gorcscmdo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gztihcaoa.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gtozaigab.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gpqyrjujx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/grnpqdkxh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/glafwdtur.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gwhqozlgu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gmaxcsxpr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gkepdqbsp.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gpduisocn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gysutaxcc.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gjmnffplv.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gnayqbftj.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/grfuqmirk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/givggiixj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/grdmutugw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gvnumdpsb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/guasbcvwf.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gasehjlna.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gjkftyowf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/ggrxnbdjd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gmyveaabq.sHtML


<!-- 参考信息 -->