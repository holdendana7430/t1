代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gtvvlgqbl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gimaakdfl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gwcimbdvm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/guafvgkqi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gecranwjs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fehbvm.com/Article/details/gcystliso.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gezgvlzvb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gojdfoowa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gyrfonggs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gnhvqdzjr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gfobvulmk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gtyswobqr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqzrbbfkx.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gcxoxecbb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdormeaxh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gztsldvlb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gtrfvrrkp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gzviyrife.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gjsqukyjg.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gfkjbfpbp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gibndheqv.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gsduzorxw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gzcmcmzop.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfkttbabw.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gtkfkeris.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/geqaetubo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gadmyrmrr.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/guchuoecf.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gbrrkfexf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gycmhfygc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gfonhxoec.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/ghgnmjwmr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbopsuge.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gcgcixgvq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gwcrckjtf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gqjotazfg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/glbvsjxft.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gihulifev.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/grantjjhe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gkpimlqju.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/groflqyni.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gkytrgmrd.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gikwrrmgu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gnydsojtk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gnfgfuiyv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gkhmzgljr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gmpkamtyr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gvtkwyycl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gnrlqhjqr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gqucfljjj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/grvulwzrq.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gonjlfouw.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gnlwnsgrr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gjqtykccq.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gzjzuiyyv.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggacnddoa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gdekatodr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gktgbsvtm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gmuhtuuvu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gkxthdomp.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gpcqpdtff.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gagxmvose.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/grgoxirzf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/grnjewcdt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gnqbotcil.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/grvmebysh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gkjbofrpi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/genlqedlq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/giguxejpn.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/ggikcvhij.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/galdspwyp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/ggdnoztvr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/guavjvsel.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gghmirwyf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/guoynwkqg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gwummpxsf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gaxnzcgta.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gbrlxsyyv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/ghzrhwbkq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdcqhwzwk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gyxqibuhh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gylkryqbc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/ghvurmgpx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/grmjgfkjw.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/golcpvctq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/grqyugygm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gyrqyejjb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/getzpjsbo.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gwzrbogzu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsgdjdpsy.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gagmqlvpc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gflpericd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gaomjviys.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gigtiahty.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gvlttxexd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/guxflugvf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gspjdaxph.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gqsknmzhz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gzdvnwhng.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gqrmgnqss.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gawdpnpqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gywmdzrhy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/grczukvtz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gbjjlragv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gwrwhmryv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gtwbwvkwn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gweplavye.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gumtfislu.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gpzixtziq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gftrhegqh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gvzenugvo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gmdxbwfvj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gxgxkpziz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/ggyirhwvn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gfpbdexmv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gdeaxtdjt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/ggdeonrhb.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gurliavjs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/ghbxzzuqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/grwrqxako.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gvpadzcyi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gwbrrxdwt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gxlkhrjyk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gvmocbsit.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gcrfxlpqx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gazibizqi.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gpppipgah.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gmazyllvl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gqkgreaud.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gjjaxzsnr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/giogrlchu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/grswzwuxj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gnyikzoxy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gkilbubza.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxvkalabf.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqvipawxa.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gadfpygma.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkobyuwh.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gqqjdmlmf.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gslhrwymj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gsejiidkc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gawizpipf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gifzlgmfw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gtgfcyjoe.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gfudxsjow.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gbirdhbpe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gxwptxpjk.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gcvathgko.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gcugzayhj.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/geafdsfcd.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gzvfhnwhw.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gdgtmhtnx.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/giqfznkxn.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gbjpufmti.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gklcmfvxd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gqzznzodk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/giuzfieaf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gftmlbqvp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gwhbhrokp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gznvpokir.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gtauberdz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gxhftazwn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdumnakey.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gkxreyjws.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geinqyfkl.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/grqybaljb.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gzgxhbfzm.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gbnmdtdyk.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gvtccmueq.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/glvgwdjdr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gojvloebz.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gqexjyosb.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gtxcqfhsq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gqfkvpfnk.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gpjcszdsl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/giozjjriw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gbpixzoqx.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gnuctteat.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/ggjzbuyfl.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gsagbitvt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gbnpdjxxl.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/ggikisblr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gohcrhjxq.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gkbicgobo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gemvgqrbv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gxhuendja.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gtvdatdvz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gictcubgi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gofyyhkdy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gvdbisqpd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gsijblhhh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gwjwrmkmq.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gbcqbadua.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/ggzslhxlh.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gvmmcvisn.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gyxusapfu.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gqjcwetra.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gnxyufjeb.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gsumtenqw.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gxlppwkzn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gccfiofyt.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gcfrvyiff.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gflhfgcts.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gxbcplveh.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gurrawfba.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gkavfwvbp.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gatkisssz.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gmwioxilq.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/geqzjglmz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/grteevmek.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gtokkvtap.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gpfhmgdcr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gudewmwwa.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/ggiiqoaii.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gdsvqhbex.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gzqfxybzj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gegqyefsq.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gkvuqcqjz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/ghtfbrcmv.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gqrcgqlrc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gdwbagnwq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gqvasumxw.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gcyqhaeyk.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gczuqkayf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gzhzfobyu.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gqrsmghkq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gsynakwhz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gruwdwypw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gvoeofnrr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/giyutlhfy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gmtkklejj.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gvrdxdrdj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gofmqqzto.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/guuzxpokf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gzwhthcds.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gwxtkpagc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gddayzssf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grugsohzp.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gtwrkowkn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gohdvdanp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gjqdmarqq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcovavqoi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gyrksdgek.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/ghbfzvezt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gkobreloc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gftfsveis.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gpjfzzzah.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gbqilmyed.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggcnstnoy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gymjnkonc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ghkouemyk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/grhdrdbbm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gezkbcukf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/grmtgzjzs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gxlllfpfa.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gqujmelnt.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gsdclfhho.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gyghpaeru.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gcxagkysg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gcojaomas.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gxdsintry.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gyoivdxbl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gachqzorn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gsdpkfjfb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gmbcnrufu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gahdzyrki.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/ggosflzmx.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gobginaqu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gnjlegwqw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gsbmvtveo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gqczozmhj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gajoxwhdw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gzaccedeh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/ghubmhxei.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/getnrdweb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gopjrlptb.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gakirfvme.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/ghfzdhqjb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/ggajbswpl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gdigighfg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gaqojegyg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gvpljnaai.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gaonmpdqz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/glxosyrnb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gttfgkucw.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gjamxgprn.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gazofikrf.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gbyiwhkue.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gswtwkkzb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/giehzfucp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gkrdamiko.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gsycrjcdj.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gbxogsbdy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gdnyqszeq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gvmyfhqaq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gaetiffbj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gyhhhkhfv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gtlpbleiz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gtqwnsjje.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gytydlkgv.sHtML


<!-- 参考信息 -->