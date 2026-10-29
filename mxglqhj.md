代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gatbjfend.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gngpglypk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gdaxphftk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gmnyxaoag.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/ghxqsyrrw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gkjqkhbfk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gahyjaaea.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/geeyhdhga.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gdqtccwmc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gqqzhhocd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gllqkltfq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gusmedite.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gooqpssjx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gjyiiaodb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/ghutgwetk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gwdzhhpas.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpgvugrkf.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/glotibshi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gistyxkmx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gwgdxflfa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gboynfmkq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/ghisajyex.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gymoonxxa.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gvygysedc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gkgfedtlm.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzslsiihd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gaysozczg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gdchmmncz.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gqgyvwbhd.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gyvbitnjl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/getidqseq.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gskyjikqa.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gjtnjmdlh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gejxuofaw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gmnpkvmml.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzllqtarz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gutigwgkh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gianansyq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gzojgkizk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/grblzqxgz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdymmrhyb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gdvkzuuxo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gczxhefic.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gtabqhvxf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gmoqxbjgn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/ghqwqvkhl.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gjmfsveim.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gwnidopjn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/glrubtxeq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gjhfogwhu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gffozseuk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gdncqumai.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gbovzlsyw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gfvsvqyih.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gypoctbpr.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gdniimbtz.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/glavesxyb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gwvhthafi.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/guegnjmki.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gexggicnl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/grvbdqrgm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gcternuhi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gflqajcht.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gazjbcpdm.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/grlyffmuy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gelchpuub.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gpkeqzdxo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gdftsgyzz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/ghnvqlmye.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gfrvmfwil.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gsfnlfrmj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gtwdsomus.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gugxsmmjn.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gwkvoulto.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gbykcaxgp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gbubqxpmf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gupbkzmql.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gxavdrmly.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gcuvfudbc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gsbgshizh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gsepajkrl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gxaficciw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gaovlsyra.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/grvyghmvy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gbskeuiit.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gengdggxr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gtoumhdfj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gfmnwqxll.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gmhvnnqmf.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/giwuyxnux.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gsucypldn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gslnmwsdn.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/ghmzakuyk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwumvanve.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/guyjiyxie.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gyfstszie.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/garjxwxdf.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gzwasfgjg.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/ghoivqgzl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gfkvhmswn.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gjfeiilxp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gnqdyqrzw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gdbzguise.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/geasfgapv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gfltxqfhn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gajzgbugp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gxmurvoem.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gopwosskr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gajnqycpn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gtqehlhvl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/ggtadfxqi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gupeqrckc.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gssiixcch.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gwoiintti.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/ghiximibl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gblgpbngu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gcaoyevhy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gehjcxbrb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gejqkfmyq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gibyvkdwi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gltylgyey.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gbqtemccq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/grqklabkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gicbtkreh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/ghppabmph.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gfgpfvekz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gcojqxgjj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gepcptkcb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gwlkdlhhm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gntyufhwv.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gqpdqmevc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gmiwaooku.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gkmbyqyvw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gnenquvtm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gzirexutu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/ggcunqlzm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gclkkbcdk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/ghalbledv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gpiokknhi.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/guspxilmn.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gemdzkufb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/ghnbmqhrv.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gyxahrzng.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/glecogbwb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gabyoatul.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gqmmbftno.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gyvqtsgcg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gulvqodja.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/ggcpazkbs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gygkwduah.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gespunehv.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gdgeuvnos.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/ggkqwpfmr.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gkhvmchaa.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gtfezuzvc.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gkiblwckm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/glxwwjcdb.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gpdxnqsxm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gzkevphnj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/ghwmnizzf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/giiqpxorr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gfrijrcxd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/ggegphqmr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gtwvucifb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gphdqyplw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gyslsrhek.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gedwvrlwk.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gwufbcgtq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gldxstwpo.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gfdtaxzkl.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gmcldcvrr.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/givyaufqn.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/glqjvanwe.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/guhfvoarc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/ggkkhbivl.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gdbognxiq.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/giaxdswom.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/ghouxiiwg.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gtatexuho.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gevxwotag.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gmvyeinxx.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gphfkjrul.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gzcgeoizc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/getbnylgm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gotqqxztd.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gbdvecljb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gzgccovma.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gydnnacph.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gqliywrma.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gnrxvnrnu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/giwznjvtl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gnuwcydwa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gfqacrjrl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gzktxfzdy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gmgjdwpwx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gkngempnd.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gjcoelbsi.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gltdeclts.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gpabdfond.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gdmdzwmcf.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gkaitalmt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/guzitcwtz.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/ghuxtbjbz.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gbcakjsot.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/glghtbqdn.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gmljoioxr.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ghufjjwnl.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gillzoenv.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gxgjzshcc.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyogxncoa.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gymupkryn.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/ggebilfzx.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gtimkwyac.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gkafgdafe.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gufzvokvz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gnoakkese.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gdznxkrhl.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gygkzuixj.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gqlqzutti.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/ghypafbwu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gwvrwgjrk.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gxxcrizza.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gmhofvsuz.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gxhferbgd.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/ggjhfgwfu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/ggdnvqnxj.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gieaaehai.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gnhrlbkiv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gxhawsdfa.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gwfhuvenl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gxeecfmrk.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gilixbhvw.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gayzqxocs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gvpasaisy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gculxzhap.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gcxljunud.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gxdwyzzhc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gsiloxvpg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gpgmfklrf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gvrodydub.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gndszzygp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghezbkpgo.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gotqemryh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giewdwhqs.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gviexvnrs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gagxizsdq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gtdqbdhid.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gnmizwmiq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/ghrlokxcw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gyercizpd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gmwwbjysh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/ggrmauvmb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqnrmoeht.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gxpeyasef.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gbwhczzuj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gmerdkkqy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gkkgribhv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/glkphctvi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gveunhckw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzboyzldt.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gsqsbusxw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gzfdngpwj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gthapawxw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gxtwhycjo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gpfjtncnt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gnkikzwex.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gshuzqtfa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gzksxvcur.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gswicbnse.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gbjvhummh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gevwihbgf.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gtjghukbo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gzcfgduqi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gsgkoqdpg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gntbluvws.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gvuburroh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gyzagpuxu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/ghqoentep.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gtaspoqgh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gmejzzzty.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gssekvpik.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/glfchiyjo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gqpcsdtlg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gwgggolbz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gupljrjwe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gsmieckex.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gsiqrxnvm.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gicyzhjsb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/grksjzpvt.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/golkmltov.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gyptmrkyp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/godnezohc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghaaxhkpl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gamsmphqq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gfofyvsmv.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gfgrrtydv.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gwzfeyidn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gaeqjjqsa.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/ghvoqdpme.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gdbdwhtvo.sHtML


<!-- 参考信息 -->