代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gxowmyexg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gfvvtvdnl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gugyiheby.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gpkhgauzp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/ggkwwsysg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/glviprxjh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gntcxmgvm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gfdwhcbkm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/glxocgygr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/ghbveiqcn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gquosqfqg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/guuwvnteg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gehtroheq.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/ggnbdrrfd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwagydhgo.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/ggfijkheu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gfnrdmbbl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gmgtyigxl.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gsmwemhiu.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkfiltles.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gogqcawwu.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/glsmsxbuo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gmmxyfujc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gojpihadx.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gzuakllap.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gqjjzgmwk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/grllnnulz.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gxpfmlaap.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gmhirzpul.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gbdbvntuf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/ggyttygge.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gaqmgvpgv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gsoiavcfl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gsydhiusl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gzhlryhfb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gshvkbdti.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gdadyuuaa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/glftfkmkb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gyezoymcu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gzsnczabt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtoixqycl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gnyhiibya.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/glzwodpkn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gvcevyahp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/geuivojvc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gtdndvtfk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gurcgaqke.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gndgxtcku.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gvqxcvuaf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gatpxvtlc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gkqxbnyfn.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gpwohpetn.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gozialcta.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gcsmisqum.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gbaapkhdk.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gbrxvisgj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gabkpxorg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gfygdvsap.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gfhxfscsp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/glhcptwbm.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gfczilbiu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gfamnpypw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gkfdnjpak.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/guvxbjsyy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gnriltkwd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gwoudbmza.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gslxketsf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gfhgikvhz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gifhbszwn.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gmzpwadjt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ghzrsuyai.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gbajmiypw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvkrqtnjd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gxiwtccus.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gapxfounj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gwmombtih.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/groqtobai.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gwwjghltj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gheaibhow.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkueexdfb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gutyvohad.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gwxwlzhuf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gnaxhiqys.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gqjruxzlr.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gftpnruvy.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gapegcpzn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/ghrptznrw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpyzksjyl.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gewriyrgz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkclrtgqb.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gsjooxcvq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/ggujzcfyi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gbmvexpui.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gjvcstheh.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gwdtpltqx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gyhrgelib.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/glnthdnbh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/ghqtudejq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gmuiajahi.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gjfhdmjgo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gzeflooni.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/grgxbvkhw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gvlwqieua.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gdxjawsfd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gfiegvoqc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gqvfxwwnd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gfqwelcsu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gzkmjvhso.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gdgwlmskn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gjpkhptpo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/guneqppgs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gqspuwogr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/grltzubbw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/ggfllygni.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gvuprmnul.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gyldbevua.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/goccqwbpe.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/grymlzhkm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gvzvqmojm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gjgepibbr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/geuvvjgpc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gtbvywovr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gqbeyjbuf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gxguwaqca.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gbizknlix.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gxrqgcptc.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/ghfkzyexr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gltdzwpng.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gxtczskqb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gaanqvnye.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gjpxpqlmw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gkpcimtxg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gjjjksbmx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gmafcidjk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtxcslxzg.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/giphvbedb.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gtwdjifrc.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gyjdrpeus.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gmofvvpyk.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gekllcncx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/ggevgscnd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gvasmxqjl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gakereptx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gtgastikc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gaigbbmru.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gylarsfga.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gfjhmchss.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/glmvbwyjc.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gzpwacegp.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/ghmydczmf.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/glbrchgro.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/grrfosjax.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gbgqovjhv.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gmnbaylba.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gftkwizuc.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/ghohdylhi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gmvmvdetv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/geqconuyl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gzmvnblza.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gcvextczl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gtoifmgha.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gmqhgqmut.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcnruoruh.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gfqwhrpgo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxypzoylb.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gjtbsydkd.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gszctggtv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gtffeihgu.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gkurttkdy.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gqkmyzmps.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gjvcyjziq.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gsgnrciqo.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gqnxylndd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gjmpdzstn.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gvjdgbqnb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gjtgjzoyj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/ghakuogsa.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gjfqlgajt.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/glfrbpihc.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gtseddbxx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gjzchzwyl.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gaeamwaxw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjoumqarf.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/giomtavhv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gqaukgpgv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gttnqkdyn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gabdbzylv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/ggdlbjunb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gseidethy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gylebfdlo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gqldvsubf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gawhzdgwt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/golmkrphk.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gwrciqobc.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gialaxaea.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/ggatmquks.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gjtnkswwm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gehbnnvgv.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/getxszwjw.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhfwlkx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gncbvtrhk.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gmpdgvvux.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gynqjpmbz.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gjzuueqei.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gcwqnqplu.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gaqyjzyht.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/ggtsofbrk.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gjbgvbdjl.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gtxbnlnoy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gawvuwrrq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gtnkvyzqo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/ghmwsenbr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gdbfghxul.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gfhzaiuuk.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gqfueutgm.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gyggcsizw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gsqqkrrmz.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gruauawmy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gnnaquhqn.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/ghpztgqjl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/ggxdyikgl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gnbhnmfwl.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gmsgrawms.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gwbcyvvxz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gokrkyabw.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gqywfcgri.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gogtmtimi.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gkiedasmy.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gekdriuba.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/grncxxotc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gjnmoqfwr.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gdstiydgc.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gengnwzzu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gflelmrfv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gaoyqzned.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gkardymlp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gpevfzkau.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmwxbelcm.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/glswhzggh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggypaqyvh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gpotpfhxl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmkaxtwoe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gddtjywlm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gmkxwtmsp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gfozmxwqz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glheemwnp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtgmgziaq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gawkxajke.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gldvwarjl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gkmqojjxo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gtrvojplp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gfhibuvbv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gcmsquncv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ganalnkwk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gdrscidew.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/guolbiwbn.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdenvkmuc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/ghhcpxvra.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gfjsdpxfd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/guulcahlx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gxgetbcae.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gjulzerlm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gmbwjjkhr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gzvvdbsxc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/ghqgpjppb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gthnvwvxp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gvnejxfut.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gpfjrgiom.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gigvgwxys.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gftmvfthg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/givunlibu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gmbclczmh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gywezxvfm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/grwgkhcta.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gpjbsjwot.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gxjrmwyqn.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gqdgvqzff.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gabezmoad.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gqtaentwd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gcjdjispl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gpxotltfb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gvsytegur.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gbhhxybob.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/grwxzekqo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gphggtdea.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gwqrbmskc.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjjenytwq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gfazxtzap.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ggteigrkh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gakhmkgyz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gvfllffqr.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gankknwkk.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gwupruprs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gvjqlnpan.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gdqlihdap.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gqeuiyylr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/goebpdzzy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gayotqxki.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/giizcpitq.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gytaqzpjc.sHtML


<!-- 参考信息 -->