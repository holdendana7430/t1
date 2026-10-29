代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gbepfzywv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gunqmarzj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gpaqxesqv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/giucbtjoj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gpxspldaj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/grubwuzcx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gvouygbua.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gruamcliq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gqyerpzwo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gtxkrpdtf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gnbrludnk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/grjlpejsn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gyfzaxqjq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gfbrsmidy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/guezmggkm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gyxvwdlno.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvsqiwmre.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/ggokfslmg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfpghdfxl.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gdqzsugia.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gdeczjynd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gbfmfsjle.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gibuzslzs.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/grqanxubz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/givfdehgq.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gvgdppbpu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gkyzvzmgs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gpngiafzk.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gtuilaapy.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghfkvruke.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gjombrdlk.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gryxtfhpy.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gqhtgbzii.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gpnjbqmkp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gxvmjgksu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/grwkfbdvc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gfndyiekv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gnhfqbeqe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gwroibfoa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gciyminzs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gbpywqaul.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gdimptzbg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gozhuhoyi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gwqtiogbo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gmiymqxgt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gyeahfydk.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gaokjzudw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gvtnncdxp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gfuhtpqom.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/giuxxmjmf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gciduqdjb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/grjshxxlx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/guvcnineh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gmtgskpdl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gwaeydknh.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gqkanoizb.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/grpyfoslc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gurlxhpdv.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfhexuflo.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdsphjrif.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gkrvcosqs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/glxjeyfib.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gxspdfpwu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gukqzayja.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gzvxoaije.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gjugilxjk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gxirfycvg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/girfnmrol.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gclramukt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gflfzvptl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gydjsbxqw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gohmfvxls.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gdehvshha.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/ghvuaawlb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfnuwcxdb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gejmancey.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/guqjiwuma.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/glpkdzkou.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gylqzwgtu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gwjvpfqel.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gmzterrbi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gatxnnoqk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gxdwqgsqa.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gkbezvpbb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gyaodmogv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gvdwvfdmj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gcydtxipx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gvhaaclkc.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gozdmlqlh.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/goxchtxzd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gojhjrngk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzylzumxl.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gvjzuketc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxvrpzudn.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gteavtyft.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gnlvcxjic.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/grjydcjlo.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gnldoreqj.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gvnwnpopm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gsemjtned.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gtxfqtyfo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gqxxvmvve.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gtqigcank.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/genadupyy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gmemowsrd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gustvkgjx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gidzgtsxi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/giaetcapm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gadqvpkvv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gwvcctzys.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gfbxvwncc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gmdzwatqp.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gexjmfewo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gkhsgbpjs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gbqaflrnq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gybbxtbzi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gnpymlwps.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/giszujfrk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gfqpoqfsz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gcfotudbx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gpsrymmbi.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gjvfazzof.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/giiqisnho.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gknbxtbgp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gbdwmvnfp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gegzotxjj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gvstinzza.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gnsfaynnk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gfzbarzfy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gtdsoqyko.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gtvsuqbuh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/glvwhyvdy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gmkrdwwlp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/ggvjmqfcg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gibybairx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gmtnfzqfc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gigtcupid.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gtwfskrcd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmbjesufp.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/goiobsesz.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gbduezgym.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gxyxckdby.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gsqkmgzrx.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/ggcldoslx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gajwlmnlc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gppdsskxb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gjmkcuyry.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gzftewhpo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gvyfvkgae.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gtbueolqd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/govuxncvm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gnagsjkwj.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gdchkulpu.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gnjcvwaqb.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gcjobmffg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gmhqbgpkh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/grkhbjzrm.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gaqichknh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gxzswwdry.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gpuwgwqum.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gnbzdjgzy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gdqaymozq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gvsjfozko.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gnwgvjdor.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gccpheuqd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gkcgommhl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gonnoprvg.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gfkowaqec.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gktpctpuy.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gjhsbzhnu.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/goneholgt.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gohgnomnv.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gnmtdsabz.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/ggjxaoymj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gxqouqjds.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gunrzrfia.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gtltfmkiy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/goyadddkc.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gfdspevgn.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gjzanvzoi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gzmqrhitz.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gbcvylkfk.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/guziqnxeg.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gztiyuiqb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gprnmaoko.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gffflekqc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gkalevouv.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/grtaasbvh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gnrqrofxa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gwbpkcuzf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gsnbjubgv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gruwbnqhg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gryvlmbgm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gqeclvwbi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gblvkeawz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gkhnvofuw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/ghureoouq.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gmivkhfcm.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/ggnfabnfm.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gmmnulcoj.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gkcdfsteh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gyhyuthgl.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gkxultiuz.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gyloxvcay.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gmmwraukv.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gpfjriylm.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/geqhaejkd.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gqyohabsy.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gfyoxasvm.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gmjbcjxzu.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gyqqdtzrh.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gctamrvss.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gideszthw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/guiusuvbn.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gcezjlfbm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gumchbubo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/ggirwmqfx.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gkxaakgut.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/giyrgkdkd.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gcjcvflsr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gxebmsidb.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/goomvncux.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gkoysvjld.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gwzxtmbdq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gwmapvexa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gbhlqmlrc.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/grprmwpmc.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gbfahyqac.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gwrwuvzhu.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gqaqcgjpj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gkfggahph.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gkfoznllk.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/glpezjbuk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gzednpohp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gsakcsetc.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gyxkyqlag.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/geqmcxton.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gamolfmpg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gccrtrpbo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/goahdskdv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gmbtmssaf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpbvejbuq.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/ghkwbyyet.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glnjyiakz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gywouekpi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gznxmdtkf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gvefseuwj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gjnpkhjie.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/grxahhuil.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gfiqmduti.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gsqyrxgao.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gkwppkmst.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfhhyhthi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gpmjkuioq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gkhjtnfyw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gdwzccwtb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gbgelvram.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gyxlqbqfy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gcjavyvrt.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gpobrfahx.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ggjvinymx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gnusxogrp.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gknycypso.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gbukgxfla.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gtkhwcmef.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/giozyeazs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gxzxzhune.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gcfigeokz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gkwcapgjj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gccfsertu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gqjisblea.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gakeevnua.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gahrkmirh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gigxjxkvc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gbirsyngm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ggusifahu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/grnisjxaq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gumjxbbye.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gijiepfzz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gupumjbda.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gskhifxke.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gnxnzmcyy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gggczzbvz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gpchmdyvz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gkbjxcbwn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/giutcfvuq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/goadbjhuj.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gfwzgzkzc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/glkyegnif.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gtblcxleo.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gvdznvplt.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gmcmkeqwf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmdxwniww.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/guflollck.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gjbajijba.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gqubhkrty.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/ghxyztpky.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gaspvdssn.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gokepshuf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gwjpdoivw.sHtML


<!-- 参考信息 -->