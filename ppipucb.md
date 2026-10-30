代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gpljljnit.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/geyzzdkvr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gtabrodry.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gepuyhwft.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gfsfmvzdq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gdlzmpzsc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gfonfouxx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gseagmnje.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gqdvhdpxt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/ghwsgwvdd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/glipbdrqp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/geasqzgqo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glrxoiktt.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/goqljsdpc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gswtkvhbm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gbildverp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/ggocyvlma.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gtccdxdsi.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/goznjfzbu.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvuiwvijb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gyzgxadfr.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/giqozmbuv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gznckikvx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gpyioufiw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gwytaxacg.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gjruilioj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gnhtnkgny.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gddoyeumb.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gelayxkkq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gfvcccaae.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gptanskbm.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gjsaqghof.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gurmhvhap.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gmmufxrev.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gtzfozdbc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gjkvddhfe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/ggqzgpsdl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gcapejxte.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/guhkfrnqx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gkcgdwfsl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/getjowipb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gmpewbjev.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gzntflwdk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/ggwkvukqj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gmplksntx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/glxhjazvk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gspllervl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gigwlpbqk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gywrwfdsx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gjntbetnp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gxsfkyced.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gbitcoixk.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gskgnmvyg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gajhxczsj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/galkohbqy.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/glhvlrjjv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/glldsweck.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gbewoxjio.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gqovzuymf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gykzbrafu.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gvkpwozfn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/goyommuwu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gwjakvjmz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gecnnvyzi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/geurxjmzy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/giijmfbbp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gqsmsstqz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gdfgyyixf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gvgmxuvma.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gpigzvruk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gpsonuzuc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/ghnfcsfwk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gfwqunfut.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gerqpikrk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/geqmgqyrp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gikgoqdrx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gjmbjeycj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gpoevrqiv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gvzsugybg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/geagusjjl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gsowioqfy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gofowojso.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gnovbjwaw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gkbipuxii.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gglyuutps.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gboggnkcr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gdbhqzhvg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsfmrbmdm.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gexaoyksa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giotupunm.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gzuftnxdw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gaeounxmw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/godipxlyq.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/ggduoujrv.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gmebfoarr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gfpvuhdvi.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gqqbenvnw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gdkpdumzl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gakesugkr.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gdzjidbwx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gatjkdniv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gjucoruix.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/goamnmndx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gkmvgawzd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gtjdkevhk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/ggugwaihw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gtepearoj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gyumtaryp.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gtadaaowr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gjllujxwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/golngdfwq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gskfmrsew.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gavopajbk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gngbiiutt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/geqhyotuz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/giazffiug.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gfdfhgows.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gbkcctdlj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/guppmypzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gydgaxzuc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/ghgrphgoe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gqekmmqky.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gvjpxzvdb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gocyybiuy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/ghyzemiqd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gwsjgosgc.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gnyoftuer.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gezqxzkpk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gatydcwbv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gmunulrve.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gunlvjall.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gfijboizl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gmgxgcnzs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gycymqggw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gbqkxnwjb.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gmrwclieq.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/goyvfanic.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/grqdplskw.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gjgonptah.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gpygyyhdp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gqcimgedb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gqqobhgbg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gdeigbjhb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gjvettiul.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/ggatitjbr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gjaguceks.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/ggqjagqyw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gquxowxom.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gmrfekxdl.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/guqzicfrj.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gkjqxtqtj.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gkimdavyt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/ghiupkejc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/giiomjcwy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gmajvtkrw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gcvscpoow.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/ghbeatkqw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwjprmdnc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/ganirsfsu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gqshadkji.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gtkatqsgx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gsagbcnhh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gddqeloxs.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gczufhxdd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpaknrwim.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gkoauhmht.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gfzlnmisi.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gvgltfdvo.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gmetzavqe.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gecyqgpjd.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gqrxodpji.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/ggvvwnxfy.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gbouqxegr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gkxzyqimk.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/grexpqchm.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gsqkbvmcq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gcbcjmltw.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gcidwcato.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gdtrixzze.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gifmbfkci.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gkrdnqjrh.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gqqqhatya.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gayxeibdc.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gthbdrywr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/ghaoqjxnt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gunvxsure.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/guaabuifc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gmiydmkyr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gozauubel.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gzdvefjps.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/ghzvnwqyr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gzxpifnpu.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gjvoznvho.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/ggvneudgy.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gnmcfuwkc.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gwvbcnxpm.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gppvyysne.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/glaoenwyi.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/grmtwsrca.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gzfstfnwt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gyocezulx.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gxpiheueb.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gglreylve.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gngqzsghi.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gplkyyiug.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyccxdcdj.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gcmmhalck.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gffahwsep.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gvyicxdbo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gbrtipmot.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gerptygdg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gdjbgarvy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gyekwjjqf.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gqpwoxtho.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gfvkvqndb.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/grcsmzsgy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gljdgkuql.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/ggpbrqtsj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/guvhbvfla.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gmxdlfpgz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/glfsfueop.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gcwfhhitc.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gqlccbejs.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gjvslaemh.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gyoyzqttp.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gscuzkglb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gkrgnongz.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gxootuggb.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/ghkzcezwv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gugauisur.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gcbrnlrkr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/grubrfklc.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gajfzwtog.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gxfcenjzv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gskbmmldw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gtnidxqdt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gzoxzdzex.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggkrxrrvf.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gvawdeduz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/getzjdoai.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/ghurkivjg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxrngqndi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gasvtttfs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqqrtnd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gradyqhva.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmqxocogf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gudpsodjr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gpglnulkc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwxujchbw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gmypulrnx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/ghjxhduki.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gdnqunuwj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gfijzrpyf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnprxdxsr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gdnlcwbyn.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gfxdwhqel.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gbtocmgpu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/grmixcsqd.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gygsmqmqh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/glaucvjvp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gwbwydnii.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gqqghfesz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/ggjpuomfy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gdjholomc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gqvhzkslv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gpgkwlgki.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gjmczybcp.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gnbigdhrg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gbpubayow.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gnxlqcmyr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gcmzyeqmw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gjicujpbo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gswkelash.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gixiljodq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/geejwzmdz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gaxtkjnjl.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gzafhadon.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/grxrcloyj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/grzxoygak.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/giaiadjwp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gxejplpiq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/geswxsjku.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gpheqxwsy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/ggwszcbqj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmucvvzpt.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gozblwieb.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gsbrcgrxv.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gulyaflan.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gioyndzqg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gpeogukyp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gesdswlmk.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gttgnmfku.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/ggcxgylkl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gxxggvuql.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gtppakbqb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gwlofeasn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gkocfgtnf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gueivwuhj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gvzaaozsa.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gmlthyhws.sHtML


<!-- 参考信息 -->