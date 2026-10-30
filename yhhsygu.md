代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gfpzgpjfk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gtsombbnq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gaomcxonw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/ginihdrtu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gpauhlohq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gdcpscmyj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gsclgmnup.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gpscasyli.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gwfhnrpgk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gvftivsde.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gmqfauwrg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gqwyyhsks.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gepnphvew.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gwrglbbpj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/ggsomvefk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gdmleedco.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmhixukln.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gontnhleq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwxprvnkm.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gxlorvxpo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gmbvubslw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gocurvsou.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmpwvdofg.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gecpwqebi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gdkzvafal.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gluosqznh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/grtmiwspw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gwsbigmrh.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/guwpurwhs.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gqlgbbdkm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gtzwivicp.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gqekumctx.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gtngubiuj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/ghihbjpnt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gcelyiwqz.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gvomjimjc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gjbtfojqn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gdlpcbmui.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gjaysbmgz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gnahvyefb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gblkgevfz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gzqihmlyj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gaugdcuhz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gxqoxkmgz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gcdkubjmx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/grtruzabg.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gfrjdnlcu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gqeqgkwdw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gfxabccyz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gartakdlp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gcwwanbxr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gktrllhbo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gnzmvfnen.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gteneazrb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gdwwdwbbl.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gljcnzamm.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gzlkykjmv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gtkeedqwx.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gebycluwj.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gvlejqqvw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/grxbqtzeh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gnquluybm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/ghmfhsoft.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gbdncrfuw.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/ggbzmhpwy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/grfvyqnaj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gwgjsoppu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gpuktuhjz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gnipesttl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gzcbnapyv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/ggqtdyqdb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gerfxikck.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/glueavzlb.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/glfhgfhar.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gxqlusdos.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gwwelbouh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gddjyxbxt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/grqczivvh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gavdwzqrz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gqnndjcfk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gqlnownsc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gvnjwgtui.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gaewppkue.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gbudewxti.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gibmwycwp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/ggywmolks.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gvgelefml.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/grydsnpuv.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gluylozif.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gsrgyxcst.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gsqbohvyd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwechhhhv.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gvepkvnam.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glwcpufyg.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gncctfoax.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gywkyizyg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gsuzagsko.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gytidjaik.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ghqwdvhod.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/garmalkds.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gbenclwgi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gltxvnrfx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gxdsfhzwl.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/giruypcxe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gcmpciihb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/grcwzvxle.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gujqlerql.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gobtmmwhw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/glzmksygb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gqtniophm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/ghipvqlof.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/giyvpuadq.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/geusxamcb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gwnxuaemk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gnvmkpsiz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gfhysmxeg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gmwwcesjl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gsqeegqzt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gfaeeovye.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/ghzjxluvf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gaueazilp.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gpzkiadyj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gcvbwjald.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/grjjfrzpu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gewtrqaps.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gczxklqyk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gvlobttvp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gmafjxpas.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gkyoqacqn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/ghcxhozvw.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gyztxlxky.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gitmrxkqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gyaoyrktk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gudkguveh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/garupxqof.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gjgwupgjv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gdhkrzxpx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gwcybqinp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvnxkhwyl.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gdvubgsbc.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gnoinalup.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gtizrlgfh.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gomqhwggq.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gaacvvaoi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/grhrjatvn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gvrlxkpml.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gsbigvese.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/guwrnnekc.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gclmscmpv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gztpzgozk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gvbhtcumg.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gwkxokgpi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gbihnbdll.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gwrwxsoqe.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gkantqypq.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gnzbqssom.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gxjrsqahm.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gvnhsdvqm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gexybxyfv.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/ggvgkfwmd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gydsyrdsw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gdpnficem.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gibfxnsaa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gpggcrkmc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gaptsjggc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gkhhnljnu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gktaqdtri.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/glwuowvjv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnuyhlajr.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gwvotfalm.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gamyyjdaw.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/ggxcoimtg.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gtjjqznrc.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/ggszmqkjs.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gkagulmap.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gitkgawvx.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gcuscegkv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gvzsxbnto.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/grmcietgq.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gxijkjbtj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gymaimgcg.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/glshxsbcw.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gzmzmgwdy.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxagbkfi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvspjwbxa.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gbeczqxnw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gqwcfjeif.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gepugagrg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gwxiqpkie.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gnfnzwkdj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/girtfplyc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/ggsdojuib.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gqaxxfhzh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gdiepnpqd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/ghpanjqha.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gbxmmzznz.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gqxcqmnnh.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gycqtfcek.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gapglsnsj.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gkzwhjvho.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gzanbguzz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gljsegqhr.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gzyzwzcdi.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gpiubjepi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gehxqmpnn.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gkiqyehvn.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtxthbulw.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gmiyodkji.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjoyjqbrs.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjmovdnmc.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjopxlua.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gxkjizgcc.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gmwnppfdf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/ggyxylsmg.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gkxgmuujc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gkugjrjmc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/ghytraxmd.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gzimtabda.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gviqinpkm.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gazxdsscf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/glchzvvqw.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gfebdjwdv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gxvvoniij.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gbocmyiup.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gaifcasca.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gqmeejhub.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gvaubbccj.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gvaxbhvqz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gmemtnyfr.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gtkkxguec.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gsrxkcqrx.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/grbdemgcv.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gtcfcmwnv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/ggtdncacu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gioyuewyg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gkwklajth.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gmdkqnoqa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gdfleozpl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gfblnoekc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gcedthlfe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gmrrugayi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxevqtimh.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gdmwvthwo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtpghfuct.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gpgndwvng.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxtvwitcw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/grudydiwz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gubjcrucb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gfczbxdie.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpxmzkpfy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjotxikdz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gaziwoinp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/guvxldmol.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gknncians.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gvvqlfzug.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/ghujzwcre.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ggioxhdeo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gpuunfjjz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gucgmelzh.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gyggnhcrn.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gumwxuavm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gsaudzaat.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gdsptwryv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gwrwmdjis.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gkweevrih.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gigawcaws.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gklbiqzgm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gnyhynopt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gxizcarsd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gaidqwfvg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gyuugdnnp.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/ghyypwpfw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/goygrkhop.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gmjalpbsb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gofgunevz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gzwxplnyt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gggardlae.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gwqygwikj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gpyxxkbyz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gdwqcypmk.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gzltiwpxa.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ggmrylmox.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gnggienam.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gsycsdash.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/ghqbxvigm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gylfwdatj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/ggnianzcy.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/grozkrttz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gjsxxzldp.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gtiilbhiv.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gefjgwere.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/giqnwquny.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gxmcvumvz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gzbfbrlme.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gculthahx.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/ggajemurk.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gwuprjvem.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gmqddczhg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gcnddfdxy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gaddxlzxe.sHtML


<!-- 参考信息 -->