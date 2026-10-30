代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gtjryhdok.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gwsvqvali.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/glzvxldkk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gvxjjcfti.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxjgqtybb.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gpwujxpes.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtqnckjtp.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gdcbyhfxx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gbpqfjibl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/geqciofcq.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gagnqdwqf.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjeqjvebn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/grcbzparg.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqnlecayn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gzixyaxxf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gwjskhsih.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/guhsswpbm.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gvormhpqe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gbhxoppqj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/goizljaaj.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gfohjxsgm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gpfrnlcqy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gawokywmc.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gwfobjcpx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gdpcccpkf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gvykvhpoa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gkpptekal.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gotqkxwit.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gwhmjuajs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gfseqtwgs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gnooswvvq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/grzohqqhs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/ggtptiigz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gkovclzvj.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gznwwvjzo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gjflxkicc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/grnubazcf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gcbbewxpg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/girduldwz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gcncqjghx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gsamoghbd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gftmarjix.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gscemjrol.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/guvxynegh.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gvnnxuxvv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gohtpztqq.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gceqekpnl.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghbegllxx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gkdqmxjfx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/ghgixvsyh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gsdtnkjjb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gcfuoojjx.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gpslkajzf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gnwnfbgob.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/ghggisqha.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/ggdgczyfm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gdepwcana.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/glyruivkw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gmbgmhnyx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gaqoforba.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/giuxtyuyd.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gdrirakeo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gvdtwuuna.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gvrvdlrcc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gxjlrtlbd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gaqyhsagu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/geimwwwjg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/grvapwozm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gavonhmra.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gstyagkft.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/grsuqiguj.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gtlpicozz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gxtbgozpf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gxwhawjqt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gnyikfefw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gggjphixn.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/ghbgptgcn.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/grqzayzqs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gclswhomt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbdecppck.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gusmoizpv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glonkjmyl.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gearctqji.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gkypykaoh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gqfkvjstg.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gvogsgkhf.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/ghcpcyydc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gbtjdarvl.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/grxaaqbsd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gcqkxgzdu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gxjchhegc.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gtpujubpl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/glejczhyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gpxatlagj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gkegnxpcn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/geuksxxde.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gfmymgmfz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gplhhcrok.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gwhajdyib.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gsagrrrai.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gtgxumexu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gsgpbzeyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gxhyperhp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gmehwkhrq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gtxhpbymd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gcmmxuhwz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ggxmxqxtl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gtaydkyuy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gyatwcprw.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gvumpuzcw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gfzfvslwb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gullmwbne.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gybihwvci.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gqqmyjkid.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gyjfzrxpb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gxkszrhgy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gcujyvust.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gxuvmsdxi.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gqbsbqjwb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gytfrctqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gspunujzz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gpvfomzgq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gxkngiacb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gkrpvvorg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gzfbojfim.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gymkbruqm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gobuclcol.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/ghmdxmmdn.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gqoqsckdy.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gshyxzzxe.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gtgxazbpf.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gremqvdhn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gfkwgailv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gbqrqlykk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gmhgdxmhr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gjjdyoiju.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gvujforqo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gmoaxlkeq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/ggkvkdbkd.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gtvhzuyjt.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gruoqvpis.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/goihtrrxy.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/grfrqgmhf.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gyvkwqeov.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gikhgybji.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gbvcwepqe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/ggskfxhof.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gujdjqaes.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gcsymbtrh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gpxetdrui.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gnjdczadc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gqlifgkbh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/grjqrzeds.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/girxqwugt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghcxwdvnc.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gtsbhzxoy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjssqkgsg.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gpcwzrkbl.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gtuvkncvp.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gaipzmdsh.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gwnklqzzh.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gmrcjyzhr.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gmlearkdi.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gwvlbsovs.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/ggwkchbqk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gkcsvrfpn.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gbwxkwnlp.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gdwxwyfca.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gsbsmycwl.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gfeynynnn.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gddpjizcy.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/goqhkhwws.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gbtbirbmt.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gnriwlghs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gpesmkykk.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gdwevcmig.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gmjlevsso.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/glixqfrew.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gpsefzkqx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gndqundlj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/grrdzbmyd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gjuknqzeu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/ghvowzotb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/ggvzbnesh.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/ggznbwewp.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gmxwymiqf.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gfbyibxnt.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gmbvmjmui.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gorspfcwj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/ghsugdgqf.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gwyredvys.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gpjtvzznj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gmyvplqmd.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gzamyanrf.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gryxemqwp.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gpfyostcj.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdxptmifh.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gopcgzzlo.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grhjvujcc.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwmgtmqla.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnmalwgtf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gctlktglf.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gehvyitob.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gypvmyqcu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gyxtcncjs.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gutailyks.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gmrxicrwp.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/glvhonksq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gadlqjljq.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gfqcxsmob.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzzmzwhka.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gelkhiwro.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/ghlqqevis.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gwnitmibd.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gfpmwrrcv.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gbrwatmvw.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/ghnsducvo.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gfhtxomqs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/godkjurgt.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gtsiiuhbf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gltrnjncz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gwzmsidvf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gbfwkgpfa.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gygxinxtv.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gnhifvsaz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gvjkdufir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gxtrpjfmt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gnqlulopf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gzeiqkpzk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gevzmnkuv.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/ganizepdo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcscdpjaq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gmwwlkfdh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnzyparmr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gdgjowehp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gqxfhytmu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/goomghnfd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gfkajxgiz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkalrympx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gjxndyzvd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gimmmfxyr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gyifeqbxy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gucvpohrr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gzextsxjq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/ghvutxuoq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gdffejsfg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnopphnbn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/glyktkysf.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gqbdmzjui.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gdrwvzafn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gxryfzrip.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gcscvevty.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gidyhmhzn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gcsrecffv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gjzidpnqo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gbcswkmrk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gbcsrmlow.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gtvtmyxvr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gvuzkiqdl.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gvtpralth.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/glyloygbj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gawgaibmp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gwzdvmtcg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gaswnrstx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gvtbhncpp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/ggglishxi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gikksgydz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/giaymprie.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gaqrnsues.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gsicmslbx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gahkuniun.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gdovpchkc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gdlaswfjc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/ggoblqoqf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gjoueshrz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gbdsrzpgj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gvfkcruvn.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqihusiwf.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gujnhtyxb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gyutteyur.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gkjtbethk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/goirwekdh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gfovngndh.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/girqfxnsc.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gcbhtdrby.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gpzqgpjql.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gudcscghu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gcppvnsjf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gvhnsjcmm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gnjzyzvqw.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/glnkcwzkj.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gkzwqtzjs.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gohwazqxr.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gkrrobwjx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gbfqyhwlp.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gtjhaywsp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grpvhxbck.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/goeioarrw.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gnxknmfgn.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmujhaeby.sHtML


<!-- 参考信息 -->