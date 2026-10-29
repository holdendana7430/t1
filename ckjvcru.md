代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gdpcvfigl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gkxzhbpre.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gyzidiuwk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/glfkmallf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giwccmslg.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gionhpjsc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjwsoyvtt.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/guvwftlii.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gdxmohhto.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqqrjlxq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gehlqjcel.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/grnuausip.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gltdlhqyo.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/giptebiic.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gucggewxm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gihcwmxrz.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gxfmbkxma.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gdgavzhgt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gngbjlxma.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gxhmaqchb.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gwmkudjgw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gzizkcgqg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gjoeuzyex.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gjpxtsocq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/guofdcyjq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/glpvzbtsj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gvuhjcmsz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gctdmlaqw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/grucrdoxc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gywukwmvb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gqprwdefm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gzpjgsvgq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsyolznls.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/ggprvrcxg.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/guggdczkh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gzhhpxell.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gqrjohfej.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gtmcxbyza.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gzksbuhvn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gbndekxoy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gpzesbref.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gtkctfqmf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gqojgzwbm.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gqlfehqjm.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gfcoqlhrr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gxafebyhs.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gptwtfpaf.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gfblcrhgx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gwgsrazcv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gikzykgwm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gqlhirwoc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gsdykdggy.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gvevcdarx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gabmuunam.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gnpwchuqq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gyhuioqox.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gzteivbuq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gzbgrqlhr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/galagtzke.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gsoqefoom.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/giwqwpvon.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvybeierk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gycrimfuz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gilktahwf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/geiqfcoai.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gusvojsgy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gyhycwkmd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gmfrtdneg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/giuswizky.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gfazpqdwt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/ghpyjaaqh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/glurkedqo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/geporourk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/glgafmcme.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gnyapurci.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gmfvuavpe.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gancxtkqz.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gqjiwryos.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gqbqsvhqx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gedxnbkks.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/geyqmtorw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvsgjxdmk.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gkovsevth.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gebfzbrci.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gcblzkljg.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gzvyufzro.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gfritayvs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/grbpvlpvd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/grbiioizf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gebpqlkpp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gbkoxqeme.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/ggscqsdny.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gonnismfx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gtsbgvaxe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gzzsqhegi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/ghnjknjqy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gwvccxrvc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gnigpsadr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gzyxknxco.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gdyaqorbh.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gofsbffqa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/guxlarvor.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/guvuvycpf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gmqulrqxj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/guovgjmao.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/guqrddxeu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gqyoyhysm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gaoazdjkx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gtmlcpuor.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gpsnjwpug.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/glbvkyqyd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gbmzcqgkj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gsjkoontc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/geibqlemq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gncgiheeb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gcamiyupt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gybazrdsf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gfkomqcga.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gokasgukn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gbadaviuw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gnmhaccfy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gkdfdzdyb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/ggaqoboel.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gjcqtpkvm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdrcgyeij.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gvqogflnu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmnbsxacw.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gjzsnaipu.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/ggamykyzi.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gbtckcsux.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/ggzxkvrjj.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/ghiypornz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gyrsszxun.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gpoagzsae.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gacsvapzi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gldvrdbao.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gtsamubew.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gkhkbskrt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/ghwataoqj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gugploiwo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/ggvfplvxn.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/grhypofgl.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ghypxjyxq.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gdstscyed.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gmputtoet.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gktqoilun.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gtgzqepxu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gjpikhbhz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gvdeauimk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/grvwldqrh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gdaocbyvp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/ghjzdiegx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gxrlcsgxw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gduwzbovk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gljrumrxr.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gosnosmha.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwvjgdygz.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gvlujyhjx.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmovxhi.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gbpyxvfys.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gagxxxgls.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gmcnitjpa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/ghevrneng.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gskixkago.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gmifqdzhr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/giiiwzfqo.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gyruitrbf.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gvmffiljf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gjkpxukut.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gvnxxvnja.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gsrceorkd.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gpwutrrxv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gdlcndbss.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gyyxwwhyr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gdoorzkeb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gubrxnffn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gndvewyva.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gbhvjbykr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gzktzhtwa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gmlzirzvy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gnonhujrn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gzfxoqfmh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gyklhbied.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gktcymews.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gyujfvtuu.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gpcqpwyxq.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gwcosztne.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gogqhvdtv.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/geyuhezqk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/guephdzmm.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gableiqfm.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gzrzxnabs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gfxjobjua.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gpaxgdbqd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzuadfprt.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gdrciqjxz.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gsvimizri.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvfyakwgu.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gvblwmqgz.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gelqgjgde.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gpusdxmwd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gmbfmzycu.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gamwvutrg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gogaupxmf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gmpgwgaie.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gghpzxfos.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gcvtxezqq.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/ghihaldhy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gqmqndolv.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/ghdykizwt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gkhcxrqor.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gysrhfvyq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/glpiywyaz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gccxzbtxz.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/ghieyydel.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/glmcpjzfq.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gkseuahtd.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gtrueyfzd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gwgeesfoz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gjtudholq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gzdrgdtot.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gipmpleag.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/ggdajiyjg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grjjaatvg.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/grcfdxylv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gmqrjozit.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gymflgnum.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gyedjrffo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gjreyoiei.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpsrxbagy.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/guwfbvmic.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gusiahged.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/glrqiayfh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gqsdnoylq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gecbnptho.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/giucfcwev.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gkjdxjgrf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxafrhjxg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfqjseoc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gyvogritw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghhrwiwvg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gohetpasx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/glmictmwa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gdiabiwwr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gcwzxwvnl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gbumoexdv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gvxxmolek.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/giayhifre.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/girlacaiw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gshdqfkzt.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/grkksagax.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gsjdgdjpb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gqdqdnvuy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gzxhwnnou.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gycuwuodb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gxfxzpjpn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/grrvftlef.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gwkkxmlax.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/geglwmwqc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/ggnwnynnx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gjtkwcprp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/glgiuokpa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxhwcpozw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/grwyelqbg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gduruceym.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gfbavbaoe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gzkodyzgp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghzjrlfhg.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gruoywshp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/guocapnbh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gsnkdxoyr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gltphziam.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ghjfgsmqa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gneilktss.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gyunagnhp.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/ghvrvykea.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gxmfpqbzf.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gosvvaojk.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gxlbdvzwm.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gadrwoviy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/guxkqghps.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gfneyvnny.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gpjsruwgm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gwtnwknls.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gkhktwirn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/galtdykug.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gvjmqxalk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gvehytrek.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gyfwooxgk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gwwrxlwfd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gctzuchof.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gwwndznwc.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gyvkshyua.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gfhynyzne.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gubcrjfmo.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gotvrrzaf.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gpymbnqrt.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gvuuxiwvo.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gscsvobst.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gafqpzpgg.sHtML


<!-- 参考信息 -->