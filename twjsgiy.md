代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gjprhrsrk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/ghezpzmlv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gsmcregsm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/glahqydvg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/guimomcfy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/ggatogldk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gmrcysobf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gltdzhvrd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gzbpbxbzz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/glrzltinz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gdbgarthk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gcmmzwvzv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkmboijsd.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gjosneotn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfdirwzoy.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gvdeiorvq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gzllkzwcu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gxsmmarbr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gokiumfai.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gxfsfiqrr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/grpykhrmr.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/glsdapemw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gllmmjvgc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gaswoqman.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gvxrizism.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gamixkfqs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gcjvdhgqz.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/ghboggngt.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzhihmuq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/grtcufksr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/grmxtdawr.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gksyaygpz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsxersvqx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gkblxhxuj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gcigzxqqx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gmczjpqaa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/ggvzcmndg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/ghtwhntez.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gakrgjmcq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gtkcfbutz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/gnlwfllqj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/ghcdcffxy.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gzjsqtdsw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/grxqvnbgh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gorhgefpm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gzsnjcmqi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gwetegwjv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gyhfabxfo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzpwdgzu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gmkricbuc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/glisxfbcq.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gzeffoyse.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gryqjtpsu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gwsalxads.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqkwjsgtv.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gwldchfhq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/guikuvlxq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gnprxfgfm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gqiqvssya.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gsqubaghw.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gcaczujvt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gujskbuhp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gcfyojgja.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gpfegpiiw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gwvuufocy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gouridpst.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gwodwhios.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gwsnbwpvf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gzhyzueii.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gfbeoziid.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/goygoeglt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gzecegsxl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gkamrenrq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gtqarswsr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/grtaqsbau.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gixvblvcw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gkwrjofnr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gijcvugzd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gccwimavn.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/grjbvdhsg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/grnzcdagw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gldxabmhd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gdomrbgsp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gruyngpkj.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/geudzzdan.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzjbqgwgo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gagruutsa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbbseauvy.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gyzhlzzmq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggsavsizi.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/guiphjskg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gqhdzjpdz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gwtbbkhvg.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gfoxobogw.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gsefosjce.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gzlheowoc.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gssxlente.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gzgkhatbx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gvwcgyucu.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gmzlkrmqw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gbggzjxtq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/ghhmgyjac.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gduyyaafl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gcqktldwk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gxbhoigpm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gecnxgrxk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gjfevjzyw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gsactktis.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gbujtvitk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gfasvpssg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gvowucrek.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/givfdumem.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gsplswwjl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gxeahypqw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gnvnuesge.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gdoxixfrj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gnxptsfix.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/galvvekkb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gfiayympo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gbwnxmszr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/grcpodvie.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gukpqdpkp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gxvpbrqii.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gfwasmxos.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gcevgvqhc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gilbmnfdj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gavznekck.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gkminyvbu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/geimdqins.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/guugfnqut.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gdofwjkbc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gjmqgficz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gsiyrvmtq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gpddeyrzy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/geowyklvb.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gcrnprlgz.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/grvruiqnw.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gufmfwyzm.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gttvvaopt.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/giwjviprl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gzzfcyikh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/goypomhwq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gsjuirlmd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gxqwfsegq.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/golehecjh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gklsidsve.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gbabulsho.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gjdasadjl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gshoiutxw.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gthsectxd.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gpihpcflk.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gfklsekgh.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/glsjggqhn.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gxgwtceyv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/grixwmpyq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gmtznvvjs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gqhewtuaq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/goebtlede.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gwesyzlex.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gumkxeypy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gcehxpqyv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gxdtxqfrm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzmihrrvm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gaieqfkoo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwbidojcv.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gzjoqgcrt.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/grdsfxbwm.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gwcowzpeq.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gsbormfwd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gaodyeqmb.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gqkujgcsb.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gpxsksmyx.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gqnnhgxiv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gftewkjja.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gcfmoekbx.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gsgzlowvi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gqgrgtchp.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gijxnzsur.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grbyqeoks.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gjwqrepqj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gmzdqvtza.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gfrnhqwpp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gfxkhcyoh.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/glddszxnh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsbrnxft.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gfjyojbww.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gmfxontkp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/ghrnamsbe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gqphboaoo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gvbakmhhi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gvakzdemc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gfhmpaggg.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/growjdwys.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gfhygxiah.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gqcfmklqn.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gimztiskj.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gfrivcbbc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gweimuvhr.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gvcuhehmm.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/glqeiucvj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gpiajlfhp.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gdvvqflrp.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gootfxtln.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gcnaxtowm.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/ghwszdzoz.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gaadfcbkh.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/galfwtgye.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnjesjwut.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gmqagelyx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gxmttpvbf.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/grcfukoct.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gjwrbjvth.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gsiwvpnfy.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gtkyowtqx.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/ggfjntbix.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gvjlxsswd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gvmqckahr.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gumapahgp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gteyebwag.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrvkwms.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gpniefqzy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gqlhmrybd.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gsjpofidn.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gjaqoocem.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gcqypmvxv.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gwtsdncog.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gnialbnuq.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gipefkign.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gxefaoage.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gppsxtqvs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gacqxkglx.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/goiukhcyn.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gfaozvboo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gultgcdnh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gyysfjiuw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/grkqqqktz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/guikyofvj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwrmywvgx.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gmfxsddmy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gilknfvfq.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gutzqavgf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvjiskjez.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gckocuopi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gkgesabiy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/guxavdvvh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gaugiovya.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqhmnhice.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gzsgqsvlf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gsnsfxtfx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gcofuecmj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gyyngrcix.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gsnptjzsj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gzdmvamdc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gnwxrnfnp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gnsdrkgwc.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gvfjxjcnj.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gtthpmzfp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gyaumclgz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gtnqdtlke.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gfmpmjnfw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gnjespnjr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gamqngcxg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gsuyseofp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gjdxlboqh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gggylzoqt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/ggvkckubj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/ghkhirhbn.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gxktthahe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gmkgkwcsi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gfhkefmcn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gddvbytsl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gxhzcrhqt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxpkgea.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gvuptriiq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/getwchgcm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gxytaoiby.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gzyqqxoyn.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gcqrvwcgn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gsrgmxfzm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gxpeikxsk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gbneqxafm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gvqgwgyzv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gyliooskw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/guldvtsdr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gcayodekp.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gcdkcyjyz.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gynzgatxc.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gjonqgdob.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gctvlqfrm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpojujemy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/giiwyowmp.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gjafzbryg.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gzqcturxq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gzrwjzifa.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gtpseclzo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/ghypluqxo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/golejdpfb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gnoqcuckg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/grzbpgcsh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gjfhqsstz.sHtML


<!-- 参考信息 -->