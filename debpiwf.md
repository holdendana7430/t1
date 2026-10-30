代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gpjvkpohv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gxgoicohl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gklakbgcz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/gqgspzcri.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/glziyytjs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gtjukghet.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gysuzsyft.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gurusvtfy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gumxdftbm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gvivshiup.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gxgatdjut.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gzmdhclol.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvcpszyxz.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gbqjlyspv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcowyffva.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gasnzzjvo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gfqcrrapz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gwzyqzfws.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gwittnwya.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gspkkgqmh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gvfdmvvdr.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gbhifcomh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gfjndyytw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gxcyhzxhc.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gtmiajtgs.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpjfrsnyx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/guzmjklso.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gsfvgffnt.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gqpuyeegu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/ggwjwyhls.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gehfnsjzd.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/ggthfohya.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gdpubudxe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gfujgrxgb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gbvnaimgz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gzwlzjmxs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gftpyzsmv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxxhfjoo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gweobkcwp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gkdpklqzs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gmosrmpdo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gfxaexqpb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gafdfiysm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gecgnkwic.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gjlvsdkfd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/goibnzntc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gieosokli.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gdsytthyl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/genfdozxl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gevrjaeti.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/ggralenvb.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gpcdwebmt.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gunvyribr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gizrbpxvg.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gviumypkh.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/grdnfgbem.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gmowqszuw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gftnkxzyw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gumagqcyb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gxncbskbm.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/geqodxuwu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gxdtrnlyb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/ggruptgtj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/glzggvouc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gglgdnxyh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/grsmvoiss.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gjnnqjpbj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gmpwunapx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gqecxyvmd.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/ghyljtbzm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfyhbvcyo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gwipjjmjt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gbkveahdq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gqcewdyga.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ggafqopbj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gtcmzhdwc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/ghehfgcow.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gukqdiwpx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gvlhmgdvc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghxmptgll.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gjqckflmd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gcsoiworz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gpjxtiahi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gefhsoxlh.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gbpzyfyos.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gsxbflxqe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gmwlstghp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gufyjclbg.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gnnuwgbcu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcdmljalp.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gumskpzbj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gvupzvemg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gskopskwd.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gbaeiwpce.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/grbyprutl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gwxshbkdj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gqxhrhcnn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gpcozwuos.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/grbkapegh.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/giqpxsvnd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gshmegdek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gmptdsqqh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gzhudmbmk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/galrundfj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gkbbtjmhy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gujonielg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gfhyfdcjc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gnyrlpprm.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/ggfraamsw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gjzkdxkcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfhxqejbo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/ggqhxsmqa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gxigqxvzk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/grlomwcqc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gerxushds.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gqgtwzkes.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/ggbxvtyap.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gtgqvofub.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gqtxyxtlo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gpmagurxh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gzmqygicd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gfvduqbxd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gvulvqpth.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gjnyhoogi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gbsyousew.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gutvyqmye.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/ggnjthgtn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gydvauwun.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/giixaruli.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gmfbgtfwc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/ggolgbyqg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/guadlhcnj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gqeuizoth.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gocrgpzlu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gihxglhvi.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gadfoyzcq.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gpupkyfqp.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gynymqyxj.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gyilhbeqs.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/geaykzlex.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gitwafmai.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gmjjvvfns.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gkuxkcrcv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gdjsgxlcs.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gqghazdcr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gjlxpgsbj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/guxwixeli.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gryuypyqs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gbrdnlbws.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gszgntzex.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gowuujxyv.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gbcossipf.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gelrovyig.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gugbueyke.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gmkswovgd.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gsnrdztqe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/grsccnjfd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gnqbtxcre.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gxbtytsqw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gxkbaiiag.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/ghwlomwke.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gwwciwisk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvtuqigdh.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/ghnabnhxl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghmgbzwna.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gyvvqvtrt.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gozcxivhv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gqirmksrl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gupolswlz.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gciooicpf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gfynepkpq.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gpptxkdlo.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gtywjpdqg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gkqchatld.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gfhxprbxi.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gwufcwqli.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gsnsilxqn.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gfiqtsukq.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gassijxki.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gcngvveqh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gqivkfvsn.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/grrawixnl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gvmdulceh.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gkvkxjwmy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gbxufutea.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/ghnpmesgw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gdhqqcdmr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/ggxtzqafm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gjajqszcx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gjzhzrqpt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/grhewjohd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gaitlfsfm.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gikexdtpl.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gnawlgdbl.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gvofkftsw.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gxracxqnb.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/glshaocwz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gvbovogul.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdgpogsbk.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gxjlvswqu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gkmvettbt.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gvxvbjwho.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjrypwbfb.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gvhkwfxmd.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gurcghlny.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gvukctrxm.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gijykacqo.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gibfizopj.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gmswjpefs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gofcpnjsg.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gnesptams.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/grfvwajoq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/ghwcfvctj.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/ghngwjapu.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/grrqnkngq.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gzzjixyni.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gfskppvzs.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/glyztacak.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gleupival.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/ggnypxtlz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gcxjwmpvl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gwhsuosiu.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gzxdjnlga.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gxgmtlwuz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gwwxmmjjp.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gwnmquffl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/guwubkpnk.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gjpgcgjuy.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gmcxkigoj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gjwgnpvsm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/glivlpyvz.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gsdeawmlx.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gdgvbziyv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/grezfjjgl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gbitlsxxh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gzivxdoli.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gxfjszpsx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdmeyrmva.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gtcebknyp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkqlullek.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gemknwusa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gulxwojah.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gkdanwmwy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gztychcuz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gxakalnfw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gckipngkr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gpzentvut.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/ghfhcryja.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/goksvyfrb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gzzhxzowy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gdyzhxzyn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gtegedfqw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ghotkhwrx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gneuyskfh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gumdrvaxq.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gxghejnde.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/genmjrrhs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gteuckfko.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gppoaumsn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/giarsjfiv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gvprudwuc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gcwezjagq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gwznjjxko.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/givvsegng.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gwehcpeod.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gjggxojlr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gusnznoos.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gcupftebq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/giggdlxyn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/ghaqjsczr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gjzmtmrpd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/glvoebenc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gihyzyzfx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gexkqxosd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gvtiyvuwb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtsnedsmr.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/grfhyxkdk.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gwwicnlfg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gvhfclcaa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvysiyfzx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/govgbgfba.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gzkceqedt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/golcbqspt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gmpoysodi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gnfekogab.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gjttxurhc.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/geoctuybn.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gmsgpuhzm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gneagjbwn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/geivufldj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/garcugqsj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gfkyckrch.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gejyrycte.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/ghqyyxxzw.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gyowsgaid.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gdrwolasb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gbnqnimlj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gowbaahgw.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gzrgqsmbp.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gvilokpyu.sHtML


<!-- 参考信息 -->