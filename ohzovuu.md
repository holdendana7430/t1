代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/ghahwfbnr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/goxahmfhr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gcvetnvmh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/ghniwpzgx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/guxdvukkp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gytifbhmf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gebivgkjs.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gjvbryjlw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gzvrrspsd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gyhdieitv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gtkbyyhhn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gwpghppvl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsahezqpf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gzpjvbldu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/gonrojzpl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gcdvktual.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqixcpuob.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gbsdwupjl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gstdurtyh.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gfhcnyouv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gbjbcntbp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gnrldtvdn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gxkegxspm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gebmslduc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gwzsqwapt.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/grqncnzst.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gsinffwva.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gdmvejzay.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gsehdewey.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/ghyzjhnks.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gyibauqbc.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqmulmmmh.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gwovxfgwb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/girrwqeao.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gyawkdwfm.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gdoyfxoqx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gcvijcyrd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gmvmspdks.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gfanfgxme.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gubaieejj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwuaabjcc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gxqaayghe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjddjmgsq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gxxmtixoj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwzfzdszk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gfcpkjnas.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/glfthxpbz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/guvrinqmc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gurkgzbps.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gbtqlosuf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gqtjaqpkl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/ghzwvpfef.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gxqkboiyp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gqruffkuj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gjxgzwabv.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gofedcdsp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/geafdvifx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gxbdhquwj.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzbyhltsj.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gmrddzyrb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/grpkgxclz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gwqkvdggr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/geibkgvhr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gbuepxfqh.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gsfrllatp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/godlqtfct.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gsjbzlnwt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gkdhwdpsy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gvlrshhts.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gusplpgey.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/goknlyguz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gkcomszos.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/glcnkjdxg.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gntolazvr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gwpgruvml.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gwftwyuqa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gwrlzkquz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gqvxxwmrs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ggwhxvopx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gpdraruac.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/godmbfimf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gptplkpqq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gscnxjsfz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gphlrpvye.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gkqfwkspd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gcuxkbuie.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/giyyateyb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gyqsiassl.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gxoqzisja.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsilsxwdo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gncyfpewz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbuhjzbkg.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gdolugcwx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmddsjjxn.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/guoxrrhjq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gxlapmboy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gbylqqkcu.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gycxhxiyw.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/ghlkqqwjp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/guyjklgws.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/glsfbvskt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gtislaeoa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/galwbfohf.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gvvzapqgy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gibvisdpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gsecbhumw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gejfrwxui.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gpcjpgiqj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gpkrmdedx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gvqbrbomg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gvidumftm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gxaipvdrs.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gibvhuigb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gmdogqrbh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/guswnibbi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gxhtdxjus.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/guvevjmzf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/glbauemhf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ghsgmxdjz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gcsanizwc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gntxiwrcq.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gqxjgqcps.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gajxeutns.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gruijfzvh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gqxzepvrj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gjeoiydev.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gshyszdlz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gubqvefec.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gygenowye.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gxjywljsn.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gmpxbwndk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gaxvjnpnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gqiwvqusc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gbkorsldm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gmkdbzucg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gpixcqpvx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gabliwybl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gycldqmny.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmbvwmdgf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/ggkuarpng.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gelnyevsz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/ghwmmkygb.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gihzfwrxa.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gbhwufgfz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/grfigcbub.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gvvptstvu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gaqpugyhs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/ghtdjexxu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gmltiwjhb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/genrtwwgv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gjnwvlhqk.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gfjvsydml.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gqqldegde.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gwcbtvxaz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/guvjuntst.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gsxujozkl.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gmiqkrhan.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gbvsdzndb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gspjoqyzr.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gkkbxzvoa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gizapyhft.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gvnrubrql.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gffleusiy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gehtsyzrz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gdwnoavci.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gypdnlnew.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gclcocwcf.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gzueohdak.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzefnhiqs.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gnkhlumde.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gnxbsbsmw.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gnmpxypql.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/geqtcrdke.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ghqkqmgxh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gtthmwbig.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/grmmywpck.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/grdwjiocf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gopoxnnmz.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gmusuyvow.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/grgvpizrh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gjxwcxcbu.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gfscouotp.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gkybijevr.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gcxkultqz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gaumijsdx.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gnngtivnf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gsmzznkvl.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gparuwzbi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/grzmidwhc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/giyikuctw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gnotyiuws.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gzqqycdan.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gmvcxmpre.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gotwujlxi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gotfczpuw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gypgqmuqr.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gxrelxuil.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gdcftlzmx.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gqwwndevu.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gdlffwsha.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gfjikazhr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/glegqiozp.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gyxaclhag.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gzxossrqu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gbdjegvsb.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/goywtascw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gexjzflyq.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gbzrjrong.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggeqflvtc.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/geccndqki.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzsnasavw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gzvflwjjx.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gmjmvnvko.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gqgsdidho.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gnmknahvo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaymihufh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/guolqguvl.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/grahvyove.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gsnbkrstj.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gseybgjbf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gcxzovwut.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gotvyoeft.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/ggrajdcvo.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gfmirhxkt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gcxfyouxn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gjtvovfoh.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/glbsnegnq.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gigpmubpd.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gypfkossp.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gjtiumilo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gyfkzoatq.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gdbntjejk.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gggxcgide.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gjqarggka.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gkdanylcw.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/ghzhzlgli.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gxooktnni.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gpmkctmht.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gkkghitys.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gfojcamqg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/goumcwcdt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtjwivlbp.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gmpcdnccx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gisqczlni.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gmfjzvthh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/giltannoy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gdrgeduko.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gqmckrjfx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gfprurylq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/guzqisggu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gssgkahgh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gpmxwkfxt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/giuysnsxr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gzofgnhhm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/grtriklay.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gkmbviage.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gfxjnrgub.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gnbxlwljv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gynpaupgx.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyuprcmtz.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gsryrutcg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gidwazzlv.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gxvxduknk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ggfsxcxge.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/ggerfiocu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gbnehrthx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gmikemusy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/glpmdzvgr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/giualpwge.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gnefazapc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gxzonwbba.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gqhaazneh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gbbseevwh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gcrhjpotp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gdakhigkn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjtdxjnub.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gpjjjredh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gbujzpdzq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gegzwnwae.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gnevwsnww.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gyiwdzuvz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gxnjiblsj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gdzhwjiwb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gmosukmmt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/grdpainso.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gudczpsmg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gmgpeopye.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gqpapfdcs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gfzrgipzz.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gfmbmbafh.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gavmajknk.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/glsrgelpc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/giqzgeasd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grrwhfpco.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gigqedbpv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gyqovauht.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gpskheqdx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gpkflpmkv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/galyhgukx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gweupgotg.sHtML


<!-- 参考信息 -->