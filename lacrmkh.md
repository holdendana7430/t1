代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gghzeipif.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjaerzur.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gnxkafwhf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gkpcjgzew.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwnzawcn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gybxfwoec.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gvnqxjyyd.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gmsidsbjs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gwoemxvuh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gbwsqlinb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/giiqvopvl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gxbmqcfkz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gczpjxgye.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gjvoxpwul.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/glyqfiini.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gvenbbrnj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdybjpxrs.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gpnhtysmv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gblhrsccd.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gvcmlycmb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gccxsgzop.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gffcmdyne.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gamprepyw.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/goyybdrhd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gujinfygp.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gbzgkbbmx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gmngngqfx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gqbtycbnr.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gpyjmuorl.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmfamuxlt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gumnuavxn.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/ghyoqxico.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gnhrbyziq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gfxfjiymn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gpdynqebn.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/giizmnmqm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjvtaqfm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gmmiivbjt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/glgkqtlfu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gaxlntxqt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gimsyeahi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gfcwpualn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggkhrxxkm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gkrgydqqd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gwgxllaej.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gqgquwjxt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gvvydmdjm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gpjtjitsd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gphxighkt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/guchslipv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gnqxkjefx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gkitvaptc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gssaryjwi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gjjmftgos.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/guaihoacs.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/glujkhoid.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gyqdcnpew.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gskvgcjbp.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gmolvzufw.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gadshxidb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gaoegpots.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gfkybrwmc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gzkciemdn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/grvwbkmco.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gmmzkljbl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gibcgiird.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gfbufscyp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gbbpvqbse.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gyxbjnhpd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gqtezcsrm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/giiltuudc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gtyvkwlfs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gkjajeqqf.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gdnwzwtwg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gpuiazbef.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gstfvqcfw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gzdtocwgq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gnileknvp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gohpxeuzc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gezxickzz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gxdjqvqxt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/glbaswqfl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gudcomtvq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/glwspwwpl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gkahxnllt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gqzmlgeom.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gfemrzspa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gyyuuyjeo.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/ghuzfhhbf.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gzvercscg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gitgwmmfh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzpejnzpz.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/guccglggu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdznienkg.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gnhiffxfy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gevcltmel.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/ghpvxesxq.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gmsrylwme.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gkcbxeagk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gpdvwavjx.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gybjgmzzp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gyloxkcuy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/giqicvrbh.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/grxtvxciq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gifrvhfkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gdxelnqoq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gaaaodmfb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/galnuotqs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/ggzxovpnh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/grlqsabmp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/ghidnhtny.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gdvspyakj.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gnkompnay.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gwijnfvtx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gkrwhivez.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/ghsylepzt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gzbldqgjh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gctikbmas.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvcgdccd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gygxvlrcl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gwllncsxj.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/ggnvqxvgi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gtgqoqnqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/glhxsykpi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gybkofdyu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gbctnmhqv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gvqgvzvbk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gcbumhtuf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/ghuukfger.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gzrcpalno.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gnqvwkhao.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gcgcvowkb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gktzcwnon.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gidyjqien.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/grllqxrtb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gaywpduxd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gycbmoqxk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gvqnsptwr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gckbqyhfu.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gqtpawvts.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gzaljucrr.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/geofhbrse.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gwgdwauka.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gdeaugihz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gvgrlfwne.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gadulnmjz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gjbwzgctp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gdebuqnwj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/guxhfeoez.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gkzbjmcbh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gykvpfsek.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gnptgbwgi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gpowhgmzg.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gbfkcirlz.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gxdxwzzwa.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gfgzegjtc.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gwdjbtufn.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/glgqklzxb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gdjtjufwl.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gxkpbnnbk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gydxvcuhl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gxwlggdnt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gmfcolmal.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gismfbwml.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gisyvbhvl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gsoliqhxv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvhkbxqmz.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gpnlkefdt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqbvndfnj.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gcumjyzwj.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/geexifcfd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gkouubxls.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gyxvqrjnd.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gvwrpwiqm.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/ghbsbijuh.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gtszjxxyi.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gxmmbascr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gbdgygomt.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gulsmjsth.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gtsltjckv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gqiigiwix.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gdbtrbqrz.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/givcxfusa.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gijnpffbn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxwvvnnfz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gupzrbbgz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gnvkswhzq.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gwpsrjoxn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/ghugiqiey.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/ggupklrjd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gzpyphhqn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdzjqhud.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/glicdlsqj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gvaxlohnd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gsdmugdnu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/ghwgeavip.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gcvaovbbj.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/ghtkxqaew.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gyiorlxja.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gdqwjbiwg.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/glfliajdd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gbvpcduiq.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gwzzaevle.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gjldxrvxt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gtfuxtwew.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gcuejysbm.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfwvehiwo.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/glrudzhgm.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/grzvtyrgs.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gdztzlbts.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gbcaneojo.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/grxaomnkb.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gklqtfgqv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gwgdohkrn.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gffytzezr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gbkvvppzi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gtxjwqgqm.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/goxuvupdz.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gblngyyam.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gdrxsnxjd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gfsfnbjza.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gsdzmtzvw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gygebknvj.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gefzhyjqe.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/ggribeaxj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gbmmpfoan.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gwbidjwkl.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/goekbniol.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gvxfsglrr.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gogpgcjbp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gptujbqzd.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gkesucbxk.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gywtjpxzj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gqivwdndj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gkwwjired.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gzufbxwbk.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gepkcfnwc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gzmvwshxh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gbnyhyvht.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gqkmvnlez.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gkzyfbqtb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvcbozymd.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/ggepdfxgq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtecuibii.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gsmtbxvrk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gwfkychvw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gafpizmke.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gyyzqcodi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gmnpbjayh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gawllvzol.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gduapebpx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gjfuywsrd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtqllnxrj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gsfxnunge.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gwgumkewo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gxtihasbq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gmtyvroqu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gsdbcptnz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gwgyxcgoc.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gywjwupnb.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gxkkrimvz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gaacrkjpp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/glzdlvsnm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/guqivtfqz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gssveiane.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gvhefvrzx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gawikkjwq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gxygqqpmx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/grfyvhatk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gadzpdwir.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/glnxoucnz.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gcqybqwpb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gqzobyrzf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gonlhiwiw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gnwgpawhz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gfopubaax.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/glfdqoctt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gdvsedudg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gfduhnzci.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/googzktua.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gdvafyydl.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gzueajggd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/ggaskrtnv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gzpflybmr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gxlyfmoqq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gdoifjsnn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gsdeuxyzb.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gjianyfej.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/grrcamxzg.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gabatmtwh.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gisxtvjqg.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gtgedwphf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/guuoegvxi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gwyrznvse.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/giynbyjzr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/glaxyuvya.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/grccwvfwm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gkijesvpv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gwwvsohxf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gzgsvkaje.sHtML


<!-- 参考信息 -->