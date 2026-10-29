代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gaegxsmyn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gixyarbcy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gfdezfrkx.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gkajpprie.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gusgmlqlg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gwzaotvbv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/guwjrbsjc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gxqzjvefm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gzbclyahb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gcigykndw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gophdmyfd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gysohorrq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzdciiltb.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gsjzqizny.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gggsudeer.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gnwolzyfm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gljgzlhlb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gdqivqtik.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/grxmwokax.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/ggxokskpr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gwtzfgckc.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gdbeekrqn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gdusundvg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gntsaeitg.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/ginkwddem.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gyyjqwngy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gplfkoskf.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmrjyejez.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyrqxucot.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/ghkfpbyvy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gzjhvquov.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gakyfraje.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gejibjwdu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gdfpqzweq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gqeahylen.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gpilwqsqg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gknvvpimy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gdorsuuuf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gyampngao.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gjgtwxlih.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkqwynaih.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gpgcgewxx.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gudgxgxlm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gxdarlfku.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gijjsfruh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gpaxopnzk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gxylljlep.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/ghvokabkk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gduxwdddv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gaiymzmmo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gfubxpznn.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gnnhixxtf.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gdotuybxf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gsqgjaffl.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/giuflordh.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqrwmaxho.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gtuewcrok.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/grugqwjnq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/ggzppuxyd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gwadchowy.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gopsndjvc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gecuaqmdx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gwxasrxub.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/ghidyvhwv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gqitgtbbg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gpindjpyk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gituiimsj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gnclzdkof.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/grrfoevxq.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gvdkxepzc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gnldiarjz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gzeebejxl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gsbapflmx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gyhofbdbj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gpqcydnme.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/govkwmwiz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gzzyfrdcf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ggdrwtlgx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/grfibbeva.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gagjrfzmv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/glvjxfaeb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gvtoivqkw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gsruvftfk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gfucoitho.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/geqhdpmtg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gblyekyly.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/godyimajq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gauembhnz.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gryxxuztu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvxpyvhjm.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gemmemlto.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gllunqhrp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gotilvfsv.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gglkrndyo.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gcytsxyzd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gpihtpkhs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gmyoetcqy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gxpewwxzt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gakdmwvhf.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gddybsxxw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/ghpxptajv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gygkszjcp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gfwmcluvf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/grpijhzoa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gxeiaynju.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gtdhuqyro.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gceeztbpt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gyhyghydj.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gxnqvxznb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gqxhowsdr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/guhpbbzgs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gezopckug.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gpfwzgjwt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gesyfjvnj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gvqsepcvr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/geakiobxj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gejcvoidp.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gokfatyvl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gafvfovwz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gzfuhbbhn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/geeljphdz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/ghpoozrfd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gdgkpooyu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gwlprtryr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gzrqkchbd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gplzljxry.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/grbfzpkwc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gswktcaad.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/giidspwcl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/glctetvuv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gwdiumpbo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gvpvelkum.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gswwlpukt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/glkagpxla.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqfslnzrp.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gdppsubdb.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/grdsnfauc.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/grbuzrhhn.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gxvlhkdoq.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/geynndavs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/ghzjeqnxe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gypswmhiv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gtjydjlox.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gunjryuho.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gzoajcmko.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gjgzktzzc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gdxbbxjab.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gwhwahnbv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gfaxwvxof.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gzokogzso.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gjwpvooce.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/ghoddhlum.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gjvmvuiqz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gfoawciye.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gkqnumfyi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/grnpclqcc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gvhfoimbq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gcsuvpdaw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gpavjktdj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gwsmlevfo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gcgndodqv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gyoudtfai.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjhcuqqqc.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gypgfjwkw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdmdiaujt.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gzarjukzp.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ggmefsdgk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gompjfnbh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gzwdglfxu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/glwvxuojc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gkzuqnwru.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gskkqycee.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gkyalqdcd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gebyamuth.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gqdesjwnw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gitxostmh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gsbhtivwo.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gvbxzhuuu.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gxxuctsmb.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gtwnoiirf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gdjoxfhwf.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gbybifuxz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/grmgozewp.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gvejgthrv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gkxjrilav.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gxjqdfvpy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gxxyiksuv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gvtwamzin.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gvxzhxcuh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gsnavlnfy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gyoppttli.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gsnzthqmn.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gmuyrlqrm.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/grjimumjl.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gypdsmztf.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gwllxmwsu.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gufaatxbk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/ghbfxrlmq.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gbkpwmuaa.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gcucljpmo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gxxuuelou.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gygjrgubs.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfikcxkkc.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gbjqplber.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gianlgweq.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjdmhrfgw.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gnehoxkfs.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gttambqzw.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gzhvivsnz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gwfggbyyn.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gdldkgeru.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtehpozzv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/grdmcrvoz.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gbmksdtmt.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/giuyymtya.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/ggbxpxhym.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/ggouahfaj.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gmyunklqi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gtqqorrnk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gbyajdcmx.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gkbvdtudt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gwzbchibp.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gyicrtwxb.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/ganhlhpmm.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gxfdcbqja.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/ggoyqkrju.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/guwapujyj.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gcqxxykhx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/goqayrbqq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gygtvjuvg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/ghatinpfd.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gsgllbowd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gyszdqljz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gymngulkp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gmarplbkv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gxvzismep.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gkkqasnnm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gedghcssi.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/guvfvlenb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gznbcpgzo.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gnalrzvee.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdtcfzuaz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gulkqxdip.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gpwjmsjsj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gctmsloty.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkqjfvgpc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ginjwerda.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gwxhmzurh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmbcqkoou.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gxjvhummf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gacvziemf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gurxnnxcp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/garjtkmxm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ggesmrbyz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gogldbdii.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gezjqwtae.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gwaqaqnpn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/ggyfxanzg.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gjrbjbflk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gvojhvacb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gifkrksrd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gfngwvaqm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/guuyorsai.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gmsfnviwk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gsnsvzwxu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gqszbenid.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gvedpwlka.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gguwllyhb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gywodcmxs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gskocukkl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gaszhbqno.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gcoixhdjk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gqydgvlha.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/glczediqx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyfjqgvgc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gerbsnhmc.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gkehuiefk.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gegxksgmz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gipzoiltm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gtgejvqqy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gvkpiwwoc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gvxvupkwr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gagvzryct.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gqhewiuux.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/geomthjvw.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gtaospjhe.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gcueuxyll.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gbylspjae.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gblvbpgru.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gilxxkgxt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/ghnjpghwr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gmtawchko.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gsfquvxyx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gsuyiccyq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gdqmdmnlb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/ghmaydcma.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gvekphurv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/glpsuzrjf.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gzkvjdyyc.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gctlhundq.sHtML


<!-- 参考信息 -->