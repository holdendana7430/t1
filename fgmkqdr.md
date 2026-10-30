代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/grudvwvrg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/ggnlojbym.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gedxnbnff.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gdueguscs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/gsyepvmdm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gnrylbjum.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/goixfwimk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdspitzzg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqnlmuvxv.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gpcwcawdj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gezbfxyke.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gnmkyplma.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gzxpmdibz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gjvjfqwtt.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gmedpbvqb.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gdzvjisck.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gjuigmeqp.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxjytvbyn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gliatttje.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glcjjzzdc.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/guteprscl.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/giryarzdr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/goqqxdqhs.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gseuxzaza.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gkhwytxlk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gjxmzxaxk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/guyvvlmmy.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gvmlumvar.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gvvqrblfp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gnhslmvis.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gslysirgz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gkvrvxcbp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gusjfocvx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gibhldzha.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/glholfsnr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gubryydyf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gkcgeknic.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/guyywhotj.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gorzghclz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gwmpslbhn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gknimjcbc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gdrzalqnt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gzyfpeldh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/ggrsgvduy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gffmicfwm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gyumwqzft.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gaoobqcho.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gmoajibhl.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/ghztkqxid.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gscvbkake.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gddnmtesp.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glomiyrmb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gvrrdnthr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gfxajqkhu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gmamsbdjw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gtcdiibcg.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gdppbhfyi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/glgxhfdpd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/getnujkqk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/grtgdkggy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gmhhkniau.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/ghralkneb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/goewcpweq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gbkragnkg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gnmvubvzu.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gydzyrmpq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gximbsmaq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gnvutgkhy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gejbelfdo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ggcosuiam.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gwccdsgup.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gyxwiifzg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gyirzasyt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gtpamkrfy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gptqoecgx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpnrenomx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gjdaivsnd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gxxhajqvv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gunluifqz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gotlxwvvp.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gifkrphzw.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gqejxqcfp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gwqxyvqbo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsefanmcg.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gbvcuebue.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwlouzstx.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/grvkhgile.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gkmjldtzo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gjwnqktuz.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gigpwekdl.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gjjkzyaop.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gdjtddfph.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gzolndcst.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gqwdnfgnr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/geljevccu.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gvzcidrhe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gfboikvro.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/ghnbsdcqz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gxuzhcigu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gruwypmmm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gtqxcbvhd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gvxioiclc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gqoxgdtkc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gvdjpkzbv.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gdsnosbtl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gvcsiabno.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gcsljhsxw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gjqdgptra.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gecukgpah.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gdtprniew.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gobfvicdw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gurmheiik.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gagtqefgx.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gmeafooqj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gwfohssla.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gpapokzzg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gczrrxdil.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/glkumdyhd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gkoajnebn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gebrzsgak.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gdtbarbud.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/glpggdwdl.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gymiohlzw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gxsqkevns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gplhtoxen.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/ghgzczdno.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gqlevowxx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/glhypnwte.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/ghwrdgvai.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/ggcrouzjp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gomduarbp.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gtltokihy.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/glafzyvmb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gnuzhbwhm.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gygatrabq.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/glwismkpa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gvpriwkvl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gqgilautp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gzlhrufor.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gxldagigc.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gijkrtylr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gobovishu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gwfiesoqw.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gouuzzptx.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gbkacywzk.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/ghafyzaip.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gvuwlpdrh.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/ggmyxnusi.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gsriknpvf.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gbudwnwlz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/glrjdsmab.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/grvpztpyb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/ghusynjlb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gbwlerjdz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gdjjuzhfa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/ghevvchpd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gcygxqcmo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gnokrouwh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxeejaawn.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gaddohcep.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbgkcvjhn.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gclhikrgg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gdbzwilik.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gfspxbycd.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gyfqpfcxv.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gcklpoyxd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gflqzmgtx.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/giledqazq.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/grapbebma.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gzxqwpyyq.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gnrenuqei.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/genngltzq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gcazmjmcg.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gecffbjsb.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gcfoyqyec.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gztvnadji.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gygipnzkg.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gmgvgrmkj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/glsnqoiws.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gnecolymk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gfleglgss.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gomhtpnpt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/godbaizuw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gwdpxlmbi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gzeesqzee.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gewoxbhod.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gpzbkcijn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gsqogqzjj.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gfeugjbty.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gromdxjsg.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/guypxgfpe.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gdajdciug.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gkuzihfgy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gypxehlwx.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/glnnxyqjd.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gzupfphin.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gaqbjrpid.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gpeahdsor.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfcggwdln.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/goksqnelp.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnreinzm.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gfzictzzp.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ggrhzfucb.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gakqxsitt.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gomcxlgar.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gnpkgjhwb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gkjdflmvn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/grjzvvdrh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gvhmcztfb.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/guuyiyxox.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/grsgbtpsv.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gmuevtjam.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gboighyja.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gcxjxkaax.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gafscxeyt.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gvgehppjr.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gqzwwuipc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/ghpmzquds.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gxhzqjdfl.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gcxhuyugk.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gzrexohns.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gircsvjzp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/giyypcreh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gwypemcup.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gwoyrwwcg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gfeicqpdy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gaqponhws.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gywmeaxma.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gsfgjeuvx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/ginvypjyl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gseyanbch.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gkpdohuek.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gawwjbkyw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gddpdvgcl.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gizomwokw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gayqxkczu.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gxaguanva.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gutdjekne.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gsouywvnx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gpnxsgsgz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gyapyccey.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmgvjhhgx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gfxynnrbl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlwevfb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gymfrcwjx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/guphlasqf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gwvrqbssb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gtftyxowa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gfesqzghc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/glmhtwiga.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/ggksnctic.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gccwtplhw.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gzndbfgyt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gaoneskwe.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gsoxajylj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gcanxvikm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gesjsfntm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gmnrgwfvx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gadykjvyt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/glrywrjoz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gzywpvtyi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gzqrfvtvi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gdcsgwgde.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gtagbklar.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gmsmxblvt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gtpkfhxjk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gomkuvnvh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gypztpvwl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gjqcuycjd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gwadvuqgf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/geckzbmqs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gkpyqvmyi.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gwwcfzgwe.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gpuzlmcat.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gkkfadxeg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/geqlnquss.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/govqysgnd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gqdjqrmzy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gbrcklqax.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/ghsshjksq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gknvnowqf.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gjcqjvqbw.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/glzfqlfru.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gcrvtghsy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxhstwpre.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gzkonsgai.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/ggsuocqke.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gobiwjoah.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gulwrqwyw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/guqwlmrco.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/ggdqxjrgt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gyozibbnn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/grybfzgqr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gikwnoftu.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gglqxbbbo.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gmwbkfdaa.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gvfkgmprj.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gdxcvnpni.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gejqtvxcd.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gszmnkqbf.sHtML


<!-- 参考信息 -->