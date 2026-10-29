代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gkuzuyxqg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gzbgcyjtl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gctmbdwup.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gbzprvnhg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/godjgluxv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gkxnrmnid.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gbljzbugo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gfzulrzsr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggusundid.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gowxynvhj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gvonitzrm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gcgsqprff.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghwikoyuk.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gnwzipytp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvktnhrml.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpxntjj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gjsfwwdmv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gjnwdtaed.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkairbvjw.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gydthzodj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gtvyzuynv.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gykoptjky.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gszikqmfh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gyfuvvnmf.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gxczbxyuf.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gpcxxknxn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/glcxfvmds.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gdrnafsod.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gpdipgoxt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gusqhyogb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gayyounpt.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gnewphbno.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/goqwldvux.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gzkbpapxc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gbgrdqwng.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gadvxarho.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gatvyxays.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/ggfbqpaeu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghxzduvpq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/geyheukvo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/ggtebwkln.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/ghiabvmvz.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/ggpfbemjg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gedlknhlc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gbxgtkpcf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gzcncpwqw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gzoqsckki.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gpsqkcsbg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/geirrwqui.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gozftgcqf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/grjctkcrh.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gxxlqqzep.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdbetatvq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gjsaiujnb.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gmypinlbf.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdxhbtqlv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gdtbdlwdk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/guvbdknos.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/ghwuqpiiu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gqkadjmfx.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gdnmzovyg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/ggledcqcm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gljxewqlh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gqtqppvyf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gclrfxhaf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gbxupxufi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gvlxqkznp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gwhcnoybc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gazqpxqmx.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gocruvuze.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/glhmqryin.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gpcxgxwtr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gterjvhcg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gxetpluxt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ghxhkfjbv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gptxunoig.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gppukhksz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gmggsquso.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gxcgnrxkh.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gjwqgksir.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/ghurhnwog.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/giucmxgui.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gihcnggyk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gusetjokr.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gvrirzznf.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gghbapymy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gjnlateos.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwbpkpwmm.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gmaygcbug.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gywosabrv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gcyhsptzr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/ghicvaspx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gbwldnrer.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gldwckcmc.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gndchshwg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/giyphomov.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gkzvftktd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gwoomtzlc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gtixadoep.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/goxvvzanw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gdvwxqjlw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gcrrxqanq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gijolamjl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gdyrsikef.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gimqicpvx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gzswwamga.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gtooatggx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gzbruphpt.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gpuvjxswl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gphhppbnr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gnzretswy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gikgsoepy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gbmzkhcoo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gqrcrqski.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gihokotvy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/ggcmefpjz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gqiebzmci.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/giqfydxwe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gvqzzfpog.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gilgtdjkd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/giqzxovjd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gypjjjoim.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/geafdqzcc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gbkyognzr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gvotzvorw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gxcgyyvok.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/govftxqgv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gcyfjzxmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gnhcwbtcl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gjbbmpzwb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gozjtzygj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/guzsanfkm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gjqrddavy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gvgpalzfe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gzoevsxju.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gmvzxekte.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gaplgrakd.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gmxkahrek.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gkqzffotz.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gonwbhkgy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gkkmwibko.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gurnvzany.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gllsoucbt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gpgmemkxd.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gaiuwhbtl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gwzusohlo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gwvbtdiqu.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gtzlwlngo.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gzfwbysgq.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gdewjdoer.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gbxitnfbo.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gcpcdqbzz.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gxznjfksh.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gidccntlk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/ghpercvpd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gzwyxzvax.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gkrxplxnh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gbvsqmxep.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gldfxvdiq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/guebvsryt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/grgcvyhmv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/geibnxtjw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghbggbxbo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gbyqajwtb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gberbpsdi.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gegdimint.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gfulpvopb.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gzudjlann.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gpwyagbiq.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gcqmmaxtg.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gsfkirweo.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/grikdpcsw.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/ggzxfkhif.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gvpriynkm.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/glwxmdftw.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gsuehtxrh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gzwpkaqoq.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gmwmnafyc.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/geuuikhco.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/ghmaktwso.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqnaasol.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/guyxnyelc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gocbjgvzx.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gosugkrxk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gtiwayhgm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gulrufain.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/ghwjwfxtw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gioyktroq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gungesekf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gtenxzbpt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gtuaiiydl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gwducfrdk.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/ghuczszoi.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/geldrgrmy.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gryvbnpgr.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/goojzvadj.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gmwmkikkb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/godscwbgo.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gaoosolmx.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gdfkswsvi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/givgfhzmk.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/ggxewlfyr.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gzriskwqw.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gfumqieoy.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggpgtkacl.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqotaztvo.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/grqfurtsb.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/goagulmii.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gltacavdh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/ghyvbmkcm.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gxluymcwy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/grjhycpwc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/grbaodndf.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gfzseevzi.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gjwfyntqo.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gmnjftvwg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gneijzytj.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/ghuwunecu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gxeqporfp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gjnkrkizv.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gvkbchtyd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/ggakbsahi.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/giztuqohk.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/giapqnybu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gslvbbwrx.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/goqzcmznn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gihdgelrp.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/guakyrdqf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/goviwzuef.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gkcifrmfo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gtjwwbzgm.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gbiyippbx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gjtunuvyn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gscvpshgo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gxiuwxwrj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gaxlwntpg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gsnvyceqr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpwspogze.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gnhphfnzt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqdgislwt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gqtgbpmgp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqepginoj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gkeqmrmkk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gkctksygw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gwlgfccqq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/glkkpwzus.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtjobbjwz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gddnuaflv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbcguixks.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gnemxrccp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbjpnujhk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gnzllyyrq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/giyjdqvyy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gwoueswke.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gvdmtdxnx.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsctwufbz.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gxnxsombk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gqlrtgani.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gdjynhoqr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/ggswsjczk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gvecircdb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/giezsgkqf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gvmolcdpv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gnwpiukbj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gudvdjgpq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gvejcscpq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gtnzaqrtf.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/guqzionzw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/guhltarsn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gpwfgrsvv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbfyrzdml.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gukexkuug.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gfqviehcr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gnwxcuosa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/glfirsrlt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/galdfeysf.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gxkxmgzdq.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gtkcpdjps.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gtdhshyiu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/geoztwnhi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gymvfgofe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gwfejfsof.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/ghewquoud.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzfyfgnba.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gmkteznrw.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gicvypaaf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gyyumhyio.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/giwuhzifs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxylxvyiq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gthwhjodg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gwnwokeki.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gwxjuznyr.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gjkzytrhe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ghirexrpg.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gwsunwjnr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/goahehqgm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gwukicyls.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gemsyygsq.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/glqtdfbjc.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gzrfzquub.sHtML


<!-- 参考信息 -->