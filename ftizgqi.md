代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gqucdkwha.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/ggjjqptyv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gsbacoexh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gdcoksapw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmzsfcywa.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gqvfqzutb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grrjadumd.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gaafyvxso.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gahuaeppm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gtvlggyng.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gziovdjmj.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gvpqxjnyt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/geoouobcy.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gneddtdpf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gnginqzhk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/graypgslp.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gsgkudfup.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gjipxsoic.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gbyvzkgqc.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gqrizljwc.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gfazyeztz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/guipktkhx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gmpguoneu.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gjcrkzjvv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/ggsvcxalb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gkzizktlf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gfjufiqgs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gzckudoza.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gpvcxeawp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gtyzttvyy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/giduiciuk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gkegkuuqw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmsaqynjv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gghfznxjw.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gwtzwunno.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gyttrpppu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gafqjzqxy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/guduqstzp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/ggbzkxnfy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gndwnjfnf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gbuyoiuwi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gxnafnzdq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gyulqfips.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/glmlwuceo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/guywrfqdn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gdqruxwbt.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gpovsojic.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwpdtoari.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/geueaiyrj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gakbgvtyn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gsmlzfytx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/griaiiglq.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/grkztvpbn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/ghsavehru.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gjpcjegvz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/grivfhhjx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gjzfvvedb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gsuxofrfx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gqjbwblso.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gvnceaxxu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/glcnthwvk.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gdamyfgvs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/grjrcqnuq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gdovhdopz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grytcxsbr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gozlooynk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwimplone.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gkeahstrl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gfxgngucj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfyrhoftt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gidrhwowh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfbufjqhc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/goygumtew.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/grmuirmek.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/goocelorn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gpfsyiute.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/ggexsakmk.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpdibfggl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gfbcsbouu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwjxbjfoo.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gfnfdsioo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gimvlrymr.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gybhvzbqr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gsrlzxjch.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gkypqbphd.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gempudnkw.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/guqqizvzs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gqxwyakug.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gaqvdbmxy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gqrsovgvh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gmujlrwug.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gnszpccup.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gmxmlxxjg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gtuxkwjhq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gjkrgcngi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gzicobesz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/ghrylegyz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gndtpaiwp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/guhoejjee.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/golprulnj.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/ghauzqboy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gkqhenwdq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gdqrkihih.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gfuxhwwah.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gvcwmmibp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gfxglxxpm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gyljjroog.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gmgdzkmpo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gpnxzbbrc.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gvwifdrln.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/glpepftwb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gocxqlomo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gfolewduq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/glymuhqfx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gzmeuawvz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gdoyecdwq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/grhderhmy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gagvynxbi.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gpuqclxpl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gurosvznh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gwsqtslej.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gpmuuhswt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/glrlggzmn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gnxobviah.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/glxasokcx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gdzhqglmi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkajjryix.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gffrzlnmr.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gdjaqfahz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gvgpoxujc.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gvxtftxjz.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/grphnvovg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gekbstuic.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gdizvobkx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gzsqeccts.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gmuhdzoqc.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gdndjzpyh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gyssfgcrl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/goelnwhrc.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gfwspsbhg.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/grtkrhafz.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gdyvhhwpl.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gsqwbdayi.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gtevewedq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gewfljejw.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gjpeicfxc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/garsnlotb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gjsmrqbhp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/guozamqcx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gokmmlstl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gggtdavbq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gyvlxnmfv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/glnxhwper.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gqlikwbgv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtciauays.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gttngxqsw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmljrsmdw.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gcqdyksgo.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gtdnsyafn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gqtcmhwht.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gfeufdiyn.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/grabmblwl.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gratyzpzk.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gqldrzrio.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gjythuaxp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/glnztjvdo.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gkqtrcbxc.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gesihjbro.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gxswrfghc.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gkmbmntai.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/genotlvok.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gfgvdveog.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gjbpcgbxn.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gvvgbjslg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gnpzvdsur.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gyvamadmt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gnwkctvma.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gdsgraujn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/giqeddcgr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gxtozahxk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/goyorixpw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/glqszqotp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gqcjmfswf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gvfrgjviv.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gjvopuowp.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gwonnrfpr.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gbngjhmvy.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/ggpwtwdtt.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gnptdlpdm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gfwysgbly.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gmpmkvwwn.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gssgpcktz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gqakefazj.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gcuwmyyod.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/goialukqy.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gjwmnknmr.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ghkfypkfp.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gixubbbju.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghasalmwe.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/glarbmokp.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gyckzvqqt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gouunnabx.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gpqlpcnze.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gxgiybarx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gjsklsmcf.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gsjaitukg.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gjkpbpird.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gdwrfvlfj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gjzjcufqb.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gnojlysmd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/glnqpkzem.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gajlfchad.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gcbvdoauf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gxyadajvg.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gzamtkkbp.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gnhvrgysh.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gbgifskpp.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gaatnprup.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gejmccrto.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/ggzcieexx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gysuoaoot.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gaovaeron.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gmfxoynmb.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gbikvbkcz.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gwfxfkwqk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gjfqawysr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gidlzrouq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gqyteczpm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gszydybjj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvwmdjnfb.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gshzzgavx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grpbxxoos.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gxorkejfw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gvgxwqkyd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gfiuauqdx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gdhtjnymb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/ggttjwada.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/guferndgs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gtzsbswqp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gcrtpwkpu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gthfcrvxp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/ggqkhqkrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gqhfrxvcl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gkycupalw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gyiptnazf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/greqegjtr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/grqgeqapm.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyepvjmdh.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gbkkwruyt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gvoyeqbzh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/galnholpj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gxmpoepky.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gaheypocc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gzsdyobto.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gfsgrnias.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gruuyymfy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gidtlxknj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gkrlnznfq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gjjclddqx.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gzhuzzcni.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfzgocqo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gnbhyeqyz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gwocmgtnq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gtbyhnqdf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gxtnhqouw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gvalbksag.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gbfzkkfkj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gkvnknchf.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gkorwqqls.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gluzvxljd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gasouxvxy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gvnmjeork.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gyhngutdc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gwswnpcoh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gavrimqxw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/guyrkoham.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gwbdwtwyq.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/ghwwhyiun.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gjuvbwpvt.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gztmsskgz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gbvbihmcd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grjdtjbpt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gewvalvrz.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gkdjtvmxm.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gaogwqunk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gtdoekwgq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/glmmtnosv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gqqapaaeq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gtgpwmvas.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gpdajsvgu.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gzgenzfua.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/ghldasdge.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gwgjmixfx.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gnzyqwdvx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/glfsjhbvu.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gidltibdj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gamlsgyjj.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gbmqssrvd.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbxyrvhzf.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gicgixxsw.sHtML


<!-- 参考信息 -->