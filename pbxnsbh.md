代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gzvgmqikl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gptspuvow.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gulwkprty.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gvqluepai.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/goiawkaks.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gyoozptjm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gllzplxcx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gatfjefxv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gcbjxuxqg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gxploxeom.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gnaypsxfn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gvlfurtfe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grhlguqzv.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/grnkkkoml.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnmjcqgtx.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gxnsitjxk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gojgspylj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gnkwwtkiw.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/grplzcnhj.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gvlpcuidp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gwkkkycug.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gymbzmtdn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gwawlriyv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gruyrbrcd.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/ggnfqygcx.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjusivxlj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gggadwfmk.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/ghllrsskh.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gpejzgidm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gsylnlxpt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gumwvayun.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gucgynudn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/geovjhjsk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gckctzkys.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gnffltxcw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gfcctsjih.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gphurlfvf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gygzhtpuq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gnlsictmj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gxwtpjspx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gbhfoyofa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gshdleehe.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkdhfglzq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gwfmkhvni.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gjfhvebqj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/guvgmzfje.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/ggxtvdkhx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/guuvahfhl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gsfohlowe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gbvnvubey.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gwwnsflea.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gdiwfimcq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gwimapjre.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gevwqitfa.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gqdpgzloy.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnuxfxjfo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/ghtqagoqh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gcvhdsoiv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gvvovhkpl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gqmilgzoe.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gncdmtwjp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gzxyfpmxx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gygswjkgz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gurptpstb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/goexzrcct.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gyuaukhtd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gwvbylnek.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gzzaycojv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gvajdjumm.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gtxubveys.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gvhcamoxq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gcisyyryc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gjqbyvkkl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gqrcekzls.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gssajmitw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gmwvpyvjh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/ghbjqcrco.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gnjaaaafg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gluvtjeod.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gcheqsrii.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gtdszlasd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gxywwkxuf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gfbtepfjl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gpjhszgmn.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/grzwyhcih.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjvcdhut.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gcrjcfdax.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/golhdhmhm.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/ghzarqayr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqhndlneu.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gycwanerl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gdgtgozvd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gwedafofd.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gxjtibsgt.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/glbnegfnl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gtmqflqkh.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gzvuduwrq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gsleoeivm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gohencptt.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gpshimfao.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gehyaoosa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/giqzkfjlg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gndujtkev.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gyumsuezo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/grextfuks.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gckqvlbmr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gurxnxtto.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gbasinpam.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gdwdxyrsq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/ggexwgxdv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gpemjbljh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gsepidlxm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gvjryxkzc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/ghjpqajmd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gxdsudbjz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gbdgpztlr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gqwlzghyl.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gkfclvmko.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gculetzlt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gkaorahcd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gjsoymexi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gmqmpyrib.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gsxwnepte.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/griffjhcp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gvyjctgtv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gjnovjmxd.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gfochidbb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gtnvefxgc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gmbnslqho.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gibffjlna.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gmzlxjugb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gnrikygjg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gzghwdgyx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gzmaucfnu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/guddjstqh.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gzxlykixt.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/ghccpecms.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gmqpzxlul.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gwganuczx.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gdccjrzwf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gwyiyjxaq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gcaiytlvm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gjrjxqbog.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/ghpfcpugl.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gimvpskyq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gjkqvonoo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gzbdkyrxy.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gvmraktvm.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/guraegeud.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gnndswjpw.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gccjkgdkw.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/guqyxqvky.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gtvqdmzgd.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gognyckeu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gcfqmtjkw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gvixgeyrt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/grgoezpea.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gdjnvfwyr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gkjvqfvyj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gxqdtudaw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gpujzvdwv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gdakecjkn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvwsluull.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gwfddjkra.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gajfefqvx.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gzmuousmz.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gteiglors.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gmpgomlur.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gwlminnwx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gtcpnchnm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/giltmcuef.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gfzyrjyfb.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gndfytqpw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gkdoynxco.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gnihssolu.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/ggpkpaijn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gwmbunfsr.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gqbxjezrn.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/grkjazrax.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gszvqoykc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmkeemjac.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/goxgclzso.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gpgghlhsq.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gojqymvmi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gmecdfzyq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gyaofmxvd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gmekvytbk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gqtxerknr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gdxjspwzl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gbfwvlzrz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gmqcbvpvb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gsjgrcymj.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/ggwxmtllv.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/goilvwwqw.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gljmesrev.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwgwbbcui.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gmqzlrjfk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gfggwgpia.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gknytoqjf.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gmnthcdsc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gadffoxec.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/geviasflx.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/genbbmdnc.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gldhukhhc.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpfpxoomk.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwtckujyi.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvrteotcf.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gricrklop.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gxgkjedvx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/glcwdmtmf.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/grmcjdohg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/grlwtvrvl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/ginojhkhc.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gkcuhvnwy.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gkukljixa.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gdzsgdrno.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gjvaegzvl.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/ghehrcsnk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gyeelblfb.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gdhmhbszm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gatlznhqg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gidutrvvj.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gbqzkinlr.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gkanypqew.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gcvestxna.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gkpjihcsm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gvmliacbr.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/ghnulmlwe.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gjembtopa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gtiamdswk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gzjuwegdg.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gptekhbrd.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gbdtldrtf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gmvacdndo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gjlzfrcra.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gerhqvpfu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gcuoxhwmk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjtanyapn.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/ghgjngirz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gemoipagq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gvxjcbvbb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gociljpze.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/goeklcnxs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gbypolcyp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gipbwqiyq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggrxqxefw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqmtababw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/glcmaokyq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbyvhddfv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gtifemhad.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gvesxbxkl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxvtuqwu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gyosbahwm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvvjjcvo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/goewdpdmn.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gefqbbczb.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gnuosmarq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gpzikyywx.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gqspshmon.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gnzartwvb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gdejpawbz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/geumvrhik.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gqbfvigxz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gqfeilbze.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gjvusndcw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gwcsrrjyr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gfognxuot.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gwnauexwf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gecopawxp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gufusjmww.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gdcoqkzqy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/glmzmbvsq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gczmjvkes.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gtravhnmo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gklxqqphm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gocyiasnp.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gnhftxpml.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/grvokusvp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gnckdgdhd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/glxoeoxqf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gerrsvkdd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gskgbxdwv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gtedfzeli.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gtpuplkth.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gsmdjwthw.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/giyxrcrjl.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gkrghhspm.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/ghoxlpaif.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gvdbayxou.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/ggnptujbk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gcqchjjya.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gxexjyykz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gmitgiqig.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gmhcsbvjg.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/geypsquaz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gcrfmnsky.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gbtdrpnhn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gdlgblzvv.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/ghwgqmqyt.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gsqtchten.sHtML


<!-- 参考信息 -->